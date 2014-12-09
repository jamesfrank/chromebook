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
