# Notes

## Entering Developer Mode

Hold ESC and REFRESH keys while pressing the power button; follow prompts to complete transition to developer mode

## Installing Chrubuntu

    curl -L -O http://goo.gl/9sgchs
    sudo bash 9sgchs -u 14.04
    
### Installing on SD Card

* http://chromeos-cr48.blogspot.com/2012/12/so-you-want-chrubuntu-on-external-drive.html

### Hardware

#### Trackpad

From http://www.reddit.com/r/chrubuntu/comments/25n5s8/touchpad_fix_for_the_dell_11_with_xubuntu_1404/

    wget -qO- http://pastebin.com/raw.php?i=WNhXZ1Ht | sed 's/\r//g' | sudo bash
    
#### Special Keys

* http://www.reddit.com/r/chrubuntu/comments/29wb1k/volume_hotkeys_for_dell_11_on_ubuntu_1404/
    
##### References

* http://www.reddit.com/r/chrubuntu/comments/28wd8z/xubuntu_dell_chromebook_11_touchpad_fix/
* 

### References

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

# Crouton

## Installing Crouton

    cd ~/Downloads
    wget http://goo.gl/fd3zc
    sudo sh -e ./crouton -t trusty
    
## Using Crouton

Switch screens using ctl-alt-shift-> and ctl-alt-shift-< (not ctl+alt+-> and ctl+alt+<-

## Run on Startup

* https://github.com/dnschneid/crouton/issues/170

## References

* http://tomwwolf.com/chromebook-14-compedium/chromebook-crouton-cookbook/
* https://github.com/dnschneid/crouton
* http://www.itworld.com/article/2831260/open-source-tools/how-to-run-linux-on-a-chromebook.html
* http://fuyuko.net/basic-tweaks-and-tips-for-crouton-in-chromebook/
* https://github.com/dnschneid/crouton/wiki/Running-servers-in-crouton


