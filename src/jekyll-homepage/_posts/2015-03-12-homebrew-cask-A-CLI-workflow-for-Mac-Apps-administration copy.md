---
layout: post
title:  "Homebrew Cask::a CLI workflow for Mac Apps Administration"
date:   2015-03-12 07:30:00
categories: apps
---
![Homebrew Cask Logo](/assets/cask.png)

`Homebrew Cask` provides a friendly homebrew-style CLI workflow for the administration of Mac applications distributed as binaries. It's implemented as a homebrew external command called `cask`.

An example installing `Virtualbox`, notice that, if the application was installed earlier, then `cask` will updated it.

```bash
$ brew update
Updated Homebrew from 9bbd6637 to e8b792e6.
==> New Formulae
:
```
```bash
$ brew cask list
mono-mdk	virtualbox	xamarin-mdk	xamarin-studio
```
```bash
$ brew cask install virtualbox
==> Downloading http://download.virtualbox.org/virtualbox/4.3.24/VirtualBox-4.3.24-98716-OSX.dmg
######################################################################## 100.0%
==> Running installer for virtualbox; your password may be necessary.
==> Package installers may write to any location; options such as --appdir are ignored.
Password:
==> installer: Package name is Oracle VM VirtualBox
==> installer: Upgrading at base path /
==> installer: The upgrade was successful.
==> Symlinking Binary 'VBoxHeadless' to '/usr/local/bin/VBoxHeadless'
==> Symlinking Binary 'VBoxManage' to '/usr/local/bin/VBoxManage'
🍺  virtualbox staged at '/opt/homebrew-cask/Caskroom/virtualbox/4.3.24-98716' (4 files, 110M)
```

![Home Logo](/assets/home1.png) [Homebrew cask](http://caskroom.io)

