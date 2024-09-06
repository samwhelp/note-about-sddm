---
title: sddm
nav_order: 8010
has_children: false
parent: Fedora
grand_parent: Package
---


# sddm


## 主題

* [安裝指令](#安裝指令)
* [如何設定採用「sddm」](#如何設定採用sddm)
* [檔案列表](#檔案列表)
* [bin](#bin)
* [man](#man)




## Fedora Search Package

* Search: 「[sddm](https://packages.fedoraproject.org/search?query=sddm)」




## Fedora Package

| Fedora Package |
| -------------- |
| [sddm](https://packages.fedoraproject.org/pkgs/sddm/sddm/) |
| [sddm-themes](https://packages.fedoraproject.org/pkgs/sddm/sddm-themes/) |


| Fedora Package |
| -------------- |
| [xorg-x11-server-Xephyr](https://packages.fedoraproject.org/pkgs/xorg-x11-server/xorg-x11-server-Xephyr/) |




## 安裝指令

執行下面指令，安裝「Package: [sddm](https://packages.fedoraproject.org/pkgs/sddm/sddm/)」和「[sddm-themes](https://packages.fedoraproject.org/pkgs/sddm/sddm-themes/)」。

``` sh
sudo dnf install sddm sddm-themes
```




## 如何設定採用「sddm」

> 關於在「Fedora」的環境，如何選擇採用的「Display Manager」。

> 可以參考「Fedora Wiki / [Lightdm](https://fedoraproject.org/wiki/Lightdm)」的說明。

假如原本採用的是的是「lightdm」，先執行下面指令，停用「lightdm」。

``` sh
sudo systemctl disable lightdm
```

會顯示類似如下的訊息

```
Removed "/etc/systemd/system/display-manager.service".
```

接著執行下面指令，啟用「sddm」

``` sh
sudo systemctl enable sddm
```

會顯示類似如下的訊息

```
Created symlink /etc/systemd/system/display-manager.service → /usr/lib/systemd/system/sddm.service.
```

可以執行下面指令確認

``` sh
file /etc/systemd/system/display-manager.service
```

顯示

```
/etc/systemd/system/display-manager.service: symbolic link to /usr/lib/systemd/system/sddm.service
```




## 檔案列表

執行下面指令，觀看「Package: [sddm](https://packages.fedoraproject.org/pkgs/sddm/sddm/)」有哪些「檔案」，安裝在系統上。

``` sh
rpm -ql sddm
```

顯示

```
/etc/pam.d/sddm
/etc/pam.d/sddm-autologin
/etc/pam.d/sddm-greeter
/etc/sddm
/etc/sddm.conf
/etc/sddm.conf.d
/etc/sddm/README.scripts
/etc/sddm/Xsetup
/etc/sddm/Xstop
/etc/sddm/wayland-session
/etc/sysconfig/sddm
/run/sddm
/usr/bin/sddm
/usr/bin/sddm-greeter
/usr/bin/sddm-greeter-qt6
/usr/lib/.build-id
/usr/lib/.build-id/01
/usr/lib/.build-id/01/88c5a42d057aea320d0d21b573bef5003b44da
/usr/lib/.build-id/28
/usr/lib/.build-id/28/45e6618f873be98e1e03c50c70a627c46fd016
/usr/lib/.build-id/31
/usr/lib/.build-id/31/554ec40a1fadf74def74959733b73e387f579d
/usr/lib/.build-id/87
/usr/lib/.build-id/87/cf5820ea94c5d67106e4665be14d1f46846eb1
/usr/lib/.build-id/fd
/usr/lib/.build-id/fd/86c7f9fda884c8ffaf44e77edee55e18eb9931
/usr/lib/sddm/sddm.conf.d
/usr/lib/systemd/system/sddm.service
/usr/lib/sysusers.d/sddm.conf
/usr/lib/tmpfiles.d/sddm.conf
/usr/lib64/qt6/qml/SddmComponents
/usr/lib64/qt6/qml/SddmComponents/Background.qml
/usr/lib64/qt6/qml/SddmComponents/Button.qml
/usr/lib64/qt6/qml/SddmComponents/Clock.qml
/usr/lib64/qt6/qml/SddmComponents/ComboBox.qml
/usr/lib64/qt6/qml/SddmComponents/ImageButton.qml
/usr/lib64/qt6/qml/SddmComponents/LayoutBox.qml
/usr/lib64/qt6/qml/SddmComponents/Menu.qml
/usr/lib64/qt6/qml/SddmComponents/PasswordBox.qml
/usr/lib64/qt6/qml/SddmComponents/PictureBox.qml
/usr/lib64/qt6/qml/SddmComponents/TextBox.qml
/usr/lib64/qt6/qml/SddmComponents/TextConstants.qml
/usr/lib64/qt6/qml/SddmComponents/qmldir
/usr/lib64/qt6/qml/SddmComponents/warning.png
/usr/libexec/sddm-helper
/usr/libexec/sddm-helper-start-wayland
/usr/libexec/sddm-helper-start-x11user
/usr/share/dbus-1/system.d/org.freedesktop.DisplayManager-sddm.conf
/usr/share/doc/sddm
/usr/share/doc/sddm/CONTRIBUTORS
/usr/share/doc/sddm/README.md
/usr/share/licenses/sddm
/usr/share/licenses/sddm/LICENSE
/usr/share/man/man1/sddm-greeter.1.gz
/usr/share/man/man1/sddm.1.gz
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
/usr/share/sddm/flags/bd.png
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
/usr/share/sddm/scripts/README.scripts
/usr/share/sddm/scripts/Xsession
/usr/share/sddm/scripts/Xsetup
/usr/share/sddm/scripts/Xstop
/usr/share/sddm/scripts/wayland-session
/usr/share/sddm/themes
/usr/share/sddm/translations-qt6
/usr/share/sddm/translations-qt6/ar.qm
/usr/share/sddm/translations-qt6/bg.qm
/usr/share/sddm/translations-qt6/bn.qm
/usr/share/sddm/translations-qt6/ca.qm
/usr/share/sddm/translations-qt6/cs.qm
/usr/share/sddm/translations-qt6/da.qm
/usr/share/sddm/translations-qt6/de.qm
/usr/share/sddm/translations-qt6/es.qm
/usr/share/sddm/translations-qt6/et.qm
/usr/share/sddm/translations-qt6/eu.qm
/usr/share/sddm/translations-qt6/fi.qm
/usr/share/sddm/translations-qt6/fr.qm
/usr/share/sddm/translations-qt6/gl.qm
/usr/share/sddm/translations-qt6/he.qm
/usr/share/sddm/translations-qt6/hi_IN.qm
/usr/share/sddm/translations-qt6/hu.qm
/usr/share/sddm/translations-qt6/ie.qm
/usr/share/sddm/translations-qt6/is.qm
/usr/share/sddm/translations-qt6/it.qm
/usr/share/sddm/translations-qt6/ja.qm
/usr/share/sddm/translations-qt6/ka.qm
/usr/share/sddm/translations-qt6/kk.qm
/usr/share/sddm/translations-qt6/ko.qm
/usr/share/sddm/translations-qt6/lt.qm
/usr/share/sddm/translations-qt6/lv.qm
/usr/share/sddm/translations-qt6/nb.qm
/usr/share/sddm/translations-qt6/nl.qm
/usr/share/sddm/translations-qt6/nn.qm
/usr/share/sddm/translations-qt6/oc.qm
/usr/share/sddm/translations-qt6/pl.qm
/usr/share/sddm/translations-qt6/pt_BR.qm
/usr/share/sddm/translations-qt6/pt_PT.qm
/usr/share/sddm/translations-qt6/ro.qm
/usr/share/sddm/translations-qt6/ru.qm
/usr/share/sddm/translations-qt6/sk.qm
/usr/share/sddm/translations-qt6/sr.qm
/usr/share/sddm/translations-qt6/sr@ijekavian.qm
/usr/share/sddm/translations-qt6/sr@ijekavianlatin.qm
/usr/share/sddm/translations-qt6/sr@latin.qm
/usr/share/sddm/translations-qt6/sv.qm
/usr/share/sddm/translations-qt6/tr.qm
/usr/share/sddm/translations-qt6/uk.qm
/usr/share/sddm/translations-qt6/zh_CN.qm
/usr/share/sddm/translations-qt6/zh_TW.qm
/var/lib/sddm
```




## bin

執行下面指令，找出相關的指令

``` sh
rpm -ql sddm | grep bin
```

顯示

```
/usr/bin/sddm
/usr/bin/sddm-greeter
/usr/bin/sddm-greeter-qt6
```


## man

執行下面指令，找出相關的「Manpage」

``` sh
rpm -ql sddm | grep '/man/man.*/' | sort -u
```

顯示

```
/usr/share/man/man1/sddm.1.gz
/usr/share/man/man1/sddm-greeter.1.gz
/usr/share/man/man5/sddm.conf.5.gz
/usr/share/man/man5/sddm-state.conf.5.gz
```
