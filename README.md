# EazyDeck

**The soundboard for gamers and streamers.** Play sound effects and music to your friends while you talk, in Discord, TeamSpeak, in-game voice chat, OBS or calls. They hear your voice and your sounds together, and you hear them too.

**[Download the latest EazyDeck.exe](../../releases/latest)**: free, for Windows 10 and 11. Run it and the EazyDeck installer opens.

## What it does

- **Sources:** send sounds to Discord, games and more, each with its own volume and mute. Click a source's icon to mute it, or its name to switch between them.
- **Sound slots 1–10:** put any sound in a slot and fire it with **Ctrl+Alt+1** to **Ctrl+Alt+0**, even while you're in a game. Each slot takes its sound's name.
- **Your library, your way:** add files, folders or a .zip. Folders keep their exact names and become categories, subfolders included.
- **Right-click anything:** rename sounds and folders with a nickname, star favourites, pin folders to the top, give a folder a random-sound hotkey, or remove things from the list (with Undo).
- **Clean mic, built in:** AI noise suppression removes typing, fans and breathing; a smart noise gate, low cut, compressor and limiter are all adjustable, with Off/Light/Standard/Strong presets. Using speakers? Echo cancellation stops friends hearing themselves. Your sounds are never touched.
- **Drag sounds between folders:** drag a pad onto any folder in the sidebar to move it there inside EazyDeck (the file on your PC stays put). EazyDeck remembers where it came from, so you can **Move back** any time.
- **A live visualiser** ripples behind whichever sound is playing.
- **Exact levels:** every volume shows its % and dB, and every mic setting shows its value.
- **Search:** press **Ctrl+K** (you can change this in Settings › Hotkeys).
- **Sixteen colour presets:** Volt, Ember, Plasma and Frost, plus gamer presets Toxic, Rage, Legendary, Epic, Rare, Terminal, Ghost, Sakura, Void, Emerald, Sunset and Bronze, all with a fully dark window to match. The playing visualiser and hotkey badges take on whichever preset you pick.
- **Automatic updates:** EazyDeck checks this page for new versions, tells you in the app and in Windows, and updates in one click.

## Getting started

### 1. Install VB-Cable (one time)

EazyDeck sends your sounds and voice to your chat app through a free "virtual cable": a pretend microphone that your chat app listens to.

