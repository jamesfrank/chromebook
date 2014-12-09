# Entering Developer Mode

Hold ESC and REFRESH keys while pressing the power button; press control-d at boot screen and then follow prompts to complete transition to developer mode

# Chrubuntu

## Installing

Download and run Chrubuntu install script for Trusty

    curl -L -O http://goo.gl/9sgchs
    sudo bash 9sgchs -u 14.04
    
Log in using username 'user' and password 'user' and conect to a wifi network

Run script below to fix touchpad

    wget -qO- http://pastebin.com/raw.php?i=WNhXZ1Ht | sed 's/\r//g' | sudo bash
    
Run these commands to fix touchpad speed (these are supposed to be done in the above script, but fail for some reason)

    sudo mv /usr/share/X11/xorg.conf.d/50-synaptics.conf /usr/share/X11/xorg.conf.d/50-synaptics.conf.old
    sudo cp /usr/share/xf86-input-cmt/50-touchpad-cmt-peppy.conf /usr/share/X11/xorg.conf.d/
    
Fix keyboard special keys using instructions at http://www.reddit.com/r/chrubuntu/comments/1k7o1t/how_to_enable_the_volume_and_brightness_keys_on/

    sudo apt-get install xbacklight
    
Figure out a way to fix suspend

* https://wiki.archlinux.org/index.php/Chromebook#Fixing_suspend
* https://plus.google.com/+PedroLarroy/posts/6CgQypQukMa

Create proper user account, reboot, and remove original 'user' account

Continue with Linux setup steps below
    
## Installing on SD Card

* http://chromeos-cr48.blogspot.com/2012/12/so-you-want-chrubuntu-on-external-drive.html

## Hardware Fixes

### Trackpad

From http://www.reddit.com/r/chrubuntu/comments/25n5s8/touchpad_fix_for_the_dell_11_with_xubuntu_1404/

    wget -qO- http://pastebin.com/raw.php?i=WNhXZ1Ht | sed 's/\r//g' | sudo bash
    
* https://bugs.launchpad.net/ubuntu/+source/linux/+bug/1290396
* http://scottcazan.tumblr.com/post/86666983402/dell-chromebook-11-running-ubuntu-touchpad-fix
* http://www.reddit.com/r/chrubuntu/comments/28wd8z/xubuntu_dell_chromebook_11_touchpad_fix/
    
### Special Keys

* http://www.reddit.com/r/chrubuntu/comments/29wb1k/volume_hotkeys_for_dell_11_on_ubuntu_1404/
    
## References

* http://www.amirkurtovic.com/blog/installing-chrubuntu-on-the-samsung-arm-chromebook-a-step-by-step-photo-guide/
* http://chromeos-cr48.blogspot.com/2013/10/chrubuntu-for-new-chromebooks-now-with.html
* http://www.linux.com/learn/tutorials/764181-how-to-install-linux-on-an-acer-c720-chromebook
* http://www.amirkurtovic.com/blog/installing-chrubuntu-on-the-samsung-arm-chromebook-a-step-by-step-photo-guide/
* http://ardogeek.blogspot.de/2013/10/how-to-install-chrubuntu-for-samsung.html
* http://arstechnica.com/gadgets/2012/12/how-to-install-ubuntu-on-acers-199-c7-chromebook/
* http://www.hackingnotcracking.com/?p=125
* http://voltron00x.com/2014/04/06/chromebooks-part-3-beyond-chrome-os-ubuntu-and-crouton/
* https://wiki.archlinux.org/index.php/Dell_Chromebook_11
* http://www.chromium.org/chromium-os/developer-information-for-chrome-os-devices/dell-chromebook-11
* https://github.com/tsgates/arch-wiki-markdown/blob/master/wiki/Dell_Chromebook_11.md

# Crouton

## Installing

    contrl-alt-t
    shell
    sudo chromeos-setdevpasswd
    sudo mkdir /media/removable/Crouton/chroots
    sudo ln -s /media/removable/Crouton/chroots/ /usr/local/chroots
    cd ~/Downloads
    wget http://goo.gl/fd3zc
    sudo sh -e ./crouton -r trusty -t unity,audio,keyboard,chrome,unity -e
    sudo startunity

## After Install

    sudo apt-get update
    sudo apt-get install gnome-terminal
    sudo apt-get install file-roller gedit bash-completion vlc ubuntu-restricted-extras ttf-ubuntu-font-family software-center synaptic
    
* http://www.webupd8.org/2013/12/things-to-do-after-installing-ubuntu-on.html

## Using

Switch screens using ctl-alt-shift-forward and ctl-alt-shift-back

## Optional Tweaks

### Run on Startup

* https://github.com/dnschneid/crouton/issues/170

## References

* http://www.developingandstuff.com/2014/12/the-no-frills-guide-to-crouton-ubuntu.html
* http://tomwwolf.com/chromebook-14-compedium/chromebook-crouton-cookbook/
* https://github.com/dnschneid/crouton
* http://www.itworld.com/article/2831260/open-source-tools/how-to-run-linux-on-a-chromebook.html
* http://fuyuko.net/basic-tweaks-and-tips-for-crouton-in-chromebook/
* https://github.com/dnschneid/crouton/wiki/Running-servers-in-crouton

# Linux

## Setup

Install Vim

    sudo apt-get install vim

Install dotfiles

    git clone https://github.com/jamesfrank/Dotfiles.git ~/.dotfiles
    cd ~/.dotfiles
    ./install.py
