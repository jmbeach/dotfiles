# GNOME settings

## Switch to Static Workspaces

I like to disable dynamic workspaces and set there to be 10 by default.

To get this to work, you need to install GNOME Tweak tool first.
```sh
dconf write /org/gnome/mutter/dynamic-workspaces false
dconf write /org/gnome/desktop/wm/preferences/num-workspaces 10
```

## Setup Hotkeys

Install `dconf-editor`.

### Disable default behavior of Super key + number

Go to `/org/gnome/shell/keybindings`

Clear the values for all of the settings with names like `switch-to-application-n`

Go to `/org/gnome/shell/extensions/dash-to-dock`

Clear the values for all of the settings with names like `app-hotkey-n`

### Set preferred keybindings

Go to `/org/gnome/desktop/wm/keybindings/`

- Set "move-to-center" to `[<Super><Shift>c]`.
- Set "switch-to-workspace1" to `['<Super>1']`
- Set "switch-to-workspace2" to `['<Super>2']
- ...
- Set "switch-to-workspace10" to `['<Super>10']`