1. Download **VB-Cable** from [vb-audio.com/Cable](https://vb-audio.com/Cable/).
2. Unzip it, right-click **VBCABLE_Setup_x64.exe** and choose **Run as administrator**, then click **Install Driver**.
3. Restart your PC if it asks.

### 2. Install EazyDeck

1. Download **EazyDeck.exe** from [Releases](../../releases/latest) and double-click it.
2. Windows may show **"Windows protected your PC"** the first time, because EazyDeck isn't code-signed yet. Click **More info › Run anyway**. Updates after that don't show the warning.
3. The installer opens. Click **Install EazyDeck**. It installs to your own user folder (no admin prompt), adds Start menu and desktop shortcuts, and appears in Windows' **Installed apps**. Prefer not to install? Click **Run without installing**.
4. If EazyDeck is already installed, the installer offers **Update** (or **Repair**), **Open EazyDeck** and **Uninstall** instead.
5. The first time EazyDeck opens, a short setup asks which app you use, your colour, and your microphone and headset.

To remove it later: **Settings › Apps › Installed apps › EazyDeck › Uninstall**. You can keep your settings for next time, and your sound files are never touched.

### 3. Point your chat app at the cable

This is the only setting you change outside EazyDeck. Set your chat app's **microphone** to **CABLE Output (VB-Audio Virtual Cable)**. EazyDeck mixes your real mic in, so friends still hear you.

| App | Where to change it |
|---|---|
| **Discord** | User Settings (cog, bottom left) › Voice & Video › Input Device: **Default** (EazyDeck switches Windows to the cable while it runs; if you've turned that off, choose CABLE Output). Then turn **Echo Cancellation off**, set **Noise Suppression to None** and turn **Automatic Gain Control off**. EazyDeck already cleans your mic (run the auto-optimise for the best result), and Discord's noise suppression would treat your sounds as noise and cut into them. Echo cancellation also cuts your sounds out, and automatic gain control turns quiet sounds back up, undoing EazyDeck's volume sliders. |
| **TeamSpeak** | Settings › Capture (TS3: Tools › Options › Capture). With push-to-talk, sounds only go out while you hold the key. |
| **In-game voice** | The game's Audio or Voice Chat settings › microphone. If there's no option, set CABLE Output as the default recording device in Windows Sound settings. |
| **OBS / Streamlabs** | Add an Audio Input Capture set to CABLE Output, and mute your separate mic source. |
| **Zoom, Teams, Meet** | Audio settings › Microphone. In Zoom, turn on "Original sound for musicians". |

EazyDeck shows the same steps for your app during setup and in **Settings › Help & tour**.

### 4. Add your sounds

Click **Add sounds**, or drag sound files, a folder or a .zip onto the window. Supported: MP3, WAV, OGG, FLAC, M4A, AAC, WMA and AIFF.

In the picker:

- **To add sound files:** select them, then click **Add files**.
- **To add a whole folder:** go into it (or select it), then click **Add folder**. Every subfolder comes with it, so a **Music** folder holding **Country 90s** and **Rock** shows as Music › Country 90s and Music › Rock, even if Music itself has no sound files.
- **To add just one subfolder:** go into that subfolder and click **Add folder**. Only that folder appears. If its parent is already in your library, the parent is removed automatically. Click **Keep other folders** to keep the parent's other subfolders as folders of their own, or **Undo**.

## Using EazyDeck

- **Click a pad** to play it; click it again to pause.
- **Space** plays or pauses, **Esc** stops everything.
- **Right-click a sound:** Rename (a nickname; the file isn't renamed), Add to favourites, Set hotkey, Put in hotkey slot (free slots listed first), Move back (after you've dragged it to another folder), Show in File Explorer, Remove from list.
- **Drag a sound** onto a folder to move it there, or onto Favourites to star it. Every move has **Undo**.
- **Auto-optimise your mic** (in the setup tour, or Settings › Microphone › Auto-optimise my mic): about a minute of short prompts (stay quiet, type, talk normally, breathe, open a window, speak softly, cheer loudly) while EazyDeck listens, then it tries settings on your own recordings and applies the best ones, with Undo. Best done outside a call.
- **Microphone settings** (Settings › Microphone): pick Headset or Speakers, choose a cleaning preset, or fine-tune every part. Turn on **Hear myself** to listen to your cleaned mic while you adjust it.
- **Right-click a folder:** Rename, Pin to top, Play a random sound from here, Set random-sound hotkey, Show in File Explorer, Remove from list. Removing a folder offers **Keep sub-folders** and **Undo**. No files are ever deleted.
- **Right-click "All sounds"** to hide it from the list. Right-click an empty part of the sidebar to show it again, or to bring back anything you removed.
- **Favourites** sit at the top of every list, with their own entry under All sounds.
- **Player keys** (work in games too): Ctrl+Alt+P play/pause, Ctrl+Alt+Right next, Ctrl+Alt+Left previous, Ctrl+Alt+S stop all. Change any of them in Settings › Hotkeys.
- **Record sounds:** click **Record** above your pads to record whatever your PC is playing (a game, a video, voice chat), then **Stop**. It's trimmed and saved as a WAV in an **EazyDeck Sounds** folder (inside your Music folder unless you choose another in the setup tour or Settings › Audio & devices), and added to your library. Up to 5 minutes per recording.
- **Download a sound from a link:** click the download icon in the title bar, paste a link to a sound file (.mp3, .wav, .ogg and so on) and it's saved as a WAV in **EazyDeck Sounds** and added to your library. YouTube isn't supported (it's against YouTube's rules); play the video and use **Record** instead.
- **No more switching devices:** while EazyDeck runs it makes the cable Windows' default mic and your headset the default output; when you **Quit** EazyDeck both go back as they were. Set your chat app's mic to **Default** once and never touch it again. (Turn this off in Settings › Audio & devices › Windows devices.)
- **Three volumes in the player bar:** the source slider is what your friends hear of your sounds, the **headset** slider is what you hear, and the **microphone** slider is how loud your voice is for friends (also in Settings › Audio & devices). All three use the same scale. Far left mutes; 50% plays sounds exactly as recorded (0 dB); 100% boosts them by +30 dB, with a built-in limiter so boosted sounds never crackle. The dB shown is exactly what's applied. Click the **%** or **dB** next to any slider to type an exact value (Enter to apply, Esc to cancel).
- **Recommended app settings:** Settings › Audio & devices › each source › *Show recommended settings* lists what to set by hand in that app (for Discord: input sensitivity, noise suppression, echo cancellation, gain control and more). The input sensitivity is worked out from your mic settings and follows your **Mic volume**.
- **Update history:** click the clock icon next to **?** in the title bar to see every version with its date and what changed. A dot on it means an update is waiting; you can install it from there too.
- **Player hotkeys** are shown in the middle of the title bar. Click one to change it straight away.
- **Drop tip:** click the small **×** to hide the "Drop sounds…" tip; right-click empty space to bring it back. Dropping files works either way, and the window lights up in your preset colour while you drag.

### More than one app at once

Want sounds in Discord but not in your game? Add another source in **Settings › Audio & devices**. Each source needs **its own cable**. Free VB-Cable gives you one; the VB-Cable A+B and C+D packs from vb-audio.com add four more.

## If something isn't working

- **Friends can't hear sounds:** check your chat app's microphone is set to *CABLE Output*, and the source isn't muted in EazyDeck's player bar.
- **Discord cuts the music out:** in Voice & Video, turn **Echo Cancellation off** and set **Noise Suppression to None**.
- **Sounds jump back to full volume after a pause:** that's Discord's **Automatic Gain Control** turning quiet audio up. Turn it off in Voice & Video. If it happens in your own headset, turn off **Loudness Equalization** (Windows Sound settings › your headset › Properties › Enhancements) and any "volume normaliser" in your headset's own app.
- **Friends hear typing or breathing:** open Settings › Microphone and try the **Strong** preset, or raise the gate's **Threshold**.
- **A hotkey does nothing:** another app may already use it. EazyDeck tells you, and you can pick a different one in Settings › Hotkeys.
- **Still stuck:** run **Settings › Help & tour › Run audio check**, or download **EazyDeck-AudioCheck.exe** from the release. It tests every step and shows PASS or FAIL for each.

Your settings live in `%AppData%\EazyDeck`. Deleting that folder resets EazyDeck. Your sound files are never moved or deleted.

- **Friends hear you twice (echo):** Windows' "Listen to this device" is also sending your mic into the cable. EazyDeck warns you and can turn its own copy of your voice off in one click (your mic then works even with EazyDeck closed).

## Running in the background

Closing EazyDeck with **X** tucks it into the tray by the clock, so your hotkeys keep working. A notification confirms it for 8 seconds. Click it or the tray icon to open EazyDeck again; right-click the tray icon to **Quit**. Prefer X to quit? Turn off **Settings › General › Keep running when I close the window**.

## Updates

EazyDeck checks for a new version when it starts, every 2 minutes while it's open, and shortly after your PC wakes from sleep. A tiny background check also runs every 10 minutes while it's closed and shows a Windows notification (once per version). When one is ready, a bar appears in the app and Windows shows a notification. Click **Update now** and EazyDeck updates and restarts, keeping your settings and sounds. Turn this off in Settings › General › Updates.

---

This repository only holds the finished downloads. The source code is private.
