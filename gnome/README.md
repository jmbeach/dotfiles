# GNOME settings

I like to disable dynamic workspaces and set there to be 10 by default.

To get this to work, you need to install GNOME Tweak tool first.
```sh
dconf write /org/gnome/mutter/dynamic-workspaces false
dconf write /org/gnome/desktop/wm/preferences/num-workspaces 10
```

