# CoachBoard

**A desktop app for strength coaches.** Manage your athletes, build and analyse training programs, and send them out as polished Excel sheets, all on your own computer. It runs fully offline and needs no account.

This repository only hosts the installers. **[Download the latest version →](https://github.com/Fabian0270/CoachBoard-releases/releases/latest)**

---

## What it does

### Athletes
- One page per athlete with contact details, sport, weight class, notes and their recorded maxes.
- **Progress tab**: an estimated 1RM for squat, bench and deadlift across every block, the best set of each week with the program it came from, a timeline of PRs showing what each one beat, and the bar speed from saved bar path sets.
- **Payments**: track who has paid, who is due and whose paid period is about to run out, with reminders before it happens.

### Dashboard
- A **Needs attention** list of what to act on: a block ending within a week with no next block lined up, an active program where training days have passed with nothing logged, an athlete with no active program, and videos waiting in the Discord inbox. Every line takes you straight to where you fix it.

### Building programs
- Create a multi-week program in one step, for an athlete or as a **template** with no athlete.
- A **calendar** of the whole block that shows each day at a glance, and a **block view** that lays one training day out across every week so you can edit the progression side by side.
- **Last week, under every exercise**: what was planned on the same day last week and what the athlete actually did.
- **Load suggestions**: write a target like "RPE 8" or "75%" and CoachBoard suggests the load from the athlete's max, rounded to 2.5 kg. Back-offs like "-10%" are read from the set above. Nothing is filled in unless you accept it.
- **Progress an exercise through the block**: step load, RPE, percentage or reps week by week, with optional deload weeks. You see every change before it's applied.
- **Replace an exercise** across the whole block (or from a chosen week on) in one step.
- **Duplicate a program** for another athlete or as a template, starting on any week. Loads can be scaled to the new athlete's maxes.
- **Paste straight from Excel, Numbers or Google Sheets** into a day.
- An optional **Notes column** for your coaching cues, plus a note on each training day.
- **Undo and redo** every change in the program, step by step (Ctrl+Z / Ctrl+Y).
- **Fully usable from the keyboard** as well as the mouse. Settings → Help lists every shortcut.
- Changing a program's start date moves its training days with it.
- **Generate a draft program** from the athlete's data and your bookmarked programs. You always edit the final result.

### Excel in and out
- **Import programs** you already have, one at a time or several at once, with column mapping for sheets in your own format. Your own notes column comes in as cues.
- **Import results**: read the athlete's filled-in sheet back in to log what they did.
- **Export** to clean `.xlsx` in one of three built-in looks, or in **your own style**: CoachBoard copies the layout of one of your existing sheets so new programs look like the ones your athletes already know. Preview the exact sheet before saving.
- **Email a program** straight to an athlete from inside the app.

### Reports
- A **program report** per block: intensity, plus weekly sets and tonnage per lift, done against planned.
- **Compare programs** side by side.

### Discord check-ins (optional)
- Pull athletes' lift videos from your Discord server into an inbox. CoachBoard reads the caption, suggests the programmed exercise it belongs to, and lets you reply in the channel or by DM without leaving the app.

### Bar path & bar speed
- Click the bar in any clip, from your computer or a Discord check-in, and CoachBoard **tracks every frame**, drawing the path as it goes.
- **Per rep**: speed on the way up, range of motion, how far the bar drifted sideways, time on the way down and the pause at the bottom.
- A **speed chart** through the set that marks where each rep slowed down most.
- An **estimated RPE** for the last rep, an **estimated 1RM** from a single set, a load–velocity profile across several loads, and velocity loss. As an athlete's tracked history builds up, it replaces the published reference values.
- An optional **skeleton** with knee and hip angles plotted against bar speed, so you can see where a rep stuck. Joints can be corrected by hand.
- **Frame-by-frame stepping, slow motion** and keyboard controls. Loop any single rep, or see the reps drawn apart and laid over each other.
- Set the **scale from the plate** (with a magnifier while you place it) for real distances.
- **Save** a set with a note and reopen it later, or **compare two lifts** side by side or on one plot, with a pen to draw on them.
- **Share it**: save the clip with the path drawn in, copy or save a frame as an image, or export the rep table as a CSV.
- Videos are analysed **on your computer** and never uploaded.

### Screen recording
- Record your screen, any window or CoachBoard itself, with voice-over and optionally your webcam and system sound. A small control bar stays on top while you record.
- Afterwards, move or resize the webcam bubble, trim the start and end, then send the video to the athlete over Discord or email, or save it. CoachBoard tells you up front if the video will be too big to send.

### Calculators
- **Meet scoring**: IPF GL Points, DOTS and Wilks.
- **Warm-up ladder** into a 1RM attempt, with the plates for each side of the bar.

### And also
- Bookmark programs and filter by bookmarks.
- Backups from Settings, with automatic backups kept in the background.
- Light, dark or system theme.


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
