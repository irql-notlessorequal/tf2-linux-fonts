# Old-ish Method

This method overrides the main copy of Noto Sans Thai, one of the hardcoded
fallback fonts within the current builds of Source Engine.

Of course, Noto Sans Thai doesn't provide the glyphs we need so we take a different
font and modify it using a tool like FontForge to masquerade as Noto Sans Thai instead.

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
most visually ugly, being based upon a bitmap/pixel font.