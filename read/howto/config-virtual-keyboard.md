---
title: SDDM 設定「虛擬鍵盤」
nav_order: 8040
has_children: false
parent: 如何
---


# SDDM 設定「虛擬鍵盤」

> SDDM 設定「虛擬鍵盤 (Virtual Keyboard)」




## Reference

* Arch Wiki / SDDM / [Enable virtual keyboard](https://wiki.archlinux.org/title/SDDM#Enable_virtual_keyboard)




## Manpage

* [man 1 sddm](https://manpages.debian.org/stable/sddm/sddm.1.en.html)
* [man 5 sddm.conf](https://manpages.debian.org/stable/sddm/sddm.conf.5.en.html)


## 設定預設值

執行

``` sh
sddm --example-config | grep -i 'InputMethod' -B 1 -A 1
```

顯示

```
# Input method module
InputMethod=qtvirtualkeyboard

```




## 設定片段

* /etc/sddm.conf.d/kde_settings.conf

> No Virtual Keyboard (不採用虛擬鍵盤)

``` ini
[General]
InputMethod=
```

> Virtual Keyboard (採用虛擬鍵盤)

``` ini
[General]
InputMethod=qtvirtualkeyboard
```




## Input Method Module

在「Fedora」環境，執行下面指令

``` sh
rpm -ql qt6-qtvirtualkeyboard | grep -i 'platforminputcontexts'
```

顯示

```
/usr/lib64/qt6/plugins/platforminputcontexts/libqtvirtualkeyboardplugin.so
```

執行

``` sh
ls -1 /usr/lib64/qt6/plugins/platforminputcontexts/
```

顯示

```
libcomposeplatforminputcontextplugin.so
libfcitx5platforminputcontextplugin.so
libibusplatforminputcontextplugin.so
libqtvirtualkeyboardplugin.so
```
