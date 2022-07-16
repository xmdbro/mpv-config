# README

- Quickly skim through [mpv.conf](https://github.com/xmdbro/mpv-config/blob/main/portable_config/mpv.conf) to make sure it plays back just fine. Otherwise you may have problems.
- Make sure to run [mpv-install.bat](https://github.com/xmdbro/mpv-config/blob/main/installer/mpv-install.bat).
- Running [updater.bat](https://github.com/xmdbro/mpv-config/blob/main/installer/updater.bat) is optional.

# Keybinds

#### General
- <kbd>l</kbd> - Toggle loop
- <kbd>d</kbd> - deband toggle
- <kbd>h</kbd> - deinterlace toggle
- <kbd>UP/DOWN/LEFT/RIGHT</kbd> - Seek 85 seconds forward/backward and 5 seconds forward/backwards respectively.
- <kbd>F9</kbd> - Display the entire playlist
- <kbd>F10</kbd> - Display all video, audio, and subtitle tracks
- <kbd>F11</kbd> - Show the list of chapters (Name, current chapter, and timestamp)
- <kbd>PAUSE</kbd> - stop playback (quit or enter idle mode)
- <kbd>CTRL+r</kbd> - Rotate the video

#### Subtitles
- <kbd>Ctrl+V</kbd> - decrease the subtitle font size by 0.1
- <kbd>CTRL+v</kbd> - increase the substitle font size by 0.1
- <kbd>j</kbd> - switch subtitle track forwards
- <kbd>J</kbd> - switch subtitle track backwards

#### Audio
- <kbd>Scroll_UP</kbd> - increase volume by two
- <kbd>Scroll_DOWN</kbd> - decrease volume by two
- <kbd>CTRL+UP</kbd> - increase volume by five
- <kbd>CTRL+DOWN</kbd> - decrease volume by five

# Scripts
- [audio-osc.lua](https://github.com/mpv-player/mpv/issues/3500#issuecomment-305646994)
  - keeps OSC open when loading an audio file. Auto otherwise.
- [auto-profiles.lua](https://github.com/Moodkiller/MPV-Made-Easy/blob/master/scripts/auto-profiles.lua)
  - Automatically apply profiles based on runtime conditions.
- [autoload.lua](https://github.com/mpv-player/mpv/blob/master/TOOLS/lua/autoload.lua)
  - Automatically loads playlist entries before and after the currently opened file.
- [clipshot.lua](https://github.com/ObserverOfTime/mpv-scripts/blob/master/clipshot.lua)
  - <kbd>c</kbd> - Copies screenshot (with subs) to clipboard instead of saving to disk.
- [coverart.lua](https://github.com/CogentRedTester/mpv-coverart/blob/master/coverart.lua)
  - Automatically loads external cover art as a video track
- ~~[lrc-autoload.lua]()~~ **No longer necessary after mpv 0.30.0!**
  - ~~Automatically loads .lrc files if found~~
- [mines.lua](https://github.com/wiiaboo/mpv-scripts/blob/master/mines.lua)
  - What can I say? It's minesweeper.
  - <kbd>CTRL+x</kbd> - Toggle minesweeper.
  - <kbd>UP/DOWN/LEFT/RIGHT</kbd> - Navigate.
  - <kbd>SPACE</kbd> - Open a tile.
  - <kbd>b</kbd> - Flag a tile.
  - <kbd>t</kbd> - Toggle transparency.
  - <kbd>w</kbd> - Cycle between presets.
- [mpv_thumbnail_script.lua](https://github.com/TheAMM/mpv_thumbnail_script)
  - Displays thumbnails when hovering over the seekbar. Thumbnails save to `%TEMP%\mpv_thumbs_cache` by default on Windows.
  - Each iteration of `mpv_thumbnail_script_server.lua` will assign more threads to generating thumbnails. Depending on your CPU, you might have to lower it by one or increase it by a few.
- [mpv-drpc.lua](https://github.com/noaione/mpv-discordRPC)
  - Discord RPC Integration for mpv.
- [mpv-gif.lua](https://github.com/the-honey/mpv-gif-generator/blob/master/mpv-gif.lua)
  - Create animated GIFs using mpv. Requires ffmpeg. Saves to `%USERPROFILE%\Desktop`.
  - Check [gif.conf](https://github.com/xmdbro/mpv-config/blob/main/portable_config/script-opts/gif.conf) if you would like to modify dir/res/fps.
  - <kbd>g/G</kbd> - Set stard and end time respectively.
  - <kbd>CTRL+g/G</kbd> - Export GIF and export GIF with subtitles respectively.
- [ontop-playback.lua](https://github.com/mpv-player/mpv/blob/master/TOOLS/lua/ontop-playback.lua)
  - Disabled ontop when pausing and re-enables again when resuming playback. Note that this won't do anything if ontop wasn't enabled to begin with.
- [open-file-dialog.lua](https://github.com/rossy/mpv-open-file-dialog/blob/master/open-file-dialog.lua)
  - <kbd>CTRL+O</kbd> - Launches a regular Windows open file dialog.
- [playlistmanager.lua](https://github.com/jonniek/mpv-playlistmanager/blob/master/playlistmanager.lua)
  - Allows you to see and interact with your playlist in an intuitive way.
  - All keybinds are documented [here.](https://github.com/jonniek/mpv-playlistmanager#keybinds)
- [seek-to.lua](https://github.com/occivink/mpv-scripts/blob/master/scripts/seek-to.lua)
  - <kbd>~</kbd> - Seek to an absolute position in the video by typing it's timestamp. Use left and right for navigation and once typed out, press `Enter` to seek to position. `UP` and `DOWN` to navigate previously navigated timestamps.
- [show-stream-title.lua](https://github.com/blue-sky-r/mpv/blob/master/scripts/show-stream-title.lua)
  - Show OSD stream title from playlist on change.
- [trackselect.lua](https://github.com/po5/trackselect/blob/master/trackselect.lua)
  - Automatically select your preferred tracks based on title, because --slang isn't smart enough.
- [visualizer.lua](https://github.com/mfcc64/mpv-scripts/blob/master/visualizer.lua)
  - <kbd>c</kbd> Cycle through various audio visualizations.
- [webm.lua](https://github.com/ekisu/mpv-webm)
  - <kbd>W</kbd>Create WebMs using mpv. 
  - Configure to your desires [here](https://github.com/xmdbro/mpv-config/blob/main/portable_config/script-opts/webm.conf)

# Shaders
