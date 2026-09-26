# Singing Stream Savior

Singing Stream Savior is a Windows desktop tool for singing streams. It brings
your song library, BGM, karaoke playback, queue, lyrics, audio processing, and
OBS output into one workflow.

## Download

Download the latest full installation ZIP from the official
[Singing Stream Savior 2.1.7.0 release](https://github.com/NoonIsAwesome/Singing-Stream-Savior-Updates/releases/tag/v2.1.7.0).
The ZIP includes launcher **1.2.0.8** and runtime **1.0.0.8**. Extract the
complete ZIP to a normal folder, then open `Singing Stream Savior.exe` in the
outermost folder.

For setup instructions and the complete feature guide, visit the
[Singing Stream Savior Manual](https://noonisawesome.github.io/Singing-Stream-Savior-Manual/).

## 2.1.7.0 update

1. Import and export vocal Profiles to share or move your effects settings.
2. Import OBS audio effects, with support for Gain, Noise Gate, Compressor, and Limiter.
3. Back up and restore application settings, Profiles, the song library, selected projects, and related audio, lyrics, and artwork. Identical audio files are stored only once.
4. Improve the responsiveness of Profile loading and saving.
5. Improve YouTube batch downloads: a failed song no longer affects the others. Successful songs link to local audio files, and failed songs are listed when the batch finishes.
6. Improve MP3/WAV conversion and playback afterward. The progress window now shows which song is being processed.
7. Improve YouTube playback-range editing for some videos that can play but cannot be downloaded. Fix cases where playback had to start before a range could be adjusted.
8. Add a missing-audio indicator to the song list. Click it or use the right-click menu to locate the file while keeping the song's settings.
9. Improve playback stability when switching songs, pausing, and stopping.
10. Long song titles now scroll in one direction and restart from the beginning. Refine several interface details.
11. Stop automatically installing or repairing the OBS connector at startup, reducing unnecessary permission prompts.
12. Happy Mid-Autumn Festival, everyone! ٩(˃̶͈̀௰˂̶͈́)و

## 2.1.6.1 hotfix

1. Fixes an issue in advanced streaming mode where the Microphone Block's level meter on the Audio Routing page could remain still even though the microphone signal was working normally.
2. Fixes issues that prevented downloading audio from YouTube links and converting downloaded files.

## 2.1.5.4 update

Stability update

1. Improves brief BGM dropouts.
2. Improves occasional delayed response when stopping accompaniment.
3. Fixes how Vocal Profiles are applied in player modes.
4. Improves VST3 stability.
5. Fixes an issue where preview could stop unexpectedly or Profile switching could fail after latency adjustments to some VST3 plug-ins.
6. Improves effect preloading performance and fixes an issue where a Profile containing disabled effects could open the wrong effect editor.
7. Fixes an issue where a failed VST3 replacement, removal, or enable operation could still save the wrong selection or checkbox state.
8. Improves project media collection.
9. Improves UVR vocal separation.
10. Improves recording save and finalization.
11. Improves YouTube feature stability.
12. I'm going to see Hans Zimmer in concert today! Can't wait to soak up Guthrie Govan's solos!

## What you can do

- **Lyrics editor:** Create and edit synchronized lyrics with line or word timing. Mark while
  listening with Ctrl + Enter, merge or split words, preview the result, then
  apply it to the selected song.
  [Read the lyrics editor guide](https://noonisawesome.github.io/Singing-Stream-Savior-Manual/en/guide.html#lyrics-editor).
- **Guide vocal monitoring:** Keep the Vocal track when separating audio in
  UVR and import the accompaniment to link both tracks. Guide vocals follow
  key, speed, seeking, and loops, with independent level control in Meter.
  They are heard only through monitoring and never enter the OBS mix.
  [Read the UVR guide](https://noonisawesome.github.io/Singing-Stream-Savior-Manual/en/guide.html#uvr-vocal-removal).
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
  not overwritten. Successful songs link to the local audio files even when
  another song fails; failed songs are listed after the batch finishes.
  Right-click the button beside the song statistics row to choose a format,
  open download settings, or open the download folder. [Read the download guide](https://noonisawesome.github.io/Singing-Stream-Savior-Manual/en/guide.html#feature-download).
- **Stream-ready playback:** Organize songs into playlists, prepare Reserve,
  play local files or YouTube links, and send playlist and lyric overlays to
  OBS with `Drag to OBS`. For YouTube accompaniment, the **YouTube Video**
  window follows playback, pause, seeking, and speed changes and offers
  available captions. **Lyrics Window** and **YouTube Video** icon buttons
  stay in the accompaniment player in every workspace mode.

## Updating

Existing launchers update the inner application. The application can then
verify and replace the outer launcher in the background when needed.

`updates/stable.json` is the stable-channel manifest read by the launcher
through `raw.githubusercontent.com`. It is published only after the GitHub
Release assets have been uploaded and their URLs, sizes, and SHA-256 values
have been checked.

Copyright © 2026 Noon. All rights reserved.
