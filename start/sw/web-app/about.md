---
label: need-help

title: Web Application
subsection: web-app
section: start-sw
description:
---

# Web Application
Fedora supports most web development environments out of the box or with a simple main repository package install.

For most languages, see the [language documentation for Fedora](/tech.html).

## Known Issues

### Wayland vs X
Some common development and business tools have not yet been ported to run properly on Wayland. We recommend using GNOME on X Server for now. Here's a list of common offenders:

* [BlueJeans](https://www.bluejeans.com) - Issues with screen-sharing full screen and certain windows.
* [IntelliJ IDE's](https://www.jetbrains.com) - Graphical issues, font issues depending on driver use
* [Shutter](http://shutter-project.org) - Not working at all.

### Python
Do not install or upgrade pip via other methods than DNF. Pip may prompt to self-update, but this can break the installation. Do so at your own risk.

MySQLWorkbench CE installs python-enum34 on your python 2 install, which causes issues with running python 3 apps. See https://bugzilla.redhat.com/show_bug.cgi?id=1333372
