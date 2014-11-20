# Notes

## Entering Developer Mode

Hold ESC and REFRESH keys while pressing the power button; follow prompts to complete transition to developer mode

## Installing Chrubuntu

    curl -L -O http://goo.gl/9sgchs
    sudo bash 9sgchs -u 14.04

### Hardware

#### Trackpad

From http://www.reddit.com/r/chrubuntu/comments/25n5s8/touchpad_fix_for_the_dell_11_with_xubuntu_1404/

    wget -qO- http://pastebin.com/raw.php?i=WNhXZ1Ht | sed 's/\r//g' | sudo bash

### References

* http://www.amirkurtovic.com/blog/installing-chrubuntu-on-the-samsung-arm-chromebook-a-step-by-step-photo-guide/
* http://chromeos-cr48.blogspot.com/2013/10/chrubuntu-for-new-chromebooks-now-with.html
* http://www.linux.com/learn/tutorials/764181-how-to-install-linux-on-an-acer-c720-chromebook
* http://www.amirkurtovic.com/blog/installing-chrubuntu-on-the-samsung-arm-chromebook-a-step-by-step-photo-guide/
* http://ardogeek.blogspot.de/2013/10/how-to-install-chrubuntu-for-samsung.html
* http://arstechnica.com/gadgets/2012/12/how-to-install-ubuntu-on-acers-199-c7-chromebook/
    
## Installing Crouton

    cd ~/Downloads
    wget http://goo.gl/fd3zc
    sudo sh -e ./crouton -t trusty
    
## Using Crouton

Switch screens using ctl-alt-shift-> and ctl-alt-shift-< (not ctl+alt+-> and ctl+alt+<-

### References

* http://tomwwolf.com/chromebook-14-compedium/chromebook-crouton-cookbook/

