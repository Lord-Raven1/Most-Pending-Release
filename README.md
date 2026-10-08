# Most-Pending

**Most-Pending** is a free Windows desktop app for keeping track of what's coming up: tasks with due dates, weekly routines, a shopping list, quick reminders and a focus timer — all in one dark-themed window.

This repository only hosts the **installer and automatic updates**. The source code is kept in a separate, private repository.

## Features

- **Timeline** of tasks with due dates, priorities, colour-coded tags and sub-tags (e.g. *Work › Slides*), plus filters and bulk actions.
- **Reminders** as Windows notifications, from a week before a task is due down to the last 5 minutes.
- **Weekly routines**, a **shopping list** and **quick reminders**.
- **Focus timer** (countdown or open-ended) that logs time against tasks, with weekly/monthly stats.
- **Runs in the system tray** so reminders keep coming when the window is closed; optional *Start with Windows*.
- **Updates itself** — new versions download in the background and install when you restart.

## Install

1. Open the [latest release](https://github.com/Lord-Raven1/Most-Pending-Release/releases/latest).
2. Download **`MostPending-win-Setup.exe`** and run it. It installs for your Windows user only (no admin rights needed) and adds Start menu and desktop shortcuts.
3. Windows may show a blue **"Windows protected your PC"** (SmartScreen) message, because the app isn't code-signed. Click **More info → Run anyway**.

**Requirements:** Windows 10 or 11 (64-bit). Nothing else needs installing.

## Updates

Most-Pending checks this repository for a new version shortly after it starts and every few hours, downloads it in the background, and asks before restarting to install it. You can also use **Settings → Check for Updates**. After an update, a *What's New* screen lists the changes.

## Your data

- Everything is stored **only on your PC**, in `%AppData%\Most-Pending\`. There's no account and nothing is uploaded.
- The app keeps automatic backups: the previous save and one snapshot per day (last 7 days) in `%AppData%\Most-Pending\backups\`. If the save file is ever damaged, the app restores it from a backup.
- **Settings → Export All Data** saves everything to a JSON file you can keep elsewhere or import on another PC.
- The only network connection the app makes is the update check to GitHub.

## Uninstall

**Windows Settings → Apps → Installed apps → Most-Pending → Uninstall.** Your data is left in `%AppData%\Most-Pending\` in case you reinstall; delete that folder too if you want it gone.

## Feedback & bugs

Use **Settings → Send Feedback** in the app, or [open an issue](https://github.com/Lord-Raven1/Most-Pending-Release/issues/new) here directly. Either way you'll need a GitHub account, and issues are **public**, so please don't include anything private.

## Downloads in each release

| File | What it is |
|---|---|
| `MostPending-win-Setup.exe` | The installer — this is the one you want. |
| `MostPending-win-Portable.zip` | Runs without installing — unzip it and start `Most Pending.exe`. |
| `*.nupkg`, `RELEASES`, `releases.win.json` | Update packages used by the app itself. |
| Source code (zip / tar.gz) | Added automatically by GitHub; contains only this README, not the app. |
