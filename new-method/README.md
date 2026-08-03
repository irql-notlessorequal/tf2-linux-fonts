# The Newer Method

> [!CAUTION]
> This method requires a Custom HUD or at least a minimal setup of the default HUD.
>
> Do NOT change the game's HUD files in the VPKs!

## Instructions

1. Go to `platform` in the base directory and open `platform_misc_dir.vpk` with a VPK
tool of your choice.

2. Extract `resource/sourceschemebase.res` somewhere and keep it handy.

   If your HUD already provides this file, you may skip this step.

3. Copy the provided `resource/linux_fonts` folder in the repository to your custom HUD's `resource` folder.

4. If your HUD doesn't contain a `sourceschemebase.res` in it's `resource` folder, then copy it over.

5. Open `sourceschemebase.res` and scroll down to `CustomFontFiles` section.

6. Find two free slots (numbers) that are available between all of the following files.

    - `sourceschemebase.res`
    - `sourcescheme.res`
    - `clientscheme.res`

7. Place the following at the end of the list, don't forget to change the numbers from the ones here.

```
		"12"		"resource/linux_fonts/notosansthai.ttf"
		"13"		"resource/linux_fonts/notocoloremoji.ttf"
```

8. Apply this change to the other listed files.

9. If everything went right, you should see emojis working again!

> [!WARNING]
> You may have to remove the copy of `notosansthai.ttf` in `platform/resources/linux_fonts`,
> I haven't verified the loading order of it yet.
>
> See the `old-method` for more details.

## Notice to HUD creators

This method uses `Code2000` as the Unicode font which is treated as a "Shareware Demo",
you may want to consider a different font, you can use fonts from the `old-method` as they
are interchangeable.

Also if fonts aren't loading, try renaming the file to lower case...thanks Valve.