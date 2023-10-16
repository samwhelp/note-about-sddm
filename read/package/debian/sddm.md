---
title: sddm
nav_order: 8010
has_children: false
parent: Debian
grand_parent: Package
---


# sddm


## 主題

* [安裝指令](#安裝指令)
* [檔案列表](#檔案列表)
* [bin](#bin)
* [man](#man)


## Debian Wiki

* [SDDM](https://wiki.debian.org/SDDM)


## Debian Package

* [sddm](https://packages.debian.org/stable/sddm)


## 安裝指令

執行下面指令，安裝「Package: [sddm](https://packages.debian.org/stable/sddm)」。

``` sh
sudo apt-get install sddm
```

在「Debian」的環境，可以執行下面指令，來選擇採用的「Display Manager」。

``` sh
dpkg-reconfigure sddm
```

> 可以參考「Debian Wiki / [SDDM](https://wiki.debian.org/SDDM#System-wide_configuration)」的說明。


## 檔案列表

執行下面指令，觀看「Package: sddm」有哪些[檔案](https://packages.debian.org/bookworm/amd64/sddm/filelist)，安裝在系統上。

``` sh
dpkg -L sddm
```

顯示

```
/.
/etc
/etc/dbus-1
/etc/dbus-1/system.d
/etc/dbus-1/system.d/sddm_org.freedesktop.DisplayManager.conf
/etc/init.d
/etc/init.d/sddm
/etc/pam.d
/etc/pam.d/sddm
/etc/pam.d/sddm-autologin
/etc/pam.d/sddm-greeter
/etc/sddm
/etc/sddm/Xsession
/etc/sddm/wayland-session
/lib
/lib/systemd
/lib/systemd/system
/lib/systemd/system/sddm.service
/usr
/usr/bin
/usr/bin/sddm
/usr/bin/sddm-greeter
/usr/lib
/usr/lib/x86_64-linux-gnu
/usr/lib/x86_64-linux-gnu/qt5
/usr/lib/x86_64-linux-gnu/qt5/qml
/usr/lib/x86_64-linux-gnu/qt5/qml/SddmComponents
/usr/lib/x86_64-linux-gnu/qt5/qml/SddmComponents/Background.qml
/usr/lib/x86_64-linux-gnu/qt5/qml/SddmComponents/Button.qml
/usr/lib/x86_64-linux-gnu/qt5/qml/SddmComponents/Clock.qml
/usr/lib/x86_64-linux-gnu/qt5/qml/SddmComponents/ComboBox.qml
/usr/lib/x86_64-linux-gnu/qt5/qml/SddmComponents/ImageButton.qml
/usr/lib/x86_64-linux-gnu/qt5/qml/SddmComponents/LayoutBox.qml
/usr/lib/x86_64-linux-gnu/qt5/qml/SddmComponents/Menu.qml
/usr/lib/x86_64-linux-gnu/qt5/qml/SddmComponents/PasswordBox.qml
/usr/lib/x86_64-linux-gnu/qt5/qml/SddmComponents/PictureBox.qml
/usr/lib/x86_64-linux-gnu/qt5/qml/SddmComponents/TextBox.qml
/usr/lib/x86_64-linux-gnu/qt5/qml/SddmComponents/TextConstants.qml
/usr/lib/x86_64-linux-gnu/qt5/qml/SddmComponents/qmldir
/usr/lib/x86_64-linux-gnu/qt5/qml/SddmComponents/warning.png
/usr/lib/x86_64-linux-gnu/sddm
/usr/lib/x86_64-linux-gnu/sddm/sddm-helper
/usr/share
/usr/share/doc
/usr/share/doc/sddm
/usr/share/doc/sddm/README.Debian
/usr/share/doc/sddm/TODO.Debian
/usr/share/doc/sddm/changelog.Debian.gz
/usr/share/doc/sddm/changelog.gz
/usr/share/doc/sddm/copyright
/usr/share/man
/usr/share/man/man1
/usr/share/man/man1/sddm-greeter.1.gz
/usr/share/man/man1/sddm.1.gz
/usr/share/man/man5
/usr/share/man/man5/sddm-state.conf.5.gz
/usr/share/man/man5/sddm.conf.5.gz
/usr/share/sddm
/usr/share/sddm/faces
/usr/share/sddm/faces/.face.icon
/usr/share/sddm/faces/root.face.icon
/usr/share/sddm/flags
/usr/share/sddm/flags/ae.png
/usr/share/sddm/flags/am.png
/usr/share/sddm/flags/ar.png
/usr/share/sddm/flags/at.png
/usr/share/sddm/flags/az.png
/usr/share/sddm/flags/be.png
/usr/share/sddm/flags/bg.png
/usr/share/sddm/flags/bh.png
/usr/share/sddm/flags/br.png
/usr/share/sddm/flags/by.png
/usr/share/sddm/flags/ca.png
/usr/share/sddm/flags/ch.png
/usr/share/sddm/flags/cu.png
/usr/share/sddm/flags/cz.png
/usr/share/sddm/flags/de.png
/usr/share/sddm/flags/dj.png
/usr/share/sddm/flags/dk.png
/usr/share/sddm/flags/dz.png
/usr/share/sddm/flags/ee.png
/usr/share/sddm/flags/eg.png
/usr/share/sddm/flags/es.png
/usr/share/sddm/flags/eu.png
/usr/share/sddm/flags/fi.png
/usr/share/sddm/flags/fr.png
/usr/share/sddm/flags/gb.png
/usr/share/sddm/flags/ge.png
/usr/share/sddm/flags/gr.png
/usr/share/sddm/flags/hr.png
/usr/share/sddm/flags/hu.png
/usr/share/sddm/flags/il.png
/usr/share/sddm/flags/in.png
/usr/share/sddm/flags/iq.png
/usr/share/sddm/flags/is.png
/usr/share/sddm/flags/it.png
/usr/share/sddm/flags/jo.png
/usr/share/sddm/flags/jp.png
/usr/share/sddm/flags/km.png
/usr/share/sddm/flags/kr.png
/usr/share/sddm/flags/kw.png
/usr/share/sddm/flags/la.png
/usr/share/sddm/flags/lb.png
/usr/share/sddm/flags/lt.png
/usr/share/sddm/flags/lv.png
/usr/share/sddm/flags/ly.png
/usr/share/sddm/flags/ma.png
/usr/share/sddm/flags/mk.png
/usr/share/sddm/flags/mn.png
/usr/share/sddm/flags/mx.png
/usr/share/sddm/flags/nl.png
/usr/share/sddm/flags/no.png
/usr/share/sddm/flags/om.png
/usr/share/sddm/flags/pl.png
/usr/share/sddm/flags/ps.png
/usr/share/sddm/flags/pt.png
/usr/share/sddm/flags/qa.png
/usr/share/sddm/flags/qc.png
/usr/share/sddm/flags/ro.png
/usr/share/sddm/flags/ru.png
/usr/share/sddm/flags/sa.png
/usr/share/sddm/flags/sd.png
/usr/share/sddm/flags/se.png
/usr/share/sddm/flags/si.png
/usr/share/sddm/flags/sk.png
/usr/share/sddm/flags/so.png
/usr/share/sddm/flags/sr.png
/usr/share/sddm/flags/sy.png
/usr/share/sddm/flags/th.png
/usr/share/sddm/flags/tn.png
/usr/share/sddm/flags/tr.png
/usr/share/sddm/flags/ua.png
/usr/share/sddm/flags/uk.png
/usr/share/sddm/flags/un.png
/usr/share/sddm/flags/us.png
/usr/share/sddm/flags/uy.png
/usr/share/sddm/flags/vn.png
/usr/share/sddm/flags/ye.png
/usr/share/sddm/flags/yu.png
/usr/share/sddm/flags/zz.png
/usr/share/sddm/scripts
/usr/share/sddm/scripts/Xsession
/usr/share/sddm/scripts/Xsetup
/usr/share/sddm/scripts/Xstop
/usr/share/sddm/scripts/wayland-session
/usr/share/sddm/translations
/usr/share/sddm/translations/ar.qm
/usr/share/sddm/translations/bn.qm
/usr/share/sddm/translations/ca.qm
/usr/share/sddm/translations/cs.qm
/usr/share/sddm/translations/da.qm
/usr/share/sddm/translations/de.qm
/usr/share/sddm/translations/es.qm
/usr/share/sddm/translations/et.qm
/usr/share/sddm/translations/eu.qm
/usr/share/sddm/translations/fi.qm
/usr/share/sddm/translations/fr.qm
/usr/share/sddm/translations/he.qm
/usr/share/sddm/translations/hi_IN.qm
/usr/share/sddm/translations/hu.qm
/usr/share/sddm/translations/ie.qm
/usr/share/sddm/translations/is.qm
/usr/share/sddm/translations/it.qm
/usr/share/sddm/translations/ja.qm
/usr/share/sddm/translations/kk.qm
/usr/share/sddm/translations/ko.qm
/usr/share/sddm/translations/lt.qm
/usr/share/sddm/translations/lv.qm
/usr/share/sddm/translations/nb.qm
/usr/share/sddm/translations/nl.qm
/usr/share/sddm/translations/nn.qm
/usr/share/sddm/translations/oc.qm
/usr/share/sddm/translations/pl.qm
/usr/share/sddm/translations/pt_BR.qm
/usr/share/sddm/translations/pt_PT.qm
/usr/share/sddm/translations/ro.qm
/usr/share/sddm/translations/ru.qm
/usr/share/sddm/translations/sk.qm
/usr/share/sddm/translations/sr.qm
/usr/share/sddm/translations/sr@ijekavian.qm
/usr/share/sddm/translations/sr@ijekavianlatin.qm
/usr/share/sddm/translations/sr@latin.qm
/usr/share/sddm/translations/sv.qm
/usr/share/sddm/translations/tr.qm
/usr/share/sddm/translations/uk.qm
/usr/share/sddm/translations/zh_CN.qm
/usr/share/sddm/translations/zh_TW.qm
```


## bin

執行下面指令，找出相關的指令

``` sh
dpkg -L sddm | grep bin
```

顯示

```
/usr/bin
/usr/bin/sddm
/usr/bin/sddm-greeter
```


## man

執行下面指令，找出相關的「Manpage」

``` sh
dpkg -L sddm | grep '/man/man.*/' | sort -u
```

顯示

```
/usr/share/man/man1/sddm.1.gz
/usr/share/man/man1/sddm-greeter.1.gz
/usr/share/man/man5/sddm.conf.5.gz
/usr/share/man/man5/sddm-state.conf.5.gz
```

* [man 1 sddm](https://manpages.debian.org/stable/sddm/sddm.1.en.html)
* [man 1 sddm-greeter](https://manpages.debian.org/stable/sddm/sddm-greeter.1.en.html)
* [man 5 sddm.conf](https://manpages.debian.org/stable/sddm/sddm.conf.5.en.html)
* [man 5 sddm-state.conf](https://manpages.debian.org/stable/sddm/sddm-state.conf.5.en.html)
