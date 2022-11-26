# tmux-config

This repository hosts my minimalist configuration for `tmux`.

## Installing

- Clone repository in your `$HOME/.config` folder:

```sh
git clone --depth 1 https://github.com/Hdoc1509/tmux-config ~/.config/tmux
```

- Clone the [tmux-tomorrow](https://github.com/edouard-lopez/tmux-tomorrow) theme in `$HOME/.tmux/themes` folder:

```sh
git clone https://github.com/edouard-lopez/tmux-tomorrow.git ~/.tmux/themes
```

- Source the `~/.config/tmux/tmux.conf` file from your `~/.tmux.conf` file:

```tmux
source-file ~/.config/tmux/tmux.conf
```

- Or create a symlink from `~/.tmux.conf` to `~/.config/tmux/tmux.conf` file:

```sh
ln -s ~/.config/tmux/tmux.conf ~/.tmux.conf
```

## Key bindings

The default prefix is `Ctrl-Space`.

This config just overrides the following default key bindings:

- `Prefix-L`: Switch to the las client
- `Prefix-l`: Select the previously current window
- `Prefix-r`: Redraw the current client
- `v` (copy-mode-vi): Rectangle toggle

| Key binding          | Mode         | Command                      |
| -------------------- | ------------ | ---------------------------- |
| `Prefix-h` / `Alt-h` | Normal       | Select left pane             |
| `Prefix-j` / `Alt-j` | Normal       | Select below pane            |
| `Prefix-k` / `Alt-k` | Normal       | Select above pane            |
| `Prefix-l` / `Alt-l` | Normal       | Select right pane            |
| `Prefix-H`           | Normal       | Resize the pane left by 5    |
| `Prefix-J`           | Normal       | Resize the pane down by 5    |
| `Prefix-K`           | Normal       | Resize the pane up by 5      |
| `Prefix-L`           | Normal       | Resize the pane right by 5   |
| `Prefix-S`           | Normal       | Split window vertically      |
| `Prefix-V`           | Normal       | Split window horizontally    |
| `Prefix-r`           | Normal       | Reload `~/.tmux.conf` file   |
| `Ctrl-Alt-c`         | Normal       | Enter copy mode              |
| `Prefix-P`           | Normal       | Paste the most recent buffer |
| `v`                  | Copy-mode-vi | Begin selection              |
| `y`                  | Copy-mode-vi | Copy selection               |
