# EazyDeck

**The soundboard for gamers and streamers.** Play sound effects and music to your friends while you talk, in Discord, TeamSpeak, in-game voice chat, OBS or calls. They hear your voice and your sounds together, and you hear them too.

**[Download the latest EazyDeck.exe](../../releases/latest)**: free, for Windows 10 and 11. Run it and the EazyDeck installer opens.

## What it does

- **Sources:** send sounds to Discord, games and more, each with its own volume and mute. Click a source's icon to mute it, or its name to switch between them.
- **Sound slots 1–10:** put any sound in a slot and fire it with **Ctrl+Alt+1** to **Ctrl+Alt+0**, even while you're in a game. Each slot takes its sound's name.
- **Your library, your way:** add files, folders or a .zip. Folders keep their exact names and become categories, subfolders included.
- **Right-click anything:** rename sounds and folders with a nickname, star favourites, pin folders to the top, give a folder a random-sound hotkey, or remove things from the list (with Undo).
- **Search:** press **Ctrl+K** (you can change this in Settings › Hotkeys).
- **Four colour presets:** Volt, Ember, Plasma and Frost, with a fully dark window to match.
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
| **Discord** | User Settings (cog, bottom left) › Voice & Video › Input Device. Then turn **Echo Cancellation off** and set **Noise Suppression to Standard**: echo cancellation treats your sounds as echo and cuts them out. |
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
- **Right-click a sound:** Rename (a nickname; the file isn't renamed), Add to favourites, Set hotkey, Put in hotkey slot (free slots listed first), Show in File Explorer, Remove from list.
- **Right-click a folder:** Rename, Pin to top, Play a random sound from here, Set random-sound hotkey, Show in File Explorer, Remove from list. Removing a folder offers **Keep sub-folders** and **Undo**. No files are ever deleted.
- **Right-click "All sounds"** to hide it from the list. Right-click an empty part of the sidebar to show it again, or to bring back anything you removed.
- **Favourites** sit at the top of every list, with their own entry under All sounds.
- **Player keys** (work in games too): Ctrl+Alt+P play/pause, Ctrl+Alt+Right next, Ctrl+Alt+Left previous, Ctrl+Alt+S stop all. Change any of them in Settings › Hotkeys.
- **Two volumes:** the source slider is what your friends hear; **My headset** is what you hear.

### More than one app at once

Want sounds in Discord but not in your game? Add another source in **Settings › Audio & devices**. Each source needs **its own cable**. Free VB-Cable gives you one; the VB-Cable A+B and C+D packs from vb-audio.com add four more.

## If something isn't working

- **Friends can't hear sounds:** check your chat app's microphone is set to *CABLE Output*, and the source isn't muted in EazyDeck's player bar.
- **Discord cuts the music out:** in Voice & Video, turn **Echo Cancellation off** and set **Noise Suppression to Standard**.
- **A hotkey does nothing:** another app may already use it. EazyDeck tells you, and you can pick a different one in Settings › Hotkeys.
- **Still stuck:** run **Settings › Help & tour › Run audio check**, or download **EazyDeck-AudioCheck.exe** from the release. It tests every step and shows PASS or FAIL for each.

Your settings live in `%AppData%\EazyDeck`. Deleting that folder resets EazyDeck. Your sound files are never moved or deleted.

- **Friends hear you twice (echo):** Windows' "Listen to this device" is also sending your mic into the cable. EazyDeck warns you and can turn its own copy of your voice off in one click (your mic then works even with EazyDeck closed).

## Running in the background

Closing EazyDeck with **X** tucks it into the tray by the clock, so your hotkeys keep working. A notification confirms it for 8 seconds. Click it or the tray icon to open EazyDeck again; right-click the tray icon to **Quit**. Prefer X to quit? Turn off **Settings › General › Keep running when I close the window**.

## Updates

EazyDeck checks for a new version when it starts, every 10 minutes while it's open, and shortly after your PC wakes from sleep. A tiny background check also runs every 10 minutes while it's closed and shows a Windows notification (once per version). When one is ready, a bar appears in the app and Windows shows a notification. Click **Update now** and EazyDeck updates and restarts, keeping your settings and sounds. Turn this off in Settings › General › Updates.

---

This repository only holds the finished downloads. The source code is private.
