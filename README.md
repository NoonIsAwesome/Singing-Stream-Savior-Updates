# Singing Stream Savior

Singing Stream Savior is a Windows desktop tool for singing streams. It brings
your song library, BGM, karaoke playback, queue, lyrics, audio processing, and
OBS output into one workflow.

## Download

Download the latest full installation ZIP from the official
[Singing Stream Savior 2.1.4.3 release](https://github.com/NoonIsAwesome/Singing-Stream-Savior-Updates/releases/tag/v2.1.4.3).
The ZIP includes launcher **1.2.0.7** and runtime **1.0.0.6**. Extract the
complete ZIP to a normal folder, then open `Singing Stream Savior.exe` in the
outermost folder.

For setup instructions and the complete feature guide, visit the
[Singing Stream Savior Manual](https://noonisawesome.github.io/Singing-Stream-Savior-Manual/).

## What you can do

- **Dynamic synchronized lyrics:** Search or import lyrics, then choose from
  nine animated styles: Kinetic Type, Prism Cut, Lumen Drift, Ink Cascade,
  Silk Script, Verse Stack, Glyph Motion, Letter Spread, and Stagger Signal.
  Each style card includes an animation preview. Word effects follow the
  timing in the lyrics file; when complete word timings are unavailable,
  timing is estimated and may not fully match the singing. The main preview
  and OBS share the display settings; the independent Lyrics window keeps its
  own reading settings. Japanese and Korean romanization in the OBS output is
  supported by **Basic Lyrics**.
  [Read the lyrics guide](https://noonisawesome.github.io/Singing-Stream-Savior-Manual/en/guide.html#feature-lyrics).
- **Playlist Appearance with live preview:** Preview Now Singing, Set List,
  Next On, and Reserve while choosing a theme. Theme cards preview their
  motion. Oblique Stream adds a minimal transparent layout with left or right
  placement, Now Playing above or below, timestamps, and curved scrolling.
  In themes that support numbering, the numbering button cycles through Off,
  1., 01, and ．. Edit the playlist position and proportional size on the
  fixed 1920 x 1080 canvas; an existing OBS source using that output updates
  while you drag. [Read the preview and OBS guide](https://noonisawesome.github.io/Singing-Stream-Savior-Manual/en/guide.html#feature-preview).
- **Improved YouTube downloads:** The default format is MP3 at 320 kbps, with
  MP3 and WAV available. **Download all YouTube files** processes the current
  project song list, not the entire global library. Downloaded audio can be
  converted locally while the original is preserved and same-name files are
  not overwritten; project links change only after all operations succeed.
  Right-click the button beside the song statistics row to choose a format,
  open download settings, or open the download folder. [Read the download guide](https://noonisawesome.github.io/Singing-Stream-Savior-Manual/en/guide.html#feature-download).
- **Stream-ready playback:** Organize songs into playlists, prepare Reserve,
  play local files or YouTube links, and send playlist and lyric overlays to
  OBS with `Drag to OBS`. For YouTube accompaniment, the **YouTube Video**
  window follows playback, pause, seeking, and speed changes. Compact mode
  uses monochrome icon buttons for **Lyrics Window** and **YouTube Video** to
  save player space.

## Updating

Existing launchers update the inner application. The application can then
verify and replace the outer launcher in the background when needed.

`updates/stable.json` is the stable-channel manifest read by the launcher
through `raw.githubusercontent.com`. It is published only after the GitHub
Release assets have been uploaded and their URLs, sizes, and SHA-256 values
have been checked.

Copyright © 2026 Noon. All rights reserved.
