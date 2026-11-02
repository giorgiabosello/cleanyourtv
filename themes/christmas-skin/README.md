# christmas-skin

The `themes/christmas/` look (a snowy night with Santa's sleigh) plus the Christmas festive skin, which lives in
the launcher of this branch (`christmas-skin`), not in the stock launcher:

- a tree for Wi-Fi/Ethernet (lights on while online, off when the network drops), a bell for Inputs, Santa for Settings
- snow over the first Home of the day
- a Christmas-red focus glow
- a greeting that follows the date: Thanksgiving (4th Thursday of November, en-US only), 8, 25, 26 and 31 December, 1 and 6 January,
  in the launcher's own language where the day exists; other days keep the normal greeting
- it switches itself off after 6 January 2027 (`festival_until`)

## Use it

1. Build and install the launcher from this branch (`launcher/build-and-install.sh`), as in the main README.
2. Push the theme on the day you want it (Thanksgiving, or 8 December in Italy):

```bash
TV_HOST=192.168.1.50 tools/theme.sh themes/christmas-skin
```

On a launcher without the skin the theme still works and shows the diya skin instead of the tree and Santa.
Do not set `greeting` in `config.json`: a fixed greeting beats the ones that follow the date.

Wallpaper: an original CC0 illustration, see `CREDITS.md`. Santa and the tree are Fluent Emoji 3D (MIT), credited in
`launcher/ICONS-LICENSE-FLUENT-EMOJI.txt`.
