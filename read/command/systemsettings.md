---
title: systemsettings
nav_order: 8030
has_children: false
parent: Command
---


# systemsettings


## Usage


### help

執行

``` sh
systemsettings --help
```

顯示

```
Usage: systemsettings [options] module
Central configuration center by KDE.

Options:
  --list                     List all possible modules
  --args <arguments>         Arguments for the module
  -h, --help                 Displays help on commandline options.
  --help-all                 Displays help including Qt specific options.
  -v, --version              Displays version information.
  --author                   Show author information.
  --license                  Show license information.
  --desktopfile <file name>  The base file name of the desktop entry for this
                             application.

Arguments:
  module                     Configuration module to open
```


### list

執行下面指令

``` sh
systemsettings --list | grep sddm
```

顯示

```
kcm_sddm                       - Configure Login Manager
```


### kcm_sddm

執行下面指令

``` sh
systemsettings kcm_sddm
```


## Files

| Files / `systemsettings kcm_sddm` |
| --- |
| /etc/sddm.conf.d/kde_settings.conf |
| /usr/share/sddm/themes/{some_theme}/theme.conf.user |


## Link

* Debian Package / [kde-config-sddm](https://samwhelp.github.io/note-about-sddm/read/package/debian/kde-config-sddm.html#applications)
* KDE 探索筆記 / [systemsettings](https://samwhelp.github.io/note-about-kde/read/subject/util/kde-systemsettings/systemsettings.html)
