# Motivations
Unlike the iPod Classics, the iPod Mini did not received the same love by themes developers and most themes that I could find were pretty far from my expectations and my needs. I found only 2 themes (Sprocket and Minim) that were very interesting and good looking, and started to use them regularly. I learnt how to modify Rockbox themes (using this excellent tutorial : https://www.rockbox.org/wiki/CustomWPS and also by looking how these 2 themes were made by reading their code).

The idea started essentially about just fixing some bugs and adding very small improvements but the project grew up over time and now both themes are greatly improved esthetically and ergonomically. I did not made those themes from scratch and my work could not exist without the Rockbox project and without the work of those themes developers who made a solid base to work with.

I think this work may benefit to the community, so I share it in the hope that this will be useful to someone in the vast Internet.

# Minim b4 by yuuiko
Improvements made by me : 
- Use the font "Sazanami Mincho 11px" by default in menus (to show more content on screen without having to scroll)
- Important layout improvements on WPS : 
	- Added the playlist state (current/total)
	- Reduced slightly the surface of album cover to show one more line of text
	- Use Sazanami Mincho 11px to show a 3rd line of text content
	- Add another line that show info about the Next song in the playlist
	- Text is now scrolling even if the song is not playing
	- When changing the volume, the audio format is now shown on a different line
	- After changing the volume, the WPS return instantly to normal state. There's no need anymore to show different info during a few seconds (which was in my opinion not a very practical user experience design choice because those info should be accessible just by an eye-sight without any user interaction)
	- Show track year ID3 at the end of the second line if the info is available
	- Show current clock and battery percentage in 3rd line (bottom-right), as alternating text
	- Show sleep timer if available in 3rd text line (bottom-right) and show a short description of each info before showing it (during 1.5 seconds)

Bug fixes made by me : 
- Fixed a missing space between the Month name and the day of month in the lockscreen when music is playing (there is 2 different lockscreen, one that show if music is playing and another that show when there's no music to play. On the second one, there was nothing to fix, it was correct.)
- Fix to the glitchy lockscreen each time a new song is played in the background while staying on the lockscreen (I inspired myself from the code of this theme https://github.com/D0-0K/adwaitapod to figure out how to fix it).
- Fix multiple issues that could cause the lockscreen to glitch out
- The lock icon was not showing up on WPS if no album cover is present or if album cover is disabled, it's now fixed

This theme already supports japanese characters just fine out of the box.
With all of my work, you lose 5 pixels that were previously showing the cover art in WPS but you get a precious 3rd line using a smaller font. It's less minimal than the work and the vision of yuuiko, but in my opinion it is much more usable because you now get access to every important data directly on your WPS just by looking into your screen a few seconds without having to touch to anything. Minim is now competiting in terms of usability against a very complete and simple looking theme like Sprocket in my opinion, while still looking and feeling much more "Minimal" and esthetic than any other available Rockbox themes available for the iPod Mini.

I also decided purposely to not touch the lockscreen (when you HOLD from the home screen) because it is supposed to look nice but not supposed to replace the real WPS, so don't ask me to add more data on this space. I like how the cover art is taking all space here with only current hour + date with a big font.

Please support the designer/theme creator here by donating on his patreon : https://www.patreon.com/yuuiko

# Sprocket by gogi-goji
Improvements made by me : 
- Add important fonts in the package
- Use the font "Rockbox-Mix" on the WPS to support japanese characters
- Use the font "11-Sazanami-Mincho" in menus to print more lines and support japanese characters everywhere
- Only in menus (not in WPS), the title of the list is now shown in the status bar rather than the current volume icon + text. This means that all content lists will show one more line of content. The size of an iPod Mini screen is so small, so each line shown on screen is precious and helps at navigation within a large music library. Having the list title in the status bar creates also a clear visual separation between the title and the content which increases readability and comfort.
- Enable scrollbar on the right of the screen
- If no sleep timer is configured, the current clock (hour + minutes) will be shown on the bottom-center of the WPS so you can know what time is it just by looking your screen at any time without having to fiddle in menus
- This theme can now show album arts ! It's fully conditional, so you still get full screen texts if you disabled album arts globally or if your current track does not have any available one.
- The play status (Play/Stop icon) is now showed on the status bar outside the WPS (so in menus) only when the lock icon is shown, to let more space to show more characters of the current title label during navigation in the menus and in the file/database browser.
- The battery percentage text "100%" is now replaced by "F" to indicate you that your iPod is now fully charged. This saves some space and allowed to reduce the size of the text area, which will be used by the title of the current view (list) in the status bar if it is long enough.

Bug fixes made by me : 
- Clear any previous wallpaper when applying the theme

Link to the original theme : https://github.com/gogi-goji/sprocket-rockbox-theme and https://themes.rockbox.org/index.php?themeid=1820&target=ipodmini2g

Licence : https://creativecommons.org/licenses/by-sa/3.0/deed.fr

# Sprocket or Minim ?
Sprocket is simple and clean.

Minim is gorgeous especially if you have album covers for most or all of your songs. Using a script like this one works great at building optimized covers that the Mini will not struggle to show : https://github.com/Olsro/rockbox_scripts/blob/master/album_art_fix.py
Minim even has a lockscreen if you lock your iPod while being in the homescreen, and that lockscreen is showing the current date and time which can be very useful.

Minim received many improvements to improve usability. I recommend you to try both and do your tests. At first, I found Sprocket more desirable but I improved Minim to add necessary info on the WPS and fix all the flaws that bothered me on it during daily usage. So now, I prefer Minim. But both are usable and good. Disabling cover arts on both themes seems to improve navigation performance in certain cases and to reduce overall disk accesses. If you need the best battery possible life on WPS, disabling completely cover arts is probably what you will want to do.

# Screenshots
## Minim
![Alt text](MINIM%20b4%20-%20Mini/screenshots/1.png?raw=true "WPS")
![Alt text](MINIM%20b4%20-%20Mini/screenshots/2.png?raw=true "Home")

## Sprocket
![Alt text](Sprocket/screenshots/1.png?raw=true "Home")
![Alt text](Sprocket/screenshots/2.png?raw=true "WPS")
![Alt text](Sprocket/screenshots/3.png?raw=true "WPS with cover art")