---
layout: post
title: Gnome with Ubuntu Server (20.04) 
subtitle: With graphical interface
tags: [linux, ubuntu, installation]
comments: false
---

Ubuntu server installs just few packages.
To enable Gnome desktop from command line on a server installation:

```bash
sudo apt update
sudo apt upgrade
sudo apt install tasksel
sudo tasksel install ubuntu-desktop-minimal
sudo reboot
systemctl status gdm
```
This has been tested with ubuntu 20.04.

Reference material: [Ubuntu Linux install Gnome desktop on server](https://www.cyberciti.biz/faq/ubuntu-linux-install-gnome-desktop-on-server/)

