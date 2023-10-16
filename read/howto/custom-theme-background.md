---
title: SDDM 更改某個佈景主題的背景圖片
nav_order: 7021
has_children: false
parent: 如何
---


# SDDM 更改某個佈景主題的背景圖片


## Reference

* Arch Wiki / SDDM / [Customizing a theme](https://wiki.archlinux.org/title/SDDM#Customizing_a_theme)


## Manpage

* [man 1 sddm](https://manpages.debian.org/stable/sddm/sddm.1.en.html)
* [man 5 sddm.conf](https://manpages.debian.org/stable/sddm/sddm.conf.5.en.html)
* [man 1 sddm-greeter](https://manpages.debian.org/stable/sddm/sddm-greeter.1.en.html)


## 前提

* 以「/usr/share/sddm/themes/sugar-candy」這個「SDDM Theme」來舉例。
* 假設要更改成「/usr/share/backgrounds/default-login.jpg」這張圖片。


## 設定片段

* /usr/share/sddm/themes/sugar-candy/theme.conf.user

``` ini
[General]
background=/usr/share/backgrounds/default-login.jpg
type=image
```

上面的圖片路徑「/usr/share/backgrounds/default-login.jpg」是「絕對路徑」。

因為該圖片是放在「/usr/share/backgrounds」這個資料夾，

所以可以省略「/usr/share/backgrounds」，所以也可以寫成如下的「設定片段」。

``` ini
[General]
background=default-login.jpg
type=image
```


## 預覽佈景主題

如何預覽「SDDM」的「佈景主題」

可以參考「 sddm-greeter / [預覽佈景主題](https://samwhelp.github.io/note-about-sddm/read/command/sddm-greeter.html#%E9%A0%90%E8%A6%BD%E4%BD%88%E6%99%AF%E4%B8%BB%E9%A1%8C)」的用法。


``` sh
sddm-greeter --test-mode --theme /usr/share/sddm/themes/sugar-candy
```


## 圖形介面程式操作

若是在「KDE Plasma」的環境，也可以透過「圖形介面程式 ([systemsettings kcm_sddm](https://samwhelp.github.io/note-about-sddm/read/command/systemsettings.html))」來操作「更改某個 SDDM 佈景主題的背景圖片」。
