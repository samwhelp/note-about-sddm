---
title: sddm-greeter
nav_order: 8020
has_children: false
parent: Command
---


# sddm-greeter


## Manpage

* [man 1 sddm-greeter](https://manpages.debian.org/stable/sddm/sddm-greeter.1.en.html)


## Usage


### help

執行

``` sh
sddm-greeter --help
```

顯示

```
Usage: sddm-greeter [options]
SDDM greeter

Options:
  -h, --help       Displays help on commandline options.
  --help-all       Displays help including Qt specific options.
  -v, --version    Displays version information.
  --test-mode      Start greeter in test mode
  --socket <name>  Socket name
  --theme <path>   Greeter theme
```


### 預覽佈景主題

執行下面指令，觀看有那些「SDDM Theme」可供選擇。

``` sh
ls /usr/share/sddm/themes -1
```

顯示，類似如下

```
breeze
debian-breeze
debian-theme
Graphite
Graphite-nord
Layan
Orchis
Simply-Circles
sugar-candy
sugar-dark
sugar-light
```


執行下面指令，就可以預覽「sugar-candy」這個「SDDM Theme」。

``` sh
sddm-greeter --test-mode --theme /usr/share/sddm/themes/sugar-candy
```
