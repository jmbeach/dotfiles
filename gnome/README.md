# GNOME settings

> 🗒 Some hotkeys I use, such as my layout manager are configured using [AHK_X11](https://github.com/phil294/AHK_X11). See my separate repo of AHK_X11 scripts [here](https://github.com/jmbeach/ahk_x11-scripts).

## Switch to Static Workspaces

I like to disable dynamic workspaces and set there to be 10 by default.

To get this to work, you need to install GNOME Tweak tool first.
```sh
dconf write /org/gnome/mutter/dynamic-workspaces false
dconf write /org/gnome/desktop/wm/preferences/num-workspaces 10
```

## Setup Hotkeys

Install `dconf-editor`.

### Set preferred keybindings

Go to `/org/gnome/shell/keybindings`

- Clear the values for all of the settings with names like `switch-to-application-n`
- Set `toggle-overview` to `['<Super>Tab', '<Super>d']`

Go to `/org/gnome/mutter`

- Clear the value for "overlay-key"

Go to `/org/gnome/desktop/wm/keybindings/`

- Set "move-to-center" to `[<Super><Shift>c]`.
- Set "switch-to-workspace1" to `['<Super>1']`
- Set "switch-to-workspace2" to `['<Super>2']`
- ...
- Set "switch-to-workspace10" to `['<Super>0']`
- Set "minimize" to `[]`
- Set "switch-applications" to `[]`
- Set "show-desktop" to `[]`

## Install Extensions

### [Dash to Dock](https://extensions.gnome.org/extension/307/dash-to-dock/)

I install this and then turn off "Use keyboard shortcuts to activate apps".

Under "Intelligent autohide customization", I turn off "Dodge windows".

### [Walkpaper2](https://extensions.gnome.org/extension/5267/walkpaper2/)

I install this so that I can have a different wallpaper on each desktop.

### [Emoji Selector](https://extensions.gnome.org/extension/1162/emoji-selector/)

🤓 I configure this to use `Win + .` to open and hide it in the top panel.

## Ubuntu-Specific Settings

The following are under `Keyboard > Keyboard Shortcuts` in system settings.

Under `System`

- Disable `Lock Screen` with `Super + L` (hit it on accident too much)
- Disable `Show all applications` with `Super + A` (I replace it in AHK_X11 with `ctrl + A`)
- Disable `Show the notification list` with `Super + V` (I replace it in AHK_X11 with `ctrl + V`)
- Disable `Restore the keyboard shortcuts with Super+Escape` (Thanks for the offer of undoing all my work on accident, but I'll pass)
- Set `Show the run command prompt` to `Super + R`

Under `Windows`

- Disable `Hide window` with `Super + H` (I don't really ever want to do this and hit it on accident too much)
