# tf2-linux-fonts

In early 2025, TF2 decided to remove the Noto Sans CJK and emoji fonts it provided,
breaking everything that uses extended Unicode in the process.

While the CJK fonts were later fixed by using the system copy of Noto Sans CJK,
if installed. 

However the emoji fonts still are missing as of writing, and
some Unicode glyphs do not have proper coverage by the fonts
used by the game.

## Fixing This

There are two ways to fix this.

### Partially

You can use the `old-method` to override a single font file in the game,
giving the game more glyph coverage.

### Fully

The `new-method` takes the work found in https://github.com/ValveSoftware/Source-1-Games/issues/7026
and gets a much wider coverage of Unicode glyphs and Emojis working again.

However this requires modifying your HUD, unlike the old method.