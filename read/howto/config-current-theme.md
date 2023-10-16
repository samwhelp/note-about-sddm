---
title: SDDM 設定目前採用的佈景主題
nav_order: 7010
has_children: false
parent: 如何
---


# SDDM 設定目前採用的佈景主題


## Reference

* Arch Wiki / SDDM / [Current theme](https://wiki.archlinux.org/title/SDDM#Current_theme)


## Manpage

* [man 1 sddm](https://manpages.debian.org/stable/sddm/sddm.1.en.html)
* [man 5 sddm.conf](https://manpages.debian.org/stable/sddm/sddm.conf.5.en.html)
* [man 1 sddm-greeter](https://manpages.debian.org/stable/sddm/sddm-greeter.1.en.html)


## 設定片段

* /etc/sddm.conf.d/kde_settings.conf

``` ini
[Theme]
Current=Graphite
```

> 上面這個「Graphite」指的是「/usr/share/sddm/themes/Graphite」。


## 預覽佈景主題

如何預覽「SDDM」的「佈景主題」

可以參考「 ddm-greeter / [預覽佈景主題](https://samwhelp.github.io/note-about-sddm/read/command/sddm-greeter.html#%E9%A0%90%E8%A6%BD%E4%BD%88%E6%99%AF%E4%B8%BB%E9%A1%8C)」的用法。


``` sh
sddm-greeter --test-mode --theme /usr/share/sddm/themes/Graphite
```
