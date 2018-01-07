# My i3 config

It's here so that I can keep track of it more easily, plus branches for different machines (maybe, the idea was good in my head)

## What's it like?

This config sets up a nice solarized `i3` with gaps from Airblader's [i3-gaps](https://github.com/Airblader/i3). Also found 
is a fun lock screen using `i3lock` and `ImageMagick`. The background is set using a file named `wallpaper.jpg` in the 
`~/Pictures` directory.

Other fun stuff includes a toggleable auto-lock, emoji's in the status bar, and a hacky logout/shutdown menu accessible by `$mod+delete`.

This config uses left alt as a modifier, with the super key modifier line commented out for an easy switch.

## Packages you should have
- i3 (or [i3-gaps](https://github.com/Airblader/i3))
- i3lock
- dmenu
- ImageMagick
- xautolock
- feh
- gnome-terminal (default terminal, `$mod+Shift+Return` to use i3-sensible-terminal)
- compton (for transparency and vsync)
- [display-visor](https://github.com/beanaroo/display-visor) (for really basic display handling)

## Contributing / Using my stuff

Feel free to use my shit, if you want. Initial i3-gaps/compton set up borrowed from a [friend](https://githubcom/bownairo), 
you can find his configs [here](https://github.com/bownairo/yoga900i3).

To put all this stuff in the right place, try this:
```shell
$ cd ~/.config
$ git clone https://github.com/zthart/i3config.git i3
$ mkdir i3status
$ ln -s ~/.config/i3/i3status.conf ~/.config/i3status/config
$ sudo ln -s ~/.config/i3/lock /usr/bin/lock
```

This assumes that both the `i3` and `i3status` directories have not yet been created in the `~/.config` directory.
The last line creates a symlink of the lock script in `/usr/bin` so that you don't have to add the `~/.config/i3` directory
to your `PATH`.

## How does she look?
![scrot.png](https://user-images.githubusercontent.com/4873335/34645283-c207501e-f30e-11e7-8390-7cea0522de76.png)
