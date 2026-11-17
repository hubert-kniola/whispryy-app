# Whispryy — live captions

Whispryy turns Discord voice chat — or audio from a browser or any other program — into
**live captions right on top of your game**. It shows who is speaking, and speech is recognized
**locally on your PC**: your audio is never sent anywhere.

Made with deaf and hard-of-hearing people in mind — and handy in noisy places, late at night or with poor audio.

**🌐 Website:** https://hubert-kniola.github.io/whispryy-app/

## ⬇ Download

### [Download Whispryy for Windows](https://github.com/hubert-kniola/whispryy-app/releases/latest/download/Whispryy.zip)

Windows 10/11 64-bit · one version for NVIDIA, AMD and Intel GPUs · [all versions](https://github.com/hubert-kniola/whispryy-app/releases)

> The app interface is in Polish. Button names below are given in Polish with an English translation.

## Features

- **Listens only to the program you choose** — Discord, a browser or any other program. Game sounds, music
  and other apps never end up in the captions.
- **Shows who is speaking** — with Discord, every person gets their own nick color.
- **Captions where you want them** — in any corner or anywhere on the screen; a keyboard shortcut
  (`Ctrl+Alt+N` by default) toggles the position, even in-game.
- **Customizable look** — font, width, transparency, how long captions stay on screen.
- **Stays out of your game's way** — leaves part of the CPU and GPU memory for the game.
- **Private** — speech recognition runs on your graphics card, no audio is uploaded to the internet.
- **Updates itself** — tells you about a new version, which you install with one click.

## Installation

1. Download `Whispryy.zip` and **extract the whole folder**, e.g. to the Desktop or Documents.
   Don't extract it to *Program Files* and don't run it straight from the ZIP.
2. Run `Whispryy.exe`. If Windows shows "Windows protected your PC", click
   **More info → Run anyway** (the program has no paid code-signing certificate).
3. On first launch Whispryy downloads the speech recognition model (~1.6 GB) and, on NVIDIA cards,
   the CUDA libraries (~1.2 GB). Progress — with percentages — is shown in the panel on the **Stan** (Status) page.
   This happens only once.

Whispryy runs in the background — its icon is in the tray next to the clock. Click it to open the panel.

## Requirements

- Windows 10 or 11, 64-bit.
- A graphics card with up-to-date drivers: **NVIDIA** (GeForce / RTX), **AMD Radeon** or **Intel Arc**.
  Whispryy picks what to run on by itself.
- Without a dedicated GPU it runs on the CPU — slower and with a smaller model.
- About 5 GB of free disk space (program, model and — on NVIDIA cards — the CUDA libraries).

## Updates

Whispryy checks for new versions by itself and shows a notification. Install it with one click in the panel,
on the **Aktualizacje** (Updates) tab — the program restarts. Your settings, Discord keys and the downloaded
model are kept.

## Nicks and "who is speaking" (optional, about 2 minutes)

Captions work right away. To also see who is speaking, connect Whispryy to Discord — step-by-step
instructions are in the panel on the **Discord** tab:

1. Create a free application in the [Discord Developer Portal](https://discord.com/developers/applications) (**New Application**).
2. On the **OAuth2** tab, copy the **Client ID** and the **Client Secret** (**Reset Secret**).
3. Under **Redirects**, add `http://localhost` and click **Save Changes**.
4. Paste the keys into the Whispryy panel → **Zapisz i połącz** (save and connect) → click **Authorize** in Discord.

## FAQ and troubleshooting

- **Is my audio sent to the internet?** No. Speech is recognized on your computer.
- **I don't see captions of my own voice.** Discord doesn't play back your microphone, so Whispryy can't hear it.
- **Captions don't show up in my game.** Games in exclusive fullscreen mode cover the captions — switch the game
  to borderless windowed mode.
- **Quiet people are missed.** In the panel, on the **Stan** (Status) page, lower **Próg mowy** (speech threshold).
- **The update won't install.** The Whispryy folder must be writable — move it to e.g. Documents.
- **Something doesn't work?** Panel → **Ogólne** (General) → **Log błędów** (error log) — this file helps find
  the cause. You can report problems in [Issues](https://github.com/hubert-kniola/whispryy-app/issues).

Settings and logs are stored in `%APPDATA%\Whispryy`.

---

<sub>This repository contains only releases and the website — the application's source code is not public.</sub>
