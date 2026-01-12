# tf2-linux-fonts

In late 2024, TF2 decided to remove the Noto Sans CJK and emoji fonts it provided,
breaking everything that uses extended Unicode in the process.

While the CJK fonts were later fixed by using the system copy of Noto Sans CJK,
if installed. 

However the emoji fonts still are missing as of writing, and
some Unicode glyphs do not have proper coverage by the fonts
used by the game.

A mitigation for this is to override the copy of the game's Noto Sans Thai.

## Installation.

1. Go to your Team Fortress 2 installation.

2. Go back a directory to where `tf_linux64` is located.

3. Forward to `platform/resources/linux_fonts`

4. Replace `notosansthai.ttf` with a selected font.

5. Launch your game.

## Variants.

| Font           | License               | Coverage  |             |                      |                  |
|----------------|-----------------------|-----------|-------------|----------------------|------------------|
|                |                       | Overall   | Lenny Faces | Geometric Shapes [1] | Misc. Glyphs [2] |
| UnifontEX      | GPLv2                 | Excellent | Perfect     | Perfect              | Good             |
| BabelStone Han | Arphic Public License | Good      | Good        | Good                 | OK               |
| Sun-Ext-A      | Freeware              | Good      | OK          | Good                 | OK               |
| Go Noto        | Unlicense             | OK        | Mediocre    | OK                   | Mediocre         |

[1] Geometric Shapes include: `○●▰▱■□`

[2] Misc. glyphs are used mainly on community servers and gamemodes, for example: Zombie Riot and Mann in the Machine

[3] OK/Mediocre coverage means that you may see a large amount
of missing glyphs in some scenarios

## Why multiple variants?

While UnifontEX provides the highest possible amount of
glyphs that a single font file can have, it is also the
most visually ugly, being based upon a pixel font.