# Take note
_I would suggest to go and use BunsenLabs. It is pretty slick although I do not use openbox anymore. But I still use BL and then install i3._
Go to: https://www.bunsenlabs.org/

Got tired of wallpapers? 
Add this to your i3 config. Just a plain dark lazy blue colour.
exec --no-startup-id xsetroot -solid "#002244"

# openbox
Debian server (add source.list as needed)/Ubuntu server + Openbox configuration

Note:
During Software selection, untick [] Debian Desktop Environment and [] Printer server.

Installed:
------------------
- xorg
- menu
- obmenu
- obconf
- tint2
- conky
- gmrun
- feh
- gnome-terminal
- iceweasel
- thunar
- vim
- geany
- atom
- git
- gitk
- meld
- make
- linux-headers-$(uname -r)
- lightdm
- lightdm-gtk-greeter
After base :
- alsa-base
- alsa-utils
- golang
- nodejs
- npm


Quick guide:
------------------
```
$ sudo apt-get update
$ sudo apt-get upgrade
$ sudo apt-get install git
$ mkdir ~/projects 
$ mkdir ~/projects/github
$ cd ~/projects/github
$ git clone https://github.com/drachpy/debian-openbox.git
$ cd openbox
$ sudo apt-get install xorg menu obmenu obconf feh tint2 conky gmrun gnome-terminal iceweasel thunar vim geany xterm lightdm lightdm-gtk-greeter
$ sudo apt-get install gcc make linux-headers-$(uname -r)
$ cp .fehbg .conkyrc ~/
$ cp -rf .config ~/
$ sudo cp etc/default/grub /etc/default/grub
$ sudo cp etc/X11/xorg.conf /etc/X11/xorg.conf
$ sudo init 6
```

Note: if linux-headers-$(uname -r) does not work for you, just use linux-headers-generic.


Sound
------------------
To adjust your sounds (ALSA), open terminal and run:

    $ alsamixer


SSH
------------------

1. Keep alive
```
    OSX: $ sudo vim ~/.ssh/config
    Linux: $ sudo vim /etc/ssh/ssh_config
```

2. Add the following
```
Host *
  ServerAliveInterval 60
```


Atom
------------------
Setting up atom with vim-mode and ex-mode:
```
https://github.com/atom/atom
https://github.com/atom/vim-mode
https://github.com/lloeki/ex-mode
```

Shortcuts
------------------
```
C-A-space   Show root-menu - I seldom use this usually you can just use xterm.
C-A-arrow   Change workspace
C-A-w       Web browser (iceweasel) - you can also install chromium but up to you
C-A-e       Editor (geany) - basic editor
C-A-r       Run a program (gmrun)
C-A-t       Terminal (gnome-terminal) - For most of the work
C-A-a       Atom Editor (atom) - if you think you are still not getting vim/nvim to work as you like it.
C-A-f       File Manager (thunar)
C-A-x       Alternative Terminal (xterm) - Yes, separate term usually for launching apps (i.e. scripts, python apps)
```

Other notes:
------------------
1. See ~/.fehbg for the wallpaper config
2. Use obmenu to manage your root-menu (right-click)


#Screenshot

![Openbox](https://d13pix9kaak6wt.cloudfront.net/background/users/d/r/a/drachpy_1442820278_13.png "Openbox")

* you may notice that the memory consumption is huge. This is because I was doing some webapp and test pages in browsers. But you should usually have it around 120-150MiB.



#Help me help you
If you found any discrepancies specially deadlinks. Please update it as needed or email me at drachpy{at}gmail{dot}com.
