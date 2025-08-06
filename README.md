# `mpv`

[mpv](https://mpv.io/) configuration for linux and windows.

- `mpv.conf` main config for linux (default file `/usr/share/doc/mpv/mpv.conf`)
- `mpv_windows.conf` main config for windows
- `shared_mpv.conf` shared config b/w linux and windows
- `input.conf` keybinds (default file `/usr/share/doc/mpv/input.conf`)

<img width="1914" height="1041" alt="A_(23-29-49)_(06-Aug-25)" src="https://github.com/user-attachments/assets/e14fa322-0aeb-480f-8881-003b76011072" />

## OSC (On Screen Controller)

- the ui elements
- when `osc=no` then NO ui elements will be present on screen. `osc=yes` shows default mpv's osc.
- you can have custom 3rd party osc like
  - [uosc](https://github.com/tomasklaen/uosc) - micro osc
  - [mpv-osc](https://github.com/maoiscat/mpv-osc-modern)
  - [ModernX](https://github.com/zydezu/ModernX)

### Setup `uosc`

```bash
wget -O ~/Downloads/uosc.zip https://github.com/tomasklaen/uosc/releases/latest/download/uosc.zip

unzip ~/Downloads/uosc.zip -d ~/Downloads/uosc

mkdir -p ~/.config/mpv/script-opts
cp ~/Downloads/uosc/scripts ~/.config/mpv
cp ~/Downloads/uosc/fonts ~/.config/mpv
```

## Plugins

### `thumbfast`

<https://github.com/po5/thumbfast>

provides seekbar thumbnails

```bash
wget -O ~/.config/mpv/scripts/thumbfast.lua https://raw.githubusercontent.com/po5/thumbfast/refs/heads/master/thumbfast.lua
wget -O ~/.config/mpv/script-opts/thumbfast.conf https://raw.githubusercontent.com/po5/thumbfast/refs/heads/master/thumbfast.conf
```

### `memo`

<https://github.com/po5/memo>

- recent files menu, saves your watch history, and displays it in a nice menu
- list of keybinds/commands are in <https://github.com/po5/memo/blob/master/README.md#custom-keybinds>


```bash
wget -O ~/.config/mpv/scripts/memo.lua https://raw.githubusercontent.com/po5/memo/refs/heads/master/memo.lua
wget -O ~/.config/mpv/script-opts/memo.conf https://raw.githubusercontent.com/po5/memo/refs/heads/master/memo.conf
```

### `chapters`

<https://github.com/mar04/chapters_for_mpv>

mark chapters in a video and have them persisted.

```bash
wget -O ~/.config/mpv/scripts/chapters.lua https://raw.githubusercontent.com/mar04/chapters_for_mpv/refs/heads/main/chapters.lua
wget -O ~/.config/mpv/script-opts/chapters.conf https://raw.githubusercontent.com/mar04/chapters_for_mpv/refs/heads/main/chapters.conf
```

### `vlcaspectratio` and `vlccrop`

<https://github.com/kism/mpvscripts>

implements VLC like aspect ratio and crop settings

```bash
wget -O ~/.config/mpv/scripts/vlcaspectratio.lua https://raw.githubusercontent.com/kism/mpvscripts/refs/heads/main/scripts/vlcaspectratio.lua
wget -O ~/.config/mpv/scripts/vlccrop.lua https://raw.githubusercontent.com/kism/mpvscripts/refs/heads/main/scripts/vlccrop.lua
```
