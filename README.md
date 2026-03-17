# 🛡️ FlowGuard — Focus RPG for Students

> A gamified Chrome extension that blocks distractions, tracks your focus habits, and rewards deep work with XP, levels, and badges.

![Version](https://img.shields.io/badge/version-3.0.0-black) ![License](https://img.shields.io/badge/license-free-green) ![Platform](https://img.shields.io/badge/platform-Chrome%20%7C%20Brave%20%7C%20Edge-blue)

---

## ✨ What is FlowGuard?

FlowGuard is a Chrome extension built for students and researchers who want to actually get things done. It's not just a site blocker — it understands your goals, guards your attention, and turns every focus session into a game you want to win.

- 🎯 Set a research goal before each session
- 🚫 Block distracting sites automatically
- 🔒 Ultra Focus mode — hard lockdown, no override
- ⚡ Earn XP, level up, unlock badges
- 📊 Daily & weekly challenges
- 🏆 Personal leaderboard of your best sessions
- 🔥 Streak tracking to build daily habits

---

## 📦 Installation

### Step 1 — Download
Download the latest version from the [releases](../../releases) or directly:

👉 **[Download flowguard-v3.zip](./flowguard-v3.zip)**

### Step 2 — Unzip
Extract the zip file. You'll get a folder called `flowguard3`.

### Step 3 — Open Chrome Extensions
Paste this in your Chrome address bar:
```
chrome://extensions
```

### Step 4 — Enable Developer Mode
Toggle **Developer mode** on in the top-right corner.

### Step 5 — Load the Extension
Click **"Load unpacked"** → select the `flowguard3` folder.

### Step 6 — Pin it
Click the 🧩 puzzle icon in Chrome toolbar → find FlowGuard → click 📌 Pin.

You're ready. Click the shield icon and start your first session!

---

## 🎮 Focus Modes

| | Normal Focus | Ultra Focus |
|---|---|---|
| **What's blocked** | Blocklist sites only | Everything except whitelist |
| **Override** | Yes — continue anyway | ❌ Hard block, no bypass |
| **XP multiplier** | Standard | **1.5×** |
| **Best for** | Everyday studying | Exams, deep work |

---

## 🏅 Progression System

### 20 Levels
From `🌱 Distracted Freshman` all the way to `🌌 Legendary Scholar`.

XP is earned every session based on:
```
XP = duration (mins) × 2 × focus score multiplier × ultra focus bonus
```

| Focus Score | Multiplier |
|---|---|
| 90–100 | 2.0× |
| 75–89 | 1.5× |
| 60–74 | 1.2× |
| 40–59 | 1.0× |
| Below 40 | 0.7× |

### 16 Badges
Including: First Session, On Fire (3-day streak), Week Warrior, Perfectionist (100 score), Marathon (90-min session), Ultra Focused, Night Owl, Early Bird, XP Hoarder, and more.

### Daily & Weekly Challenges
Rotating challenges that award bonus XP — things like "Focus for 60 minutes today" or "Complete 3 Ultra Focus sessions this week."

---

## ⚙️ Features

### Smart Whitelist Search
Type a site name like "youtube" and pick it from a dropdown — no need to remember URLs. Add sites to your global whitelist (always allowed) or a per-session whitelist (this session only).

### Blocked Sites List
View and manage all blocked sites in Settings. Remove any default site or add your own custom ones.

### Optional AI Mode
Add your Claude API key in Settings for smarter tab relevance scoring. Uses the lightweight Haiku model — costs fractions of a cent per session. Completely optional.

### Session Recap
After every session you get a full breakdown:
- Focus score (0–100)
- XP earned
- Time focused
- Distractions blocked
- Tabs opened
- Streak progress
- New badges unlocked
- Challenge completions

---

## 🗂️ File Structure

```
flowguard3/
├── manifest.json        ← Extension config
├── background.js        ← Session logic, tab monitoring, gamification engine
├── content.js           ← Distraction overlay injected into blocked pages
├── pages/
│   ├── popup.html       ← Extension popup UI
│   └── popup.js         ← Popup logic, site search, rendering
└── icons/
    ├── icon16.png
    ├── icon48.png
    └── icon128.png
```

---

## 🔄 Updating the Extension

When a new version is released:
1. Download the new zip
2. Replace the contents of your `flowguard3` folder
3. Go to `chrome://extensions`
4. Click the **↺ refresh** icon on FlowGuard

---

## 🔒 Privacy

- **No data leaves your browser.** All session history, XP, badges, and streaks are stored locally using Chrome's `storage` API.
- No account required. No tracking. No analytics.
- The optional AI mode sends only your current tab's URL and title to the Anthropic API — nothing else.

---

## 🛠️ Built With

- Vanilla JavaScript (no frameworks)
- Chrome Extensions Manifest V3
- Chrome Storage API
- Anthropic Claude API (optional)

---

## 📄 License

Free to use and share. Built for students who actually want to study.

---

*Made with ☕ and too many blocked Reddit sessions.*
