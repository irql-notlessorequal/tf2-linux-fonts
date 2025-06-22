# tf2-linux-fonts

In late 2024, TF2 decided to remove the Noto Sans CJK and emoji fonts it provided,
breaking everything that uses extended Unicode in the process.

A mitigation for this is to override the copy of the game's Noto Sans Thai.

## Installation.

1. Go to your Team Fortress 2 installation.

2. Go back a directory to where `tf_linux64` is located.

3. Forward to `platform/resources/linux_fonts`

4. Replace `notosansthai.ttf` with a selected font.

5. Launch your game.

## Variants.

### UnifontEX

Highest coverage a single TTF/OTF file can cover. (nearly 65k)

Ugliest of them all.

Licensed under the GPLv2.

### Sun-Ext-A

Good coverage with around 50 thousand glyphs.

Slightly visually ugly.

Freeware.

### Go Noto (CJK Core)

Less coverage with around 44 thousand glyphs, missing glyphs needed for lenny faces and other minor things.

Licensed under the The Unlicense.