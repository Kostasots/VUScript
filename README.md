# VU Review Log

A single-page, installable web app for field hockey Video Umpires (VUs) to standardize the video review script, log referral decisions, and email a full record to the tournament supervisor or umpire manager.

Built for iPad first, works on iPhone, Android/Samsung, and desktop browsers.

## Try it live

**[Open the app](https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/)**

*(Replace this link once GitHub Pages is enabled — see setup below.)*

## Features

- Guided, step-by-step script for both **Team Referrals** and **Umpire Referrals** (Serious Misconduct, Goal/No Goal, Penalty Stroke/No Penalty Stroke)
- Team selection scoped by **PAHF (international)**, **NCAA Division I** (all sponsoring conferences), or free-text **Other** for exhibition/club matches — Home and Away can each use a different scope
- Automatic tracking of which team has used its referral, with a **shootout reset** (each team regains one referral)
- Optional **personal penalty** step (Yellow Card – 10 min / Red Card) for misconduct reviews
- Auto-formatted game clock entry and quarter/OT/SO tagging per incident
- Smart script generation that reads back the VU's finding in plain language, plus restart and keep/lose outcome — one line the VU can read verbatim to the pitch
- Tracks whether the on-field umpire followed the VU's advice
- One-tap **email export** of the full game log to a supervisor via the device's mail app

## Installing on your device

### iPhone
1. Open the live link above in Safari.
2. Tap the **Share** icon, then **Add to Home Screen**.
3. Launch it from the home screen like a normal app.

### Samsung / Android
1. Open the live link in Chrome or Samsung Internet.
2. Tap the **three-dot menu** → **Add to Home screen** (or **Install app**).
3. Confirm — it now sits on your home screen.

### iPad / Tablet
Same as iPhone: Safari → Share → Add to Home Screen. This is the primary target device for the app.

### Laptop / Desktop
Just open the live link in any modern browser — no install needed.

## Known limitations (v1)

- **Data is stored on the device, not in the cloud.** Settings (supervisor email, custom teams) and the game in progress (teams, referral log, referral status, any open review) are saved in the browser and survive reloads, backgrounding, and power-save tab discards. A saved game older than 24 hours is cleared automatically. Because storage is per browser, the Safari tab and the Home Screen icon on iPhone/iPad keep separate copies, and private browsing or "clear website data" will erase it. Email the log at the end of the game as your permanent record.
- **Email export uses `mailto:`**, which hands off to your device's default mail app with the log pre-filled — you still need to tap Send yourself. There's no silent/automatic email delivery.
- Conference rosters reflect the 2026 season lineup as of this writing; conference realignment happens yearly, so double-check before a tournament and use the custom team field in Settings if something's changed.

## Feedback

Please [open an issue](../../issues) with anything that feels off, confusing, or missing — wording, a missing situation type, a roster correction, anything. No suggestion is too small.

## Local development

This is a single self-contained HTML file (`index.html`) with no build step and no dependencies. To work on it locally, just open `index.html` directly in a browser, or run any static file server:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.
