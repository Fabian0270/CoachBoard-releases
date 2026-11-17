# CoachBoard

**A desktop app for strength coaches.** Manage your athletes, build and analyse training programs, and send them out as polished Excel sheets, all on your own computer. It runs fully offline and needs no account.

This repository only hosts the installers. **[Download the latest version →](https://github.com/Fabian0270/CoachBoard-releases/releases/latest)**

---

## What it does

- **Athletes**: training maxes, progress over time and payments, all in one place.
- **Program builder**: multi-week programs with per-set prescriptions. Copy and move training days, reorder exercises, and work fully from the keyboard if you like.
- **Excel in and out**: import the programs you already have, and export new ones as clean `.xlsx` sheets. Choose a built-in look or let CoachBoard copy the layout of your own spreadsheet so new programs match your house style.
- **Send programs**: email a program straight to an athlete from inside the app.
- **Discord check-ins** (optional): pull athletes' lift videos from your Discord server into an inbox, match them to the programmed exercise and reply without leaving the app.
- **Bar path & bar speed**: click the bar in any clip and CoachBoard tracks it, showing the path, rep speed, estimated RPE and an estimated 1RM. There's an optional skeleton overlay for knee and hip angles. Videos are analysed on your computer and never uploaded.
- **Screen recording**: record yourself talking an athlete through their program or lift, with voice and webcam. Trim it and send it over Discord or email.
- **Reports & calculators**: volume and intensity breakdowns, program comparison, an RPE chart, 1RM estimates and warm-up sets.
- **Backups**: save and restore a backup from Settings, with automatic backups kept in the background.
- **Light and dark mode.**

---

## Download & install

Go to the **[latest release](https://github.com/Fabian0270/CoachBoard-releases/releases/latest)** and download the file for your computer.

### Windows (64-bit Windows 10 or 11)

1. Download **`CoachBoard-Setup-x.x.x.exe`**.
2. Run it. Windows may show a blue **"Windows protected your PC"** screen because the installer isn't code-signed yet. Click **More info → Run anyway**.
3. Open **CoachBoard** from the Start menu or the desktop shortcut.

New versions download quietly in the background and install the next time you restart the app.

### macOS (Apple Silicon: M1, M2, M3, M4 and later)

1. Download **`CoachBoard-x.x.x-arm64.dmg`**.
2. Open it and drag **CoachBoard** into **Applications**.
3. The app isn't notarised by Apple yet, so the first launch is blocked:
   - **macOS 15 (Sequoia) and later:** try to open CoachBoard once and close the warning. Then go to **System Settings → Privacy & Security**, scroll down and click **Open Anyway**.
   - **macOS 14 and earlier:** right-click CoachBoard in Applications, choose **Open**, then **Open** again.

   You only need to do this once.

On Mac, updates aren't automatic yet: download the new `.dmg` from this page and drag it over the old app. Your data is kept.

> Intel Macs aren't supported yet.

---

## Your data stays on your computer

CoachBoard has no cloud and no account. Everything is saved in one folder on your computer:

- **Windows:** `%APPDATA%\coachboard-electron`
- **macOS:** `~/Library/Application Support/coachboard-electron`

**Settings → Your data** shows the exact location, opens the folder, and lets you save or restore a backup. A backup holds your athletes, programs, payments, Excel styles and settings. Video clips aren't included because they can run to many gigabytes, so copy the folder itself if you want those too.

The app only goes online for things you turn on (emailing a program and Discord sync) and to check for updates.

---

## Problems or ideas?

Open an issue in the **[Issues](https://github.com/Fabian0270/CoachBoard-releases/issues)** tab. If something went wrong, the log file in the data folder above helps a lot.

---

The source code isn't public. This repository only holds the release downloads.
