---
title: SDDM 設定「Numlock」
nav_order: 8050
has_children: false
parent: 如何
---


# SDDM 設定「Numlock」




## Reference

* Arch Wiki / SDDM / [Numlock](https://wiki.archlinux.org/title/SDDM#Numlock)




## Manpage

* [man 1 sddm](https://manpages.debian.org/stable/sddm/sddm.1.en.html)
* [man 5 sddm.conf](https://manpages.debian.org/stable/sddm/sddm.conf.5.en.html)




## 設定預設值

執行

``` sh
sddm --example-config | grep -i '^Numlock=' -B 3 -A 1
```

顯示

```
# Initial NumLock state. Can be on, off or none.
# If property is set to none, numlock won't be changed
# NOTE: Currently ignored if autologin is enabled.
Numlock=none

```




## 設定片段

* /etc/sddm.conf.d/kde_settings.conf

> 根據目前「Numlock」狀態

``` ini
[General]
Numlock=none
```

> 將「Numlock」強制「開啟」

``` ini
[General]
Numlock=on
```

> 將「Numlock」強制「關閉」

``` ini
[General]
Numlock=off
```
