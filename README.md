# 🎓 EduFocus – YouTube Learning Mode

A Chrome extension that transforms YouTube into a distraction-free learning environment.

---

## Features

| Feature | Description |
|---|---|
| 📚 **Educational Detection** | Automatically detects educational videos via YouTube category & title/description keywords |
| 🔒 **Focus Mode** | Hides comments, dims distracting UI, removes endscreen clutter |
| 🎯 **Smart Sidebar** | Replaces YouTube's algorithm-driven sidebar with educational suggestions related to your current video |
| 🔍 **Custom Search** | Search for any educational topic directly within the sidebar panel |
| ⚡ **Auto-enable** | Optionally enable Focus Mode automatically when an educational video is detected |

---

## Installation

1. Download and unzip this folder
2. Open Chrome and go to `chrome://extensions/`
3. Enable **Developer Mode** (top-right toggle)
4. Click **"Load unpacked"**
5. Select the `yt-focus-extension` folder
6. Navigate to any YouTube video — the 🎓 icon will appear in your toolbar

---

## How It Works

### Educational Video Detection
The extension checks two things:
- **YouTube category**: If the video is categorized as "Education" in YouTube's metadata
- **Keywords**: Scans the video title and description for 40+ educational keywords (tutorial, lecture, course, explained, etc.)

### Focus Mode
When active, Focus Mode:
- ✅ Hides the comments section entirely
- ✅ Dims the masthead navigation bar
- ✅ Dims endscreen recommendation overlays
- ✅ Adds a subtle blue glow around the video player to help you stay focused
- ✅ Hides autoplay overlays

### Educational Sidebar
The extension fetches YouTube search results for topics related to the current video and renders them in a clean, ad-free panel — bypassing YouTube's engagement-optimized recommendation algorithm entirely.

---

## Settings (Popup)

| Setting | Default | Description |
|---|---|---|
| Focus Mode | OFF | Master toggle for all focus features |
| Hide Comments | ON | Removes comment section |
| Dim Distracting UI | ON | Dims navigation, overlays |
| Auto-enable on Edu videos | OFF | Auto-activates when educational video detected |

---

## Tips

- You can also toggle Focus Mode directly on the video page via the **🎓 Focus ON/OFF** button next to the Like/Share buttons
- Use the search bar in the sidebar to find educational content on any topic
- Works with YouTube's dark and light themes

---

## File Structure

```
yt-focus-extension/
├── manifest.json      — Extension config (MV3)
├── content.js         — Main logic: detection, focus mode, sidebar
├── styles.css         — All styles for focus mode & panel
├── popup.html         — Extension popup UI
├── popup.js           — Popup logic
├── background.js      — Service worker (badge updates)
└── icons/             — Extension icons
    ├── icon16.png
    ├── icon48.png
    └── icon128.png
```
