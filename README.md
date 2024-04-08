# Things-to-Do-After-Installing-Ubuntu-23.10
Ubuntu 23.10 brings exciting new features, such as GNOME 45, the latest Kernel 6.5, the latest refinements in the GNOME desktop, and more.

## Welcome!

This guide serves as a companion for those who've freshly installed Ubuntu 23.10. It'll walk you through essential steps to optimize your system and personalize your desktop experience. Feel free to follow along at your own pace, and explore further based on your specific needs.

## Update your system

The first thing you need to do after installing Ubuntu 23.10 (or any other Linux distribution) is to update your system. Often, the latest ISO may not contain all the updates due to time differences. So, to update your system, open a terminal window and run the following commands:

```bash
sudo apt update && sudo apt upgrade
```

## Remove Firefox Snap and install Flatpak or deb (( optional ))
Since the last few years, Firefox has come as a Snap package on Ubuntu desktops. Now, if you are an average user, this may not be a problem or a thing to worry about. However, many users may not like the Snap package of Firefox for several reasons. For example, the startup time is slow, snap update notification pop-up, etc. Although the snap experience is improving every day, you can still have options to remove Snap completely or remove Firefox Snap for native Debian package formats.

So, to completely remove Firefox as Snap, you can follow the guide on this page that I have written. It’s a little complex and may take time. And install a deb version of Firefox from PPA or use the Flatpak version.

As I said, this is an optional tip; you may skip it if you want.

## Remove Snap completely (( advanced tip )) (( optional ))
This is an advanced tip, which is optional. If you want to de-clutter your Ubuntu installation from Snap completely, you can do it using the steps outlined in my guide. Although, for general users, it may not matter much. But you can still go ahead and remove Snap completely from Ubuntu.

## Install and Enable Flatpak
Ubuntu Desktop never ships Flatpak by default and never will. And since the 23.04 release onwards, the official Ubuntu flavours also won’t ship Flatpak by default. It’s a decision which has been jointly taken by Canonical and official flavour maintainers.

That said, the Flatpak ecosystem is growing, and the Flathub app store is being curated every day with many new applications. If you want, you can set up Flatpak for your new Ubuntu 23.10 system.

To enable Flatpak applications in Ubuntu 23.10, follow the below commands.

```bash
sudo apt install flatpak
```
Then followed by
```bash
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
```
Finally Restart from the terminal
```bash
reboot
```
## How to Install Chrome on Ubuntu
To install Google Chrome on Ubuntu from the command line do the following:

Step 1: Open Terminal and run this command to download Chrome’s DEB installer:
```bash
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
```
Step 2: Use apt to install the DEB:
```bash
sudo apt install ./google-chrome-stable_current_amd64.deb
```
> **NOTE:** Google Chrome Not Supported on 32-Bit Ubuntu
Google discontinued support for 32-bit Ubuntu in 2016, so you can no longer install Google Chrome on 32-bit Ubuntu systems. If you’re using a 32-bit system you can install Chromium instead. Chromium is an open-source version of Chrome.

### Uninstall Chrome from Ubuntu
If you install Google’s web browser but later decide it’s not for you, that’s fine: you can uninstall Chrome on ubuntu just as easily as you installed it.

Open a new Terminal window and run:
```
sudo apt remove google-chrome
```
## Install additional packages
It’s important to ensure you can play all video and audio formats on your Ubuntu desktop. If you skipped the extra package installation during the setup, you could install them via the below commands.

```
sudo apt install ubuntu-restricted-extras
```
This should settle any video or audio playback problem in Ubuntu. Especially with GNOME Videos, which can’t play anything by default.

## Setup basic apps
Ubuntu 23.10 installation gives you two options: a minimal install and a base install. The minimal install only comes with basic items, whereas the base install comes with LibreOffice and other key applications.

However, whatever option you choose, you still need a few more applications for your workflow. And these are pretty common for a Linux desktop weather it will VLC or even if your looking to do a bit of gaming with Steam I will provide example of both 

```
sudo apt install vlc
```
```
sudo apt install steam-installer
```

