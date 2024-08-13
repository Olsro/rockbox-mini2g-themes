# Motivations
I improved themes I like to use on my iPod Mini 2G to fix bugs and better fit my needs. I did not made those themes from scratch, I am just using them and applying a few improvements/bug fixes to improve my user experience.
I think this work may benefit to the community, so I share it in the hope that this will be useful to someone in the vast Internet.

# Minim b4 by yuuiko
Improvements made by me : 
- Use the font "Sazanami" by default in menus
- Important layout improvements on WPS : 
	- Added the playlist state (current/total)
	- Reduced slightly the surface of album artwork to show one more line
	- Use Sazanami Mincho 11px to show a 3rd line of content
	- Add another line that show info about the Next song in the playlist
	- Text is now scrolling even if the song is not playing
	- When changing the volume, the audio format is now shown on a different line
	- After changing the volume, the WPS return instantly to normal state. There's no need anymore to show different info during a few seconds (which was in my opinion not a very practical user experience design choice because those info should be accessible just by an eye-sight without any user interaction)
	- Show track year ID3 at the end of the second line if the info is available
	- Show current clock and battery percentage in 3rd line (bottom-right), as alternating text
	- Show sleep timer if available in 3rd line (bottom-right) and show a short description of each info before showing it (during 1.5 seconds)

Bug fixes made by me : 
- Fixed a missing space between the Month name and the day of month in the lockscreen when music is playing (there is 2 different lockscreen, one that show if music is playing and another that show when there's no music to play. On the second one, there was nothing to fix, it was correct.)
- Fix to the glitchy lockscreen each time a new song is played in the background while staying on the lockscreen (I inspired myself from the code of this theme https://github.com/D0-0K/adwaitapod to figure out how to fix it).
- Fix multiple issues that could cause the lockscreen to glitch out

This theme already supports japanese characters just fine out of the box.
With all of my work, you lose 5 pixels that were previously showing the cover art in WPS but you get a precious 3rd line using a smaller font. It's less minimal than the work and the vision of yuuiko, but in my opinion it is much more usable because you now get access to every important data directly on your WPS just by looking into your screen a few seconds without having to touch to anything. Minim is now competiting in terms of usability against a very complete and simple looking theme like Sprocket in my opinion, while still looking and feeling much more "Minimal" and esthetic than any other available Rockbox themes available for the iPod Mini.

I also decided purposely to not touch the lockscreen (when you HOLD from the home screen) because it is supposed to look nice but not supposed to replace the real WPS, so don't ask me to add more data on this space. I like how the cover art is taking all space here with only current hour + date with a big font.

Please support the designer/theme creator here by donating on his patreon : https://www.patreon.com/yuuiko

# Sprocket by gogi-goji
Improvements made by me : 
- Add important fonts in the package
- Use the font "Rockbox-Mix" on the WPS to support japanese characters
- Use the font "11-Sazanami-Mincho" in menus to print more lines and support japanese characters everywhere
- Enable scrollbar on the right of the screen
- Use a pointer for selections to enhance readability
- If no sleep timer is configured, the current clock (hour + minutes) will be shown on the bottom-center of the WPS so you can know what time is it just by looking your screen at any time without having to fiddle in menus
- This theme can now show album arts ! It's fully conditional, so you still get full screen texts if you disabled album arts globally or if your current track does not have any available one.

Bug fixes made by me : 
- Clear any previous wallpaper when applying the theme

Link to the original theme : https://github.com/gogi-goji/sprocket-rockbox-theme and https://themes.rockbox.org/index.php?themeid=1820&target=ipodmini2g

Licence : https://creativecommons.org/licenses/by-sa/3.0/deed.fr

# Sprocket or Minim ?
Sprocket is simple and clean.

Minim is gorgeous especially if you have album covers for most or all of your songs. Using a script like this one works great at building optimized covers that the Mini will not struggle to show : https://github.com/Olsro/rockbox_scripts/blob/master/album_art_fix.py
Minim even has a lockscreen if you lock your iPod while being in the homescreen, and that lockscreen is showing the current date and time which can be very useful.

Minim received many improvements to improve usability. I recommend you to try both and do your tests. At first, I found Sprocket more desirable but I improved Minim to add necessary info on the WPS and fix all the flaws that bothered me on it during daily usage. So now, I prefer Minim. But both are usable and good.

# Screenshots
## Minim
![Alt text](MINIM%20b4%20-%20Mini/screenshots/1.png?raw=true "WPS")
![Alt text](MINIM%20b4%20-%20Mini/screenshots/2.png?raw=true "Home")

## Sprocket
![Alt text](Sprocket/screenshots/1.png?raw=true "Home")
![Alt text](Sprocket/screenshots/2.png?raw=true "WPS")
![Alt text](Sprocket/screenshots/3.png?raw=true "WPS with cover art")