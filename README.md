# Singing Stream Savior

Singing Stream Savior is a Windows desktop tool for singing streams. It brings
your song library, BGM, karaoke playback, queue, lyrics, audio processing, and
OBS output into one workflow.

## Download

Download the latest full installation ZIP from the official
[Singing Stream Savior 2.1.8.1 release](https://github.com/NoonIsAwesome/Singing-Stream-Savior-Updates/releases/tag/v2.1.8.1).
The ZIP includes launcher **1.2.1.2** and runtime **1.0.0.10**.
Extract the complete ZIP to a normal folder, then open `Singing Stream Savior.exe`
in the outermost folder.

The same full ZIP is available from the [Cloudflare R2 download](https://updates.noonisawesome.dev/releases/v2.1.8.1/Singing.Stream.Savior.2.1.8.1.zip).
Launcher 1.2.1.2 improves interrupted update recovery and shows copyable error details when startup cannot complete.
For setup instructions and the complete feature guide, visit the
[Singing Stream Savior Manual](https://noonisawesome.dev/).

## 2.1.8.1 update

Fix update recovery and improve startup feedback, UI, and YouTube search.

1. Launcher 1.2.1.2 improves interrupted update recovery for transient file locks and read-only backups. Launch failures show copyable error details and preserve backups.
2. Use three-dot startup and project-loading feedback with a uniform preparation background and no Cancel button. Prepare initial font caches and initialize resource monitoring in the background to reduce UI blocking.
3. Improve light-mode playing-song text, playback markers, and the YouTube download icon contrast.
4. Close Song Settings after lyrics or cover art is successfully attached. Keep it open on cancellation or failure, and preserve prompts for unsaved changes in other tabs.
5. Prevent mouse clicks from leaving focus borders on lyrics, song information, and YouTube preview buttons while retaining keyboard operation.
6. Instrumental search prioritizes multilingual keywords from the query, keeps explicit qualifiers, and expands when results are insufficient.
7. Original searches prefer YouTube Music songs, falling back to YouTube when more results are needed or the service fails.
8. Replace the expansion explanation beside YouTube filters with tooltips.
9. Remove the appearance button border in the project chooser and main window.
10. Add Metal and Blues to preset genres.
11. Enlarge song search suggestion text and row height for easier selection.

## 2.1.8.0 update

**An awesome update (probably), at least I think it's awesome (⁎⁍̴̛ᴗ⁍̴̛⁎)**

1. Song metadata: assign multiple singers / performers, reuse names saved in the project, and optionally write tags to local audio files.
2. Classification and search: new genre and language tags; search songs, performers, genres and languages, with keyword suggestions.
3. Song settings: information, album artwork and lyrics are combined in three tabs. Their individual status icons remain visible, and source icons distinguish local files from YouTube links.
4. New YouTube search page: search YouTube songs or backing tracks directly in the app, then add them to the song list or UVR queue. Adding to UVR only queues the item; start vocal removal from the UVR page.
5. Appearance: switch between Dark, Light and Follow Windows. Dark is the default; the Full window now defaults to 1600×900.
6. Removed the traditional song-list view because I think cards look better and are easier to use.
7. Slightly improved application startup time.
8. Sneaking in a random sentence. I wonder if anyone will notice.

## 2.1.7.4 update

Improve the lyrics window, settings controls and ASIO error diagnostics.

1. Redesign the lyrics window with a black and blue interface, consistent controls and easy-to-click minus/plus buttons for text size and timing offset.
2. Use a wider and taller default lyrics window and remember its size after closing and reopening.
3. Make playback following a clear toggle button. Turning it off stops highlighting and automatic scrolling; timing adjustments immediately update the current lyric.
4. Widen the lyrics settings panel, add scroll gutters and collapsible sections, and keep field and button heights consistent.
5. Scrolling over closed dropdowns, numeric fields or sliders scrolls the settings panel without changing parameters. Open dropdown lists retain normal scrolling.
6. Add ASIO inspection and startup diagnostics: failure stage, original API error codes, requested rate and buffer, timeout and helper exit. Export safe technical details through Help > Export diagnostic data; vendor messages remain local.
7. Fix ASIO inspection rejecting valid drivers with negative version identifiers, including the reported Scarlett 2i2 4th Gen data. Channel, sample rate and buffer validation remain in place.
8. Correct the microphone-to-Stream software estimate for the active Formal path, including its queue and sample-rate conversion waiting without adding the inactive capture FIFO again.
9. Add audio timing diagnostics for Formal queue depth, publication residence, Profile processing and source age, output service gaps, compensation and first faults. These are software observations, not physical latency measurements.

## 2.1.7.3 update

Improve dynamic lyrics readability and update downloads.

1. Add a shared text outline toggle, color and width for 13 dynamic lyrics designs. Preview and OBS use the same settings; Basic Lyrics and Classic Karaoke remain unchanged.
2. Outline settings stay with the project and are kept when switching designs. Small reading text uses a finer outline; existing projects keep outlines off by default.
3. Before downloading, compare GitHub and Cloudflare R2 using a short, bounded sample; keep the selected source for subsequent update files and fall back if it fails.
4. Launcher 1.2.1.0 is reissued with improved source selection. “Skip update and open app” cancels safely and starts the installed version; you can update next time. The app detects same-version launcher replacements by SHA-256.

## 2.1.7.2 update

Add three dynamic lyrics designs and four customizable playlist themes.

1. Lyrics search tries Traditional/Simplified Chinese name variants in the background, cleans video titles, retries temporary service failures once and ranks version matches. Confirm a result before attaching it.
2. Iris Stage, Echo Rig and Shard Stage follow the shared playback clock, with mask reveals, outline echoes and vertical slices. Choose off, gentle or full motion; hide outer decorations independently. Iris Stage starts without its outer ring.
3. Bubble Notes defaults to Comic Outline. Choose Thought Cloud, Folded Note, Rounded Droplet or Double Line. Place the stack left/right and top/bottom; the top stack puts Set List above the current song.
4. Corner Duet groups a larger current song with one rotating history row. Place it left or right, without Now Playing or Set List headings.
5. Quiet Frame provides optional Next On / Reserve in a compact right column, with paging for longer queues. Quiet Verse places a prominent current song above six text-only rows, aligned left, center or right.
6. All four new themes support theme colors, fonts, optional Index and history timestamps. Metadata stays fixed, disabled fields collapse and long song titles scroll within the available space.

## 2.1.7.1 hotfix

Fix a startup error after upgrading when older vocal Profile data remains on the computer. Preserve original saved data and custom effect parameters, bypass settings, and VST plug-in state.

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
  [Read the lyrics editor guide](https://noonisawesome.dev/en/guide.html#lyrics-editor).
- **Guide vocal monitoring:** Keep the Vocal track when separating audio in
  UVR and import the accompaniment to link both tracks. Guide vocals follow
  key, speed, seeking, and loops, with independent level control in Meter.
  They are heard only through monitoring and never enter the OBS mix.
  [Read the UVR guide](https://noonisawesome.dev/en/guide.html#uvr-vocal-removal).
- **Dynamic synchronized lyrics:** Search or import lyrics, then choose from
  twelve animated styles: Kinetic Type, Prism Cut, Lumen Drift, Ink Cascade,
  Silk Script, Verse Stack, Glyph Motion, Letter Spread, Stagger Signal,
  Iris Stage, Echo Rig, and Shard Stage.
  Each style card includes an animation preview. Word effects follow the
  timing in the lyrics file; when complete word timings are unavailable,
  timing is estimated and may not fully match the singing. The main preview
  and OBS share the display settings; the independent Lyrics window keeps its
  own reading settings. Japanese and Korean romanization in the OBS output is
  supported by **Basic Lyrics**.
  [Read the lyrics guide](https://noonisawesome.dev/en/guide.html#feature-lyrics).
- **Playlist Appearance with live preview:** Preview Now Singing, Set List,
  Next On, and Reserve while choosing a theme. Theme cards preview their
  motion. Oblique Stream adds a minimal transparent layout with left or right
  placement, Now Playing above or below, timestamps, and curved scrolling.
  Bubble Notes, Corner Duet, Quiet Frame, and Quiet Verse add adjustable
  colors and fonts, with optional Index and history timestamps.
  In themes that support numbering, the numbering button cycles through Off,
  1., 01, and ．. Edit the playlist position and proportional size on the
  fixed 1920 x 1080 canvas; an existing OBS source using that output updates
  while you drag. [Read the preview and OBS guide](https://noonisawesome.dev/en/guide.html#feature-preview).
- **Improved YouTube downloads:** The default format is MP3 at 320 kbps, with
  MP3 and WAV available. **Download all YouTube files** processes the current
  project song list, not the entire global library. Downloaded audio can be
  converted locally while the original is preserved and same-name files are
  not overwritten. Successful songs link to the local audio files even when
  another song fails; failed songs are listed after the batch finishes.
  Right-click the button beside the song statistics row to choose a format,
  open download settings, or open the download folder. [Read the download guide](https://noonisawesome.dev/en/guide.html#feature-download).
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
