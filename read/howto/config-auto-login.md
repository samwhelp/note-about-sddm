---
title: SDDM 設定自動登入
nav_order: 8010
has_children: false
parent: 如何
---


# SDDM 設定自動登入


## Reference

* Arch Wiki / SDDM / [Autologin](https://wiki.archlinux.org/title/SDDM#Autologin)
* Debian Wiki / SDDM / [Enable autologin](https://wiki.debian.org/SDDM#Enable_autologin)


## Manpage

* [man 1 sddm](https://manpages.debian.org/stable/sddm/sddm.1.en.html)
* [man 5 sddm.conf](https://manpages.debian.org/stable/sddm/sddm.conf.5.en.html)


## 設定片段

* /etc/sddm.conf.d/kde_settings.conf

> Auto Login

``` ini
[Autologin]
Relogin=false
Session=plasma
User=sam
```

> Mot Auto Login

``` ini
[Autologin]
Relogin=false
Session=plasma
User=
```
