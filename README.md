# Tahoma For Telegram

This repository is a temporary quick fix for incorrect font displaying on Telegram Desktop v4.6.0 for Windows.  

The issue is probably caused by Qt 6's font fallback logic as it tries to pick  
the first font in alphabetical order that has a glyph for the character to display.  

Simply installing all fonts included in this repository will temporarily fix the incorrect font displaying issue.  

(You will need to restart Telegram Desktop app after install the fonts.)

## What exactly does this do?

After you install all fonts included in this repository,  
They will be the first fonts to be picked by Qt 6's font fallback logic.  

## How does it work?

I added a "Start of Heading" (U+0001) character at the begining of the font name.  
I found that this character will always be the first one to be found when it tries to look in alphabetical order.  

## How did you make this?

I used the software called "Typograf" to rename the fonts.  

## How to uninstall this?

Just search for "Tahoma For Telegram" in Windows's Font Settings and simply uninstall/delete them.  

## Reference

Issue Reference: https://github.com/telegramdesktop/tdesktop/issues/25825
