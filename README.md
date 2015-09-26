# openbox
Debian (add source.list as needed)/Ubuntu + Openbox configuration

Installed:
------------------
- menu
- obmenu
- obconf
- tint2
- conky
- gmrun
- gnome-terminal
- iceweasel
- thunar
- vim
- geany
- atom
- git
- make
- linux-headers-$(uname -r)
- lightdm
- lightdm-gtk-greeter


Quick guide:
------------------

    $ sudo apt-get update
    $ sudo apt-get upgrade
    $ sudo apt-get install - menu obmenu obconf tint2 conky gmrun gnome-terminal iceweasel thunar vim geany git make lightdm light-dm-greeter
    $ sudo apt-get install linux-headers-$(uname -r)
    $ mkdir ~/github
    $ cd ~/github
    $ git clone https://github.com/drachpy/openbox.git
    $ cd openbox
    $ cp .fehbg .conkyrc ~/
    $ cp -rf .config ~/
    $ sudo cp etc/default/grub /etc/default/grub
    $ sudo cp etc/X11/xorg.conf /etc/X11/xorg.conf
    $ sudo init 6

Atom
------------------
Setting up atom with vim-mode and ex-mode:

    https://github.com/atom/atom
    https://github.com/atom/vim-mode
    https://github.com/lloeki/ex-mode


![Openbox](https://d13pix9kaak6wt.cloudfront.net/background/users/d/r/a/drachpy_1442820278_13.png "Openbox")

#Help me help you
If you found any discrepancies specially deadlinks. Please update it as needed or email me at drachpy{at}gmail{dot}com.
