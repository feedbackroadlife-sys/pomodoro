# Pomodoro Day Log

A daily Pomodoro timetable. The day is split into half-hour slots (05:00 – 05:30, 05:30 – 06:00 and so on). Type a task in a slot and press play: the timer runs the whole slot and checks it off when it ends. There are no breaks. Slots can be marked productive (green) or unproductive (red), and the app shows productive and unproductive hours and percentages for the day, plus a 14-day history.

Everything is plain HTML, CSS and JavaScript. There is no build step and no server. Data is stored in the browser (localStorage) on the device you use.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole app |
| `manifest.webmanifest` | Lets you install it as an app |
| `sw.js` | Offline support and notification clicks |
| `netlify.toml` | Netlify settings |
| `icons/` | Logo and app icons (`logo.svg` and `logo-1024.png` are the logo files) |

## Put it on GitHub

1. Sign in at github.com and choose **New repository**. Name it `pomodoro-day-log` and create it (public or private).
2. On the new repository page choose **uploading an existing file**.
3. Drag in everything from this folder: `index.html`, `manifest.webmanifest`, `sw.js`, `netlify.toml`, `README.md` and the whole `icons` folder.
4. Choose **Commit changes**.

## Publish it with Netlify

1. Sign in at app.netlify.com and choose **Add new site**, then **Import an existing project**.
2. Pick **GitHub**, allow access, and select your `pomodoro-day-log` repository.
3. Leave the build command empty and the publish directory as `.` (the settings are already in `netlify.toml`). Choose **Deploy**.
4. In about a minute you get an address like `https://your-site-name.netlify.app`. You can rename it under **Site configuration**, then **Change site name**.

Every later change you commit to GitHub is published automatically.

## Keep the timer running in the background

- Open the site in Chrome or Edge and use **Install** (the icon in the address bar), or on a phone use **Add to Home screen**. The installed app runs in its own window.
- Press play once and allow **notifications** when asked. A notification and a chime fire when each slot ends, even if the window is hidden.
- The timer keeps its own clock, so the remaining time is always correct when you return.
- Leave **Screen awake** on to stop a phone or laptop screen from sleeping while the timer runs.
- Do not close the tab or app, and do not let the phone lock for long. A web page cannot run once the browser has been closed or the device has put it to sleep.
- On Windows and Mac, if Chrome's **Memory Saver** is on, add your site to **Always keep these sites active** in `chrome://settings/performance`.

## Day setup

Under **Day setup** you can change the hours your day starts and ends and edit your daily checks. Slots are always 30 minutes and there are no breaks. The app always opens on today.

## Move your data

Use **Backup** (bottom of the page) to save everything and **Restore** to load it on another device or browser. Backups made in the earlier Claude version of this app import here too.
