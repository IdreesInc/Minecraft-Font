# Minecraft Font

***Notice: This project is not affiliated with Minecraft or Mojang in any way and is exclusively a fan project. This font emulates the typeface of the font used in the Minecraft UI, but it does not include any assets or font files from the original game.***

## About this font

This is an OpenType font containing 195 glyphs carefully designed to look exactly like the characters in Minecraft. The font contains all the visible UTF-8 characters between U+0000 to U+00FF, which includes most Latin glyphs you'd use on a daily basis. I've also added a few extra glyphs like `☺` which are commonly used in the game.

What makes this different from other attempts at emulating the Minecraft bitmap font is that it takes into careful consideration how converting from a bitmap font to an OpenType font can affect metrics such as kerning, intended weight, and line height. Through a lot of experimenting, I've selected bounding metrics that best match the original look when rendered as a modern font.

Regular Weight             |  **Bold Weight**
:-------------------------:|:-------------------------:
| ![](images/glyphset.png) | ![](images/glyphset-bold.png) |

I've also added a bold version of each character that was designed with the same algorithm that Minecraft uses for bolding glyphs. Instead of just increasing the stroke weight like with a normal font, each character becomes thicker by shifting the pixels one pixel to the right and printing them overtop the original design. The end result is completely game-accurate and only mostly unreadable!

If you like this font but think that it would look better monospaced and with unnecessary ligatures, check out [Minecraft Mono](https://github.com/IdreesInc/Minecraft-Mono)!

## How to install

### Windows

Download the most recent `Minecraft.otf` and `Minecraft-Bold.otf` files from the [Releases](https://github.com/IdreesInc/Minecraft-Font/releases) page. Right click on the downloaded font files and select **Install**. You might need administrative access to install fonts, depending on your machine.

### Mac

Download the most recent `Minecraft.otf` and `Minecraft-Bold.otf` files from the [Releases](https://github.com/IdreesInc/Minecraft-Font/releases) page. Double click on the downloaded font files and select **Install Font** in the window that appears. More help available [here](https://support.apple.com/en-us/HT201749).

## How to use

After following the installation instructions up above, simply select the "Minecraft" font in any application that supports custom fonts. You might need to restart the application or your computer for the font to appear.

## FAQ

### How were these characters generated?

The font was originally drafted by hand using [bitfontmaker2](https://www.pentacom.jp/pentacom/bitfontmaker2/). The set was then exported using their built in bitmap to TTF converter, and from there the resultant .ttf files were cleaned up and updated in [FontForge](https://fontforge.org/en-US/). Every subsequent character addition should be done using FontForge, though bitfontmaker2 is still a good tool for drafting up designs.

### Why doesn't this font contain more characters?

Each of these glyphs had to be copied over by hand as well as their bold equivalents, which takes time. The font contains most of the common latin characters you might use, with a goal of containing all of the visible UTF-8 characters between U+0000 to U+00FF. If you have a specific glyph that you would like added to the font, you are free to create an issue, though I make no promises that I will have the time to add it. In the future, someone smarter than me might make a script to directly convert the bitmap fonts stored as sprite sheets in Minecraft into modern vector fonts.

### Is there a monospaced version?

Absolutely, check out [Minecraft Mono](https://github.com/IdreesInc/Minecraft-Mono) for a monospaced version with updated glyphs and ligatures.
