# Pomodoro Day Log

A daily Pomodoro timetable. Type a task in an hourly slot, press play, and the timer runs a focus session and a break. Slots can be marked productive (green) or unproductive (red), and the app shows productive and unproductive hours and percentages for the day, plus a 14-day history.

Everything is plain HTML, CSS and JavaScript. There is no build step and no server. Data is stored in the browser (localStorage) on the device you use.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole app |
| `manifest.webmanifest` | Lets you install it as an app |
| `sw.js` | Offline support and notification clicks |
| `netlify.toml` | Netlify settings |
| `icons/` | App icons |

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
- Press play once and allow **notifications** when asked. A notification and a chime fire when each focus session or break ends, even if the window is hidden.
- The timer keeps its own clock, so the remaining time is always correct when you return.
- Leave **Screen awake** on to stop a phone or laptop screen from sleeping while the timer runs.
- Do not close the tab or app, and do not let the phone lock for long. A web page cannot run once the browser has been closed or the device has put it to sleep.
- On Windows and Mac, if Chrome's **Memory Saver** is on, add your site to **Always keep these sites active** in `chrome://settings/performance`.

## Move your data

Use **Backup JSON** to save everything and **Import backup** to load it on another device or browser. Backups made in the earlier Claude version of this app import here too.
