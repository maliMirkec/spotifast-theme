# Cita themes for Spotifast

Cita light and dark themes for Spotifast, the native Spotify client for macOS.

## Files

- `cita-light.json`
- `cita-dark.json`

## Install

Copy the files to the Spotifast themes folder:

```sh
mkdir -p ~/Library/Application\ Support/me.paolino.spotifast/themes
cp cita-*.json ~/Library/Application\ Support/me.paolino.spotifast/themes/
```

If Spotifast is open, reload the themes:

```sh
spotifast reload-themes
```

You can also use the Open themes folder button in Settings.

## Apply

Open Settings → Appearance → Theme and pick `cita-dark` or `cita-light`.

To switch with the system, pick Follow system. Then set Light mode theme to `cita-light` and Dark mode theme to `cita-dark`.

## Format

Each theme is a JSON file with two keys:

- `base`, `dark` or `light`
- `colors`, a map of hex colors

An unknown key makes the file invalid. Spotifast skips it and logs a warning. The app shows the file name without `.json` as the theme name.

## Where the colors come from

The colors match the Marta, Herdr, and Crest themes in this folder.

| Spotifast | Light | Dark |
| --- | --- | --- |
| `window` | `#ffffff` | `#011d3b` |
| `panel` | `#f3f7fb` | `#011830` |
| `surface` | `#e8eff6` | `#02264d` |
| `surface_hover` | `#c4f5e9` | `#1a535e` |
| `surface_active` | `#9bf7da` | `#0f6652` |
| `outline` | `#d6e1ec` | `#0a3a6b` |
| `text` | `#043a73` | `#e6f0fa` |
| `secondary` | `#4f6a8c` | `#9db4d3` |
| `dim` | `#7f93ad` | `#5f7fa8` |
| `accent` | `#08805a` | `#63f2c5` |
| `accent_hover` | `#06664a` | `#9bf7da` |
| `on_accent` | `#ffffff` | `#011d3b` |
| `danger` | `#d1124a` | `#ff5c85` |
| `warning` | `#a86a00` | `#ffd27a` |
| `tint` | `#08805a26` | `#63f2c533` |

`tint` is the color a page fades from when there is no album art. Its alpha sets the strength.
