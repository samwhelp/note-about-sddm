---
title: SDDM 更改某個佈景主題的背景圖片
nav_order: 7021
has_children: false
parent: 如何
---


# SDDM 更改某個佈景主題的背景圖片




## 主題

* [Reference](#reference)
* [Manpage](#manpage)
* [前提](#前提)
* [設定片段](#設定片段)
* [預覽佈景主題](#預覽佈景主題)
* [圖形介面程式操作](#圖形介面程式操作)
* [額外探索紀錄](#額外探索紀錄)




## Reference

* Arch Wiki / SDDM / [Customizing a theme](https://wiki.archlinux.org/title/SDDM#Customizing_a_theme)
* SDDM Wiki / Theming / [Theme Configuration](https://github.com/sddm/sddm/wiki/Theming#theme-configuration)
* Command / [sddm](https://samwhelp.github.io/note-about-sddm/read/command/sddm.html)




## Manpage

* [man 1 sddm](https://manpages.debian.org/stable/sddm/sddm.1.en.html)
* [man 5 sddm.conf](https://manpages.debian.org/stable/sddm/sddm.conf.5.en.html)
* [man 1 sddm-greeter](https://manpages.debian.org/stable/sddm/sddm-greeter.1.en.html)




## 前提

* 以「[/usr/share/sddm/themes/maldives](https://github.com/sddm/sddm/tree/develop/data/themes/maldives)」這個「SDDM Theme」來舉例。
* 假設要更改成「/usr/share/backgrounds/default-login.jpg」這張圖片。




## 設定片段

* 設定檔：「`/usr/share/sddm/themes/maldives/theme.conf.user`」

``` ini
[General]
background=/usr/share/backgrounds/default-login.jpg
```

上面的圖片路徑「/usr/share/backgrounds/default-login.jpg」是「絕對路徑」。

因為該圖片是放在「/usr/share/backgrounds」這個資料夾，

所以可以省略「/usr/share/backgrounds」，所以也可以寫成如下的「設定片段」。

``` ini
[General]
background=default-login.jpg
```



## 預覽佈景主題

如何預覽「SDDM」的「佈景主題」

可以參考「 sddm-greeter / [預覽佈景主題](https://samwhelp.github.io/note-about-sddm/read/command/sddm-greeter.html#%E9%A0%90%E8%A6%BD%E4%BD%88%E6%99%AF%E4%B8%BB%E9%A1%8C)」的用法。


``` sh
sddm-greeter --test-mode --theme /usr/share/sddm/themes/maldives
```




## 圖形介面程式操作

若是在「KDE Plasma」的環境，也可以透過「圖形介面程式 ([systemsettings kcm_sddm](https://samwhelp.github.io/note-about-sddm/read/command/systemsettings.html))」來操作「更改某個 SDDM 佈景主題的背景圖片」。




## 額外探索紀錄

可以在「maldives / [Main.qml](https://github.com/sddm/sddm/blob/develop/data/themes/maldives/Main.qml#L58-L68)」，看到有一段程式碼片段如下


``` cpp
    Background {
        anchors.fill: parent
        source: Qt.resolvedUrl(config.background)
        fillMode: Image.PreserveAspectCrop
        onStatusChanged: {
            var defaultBackground = Qt.resolvedUrl(config.defaultBackground)
            if (status == Image.Error && source != defaultBackground) {
                source = defaultBackground
            }
        }
    }
```

> 其中有一行「`source: Qt.resolvedUrl(config.background)`」。


> 對照「maldives / [theme.conf](https://github.com/sddm/sddm/blob/develop/data/themes/maldives/theme.conf#L1-L2)」

``` ini
[General]
background=background.jpg
```
