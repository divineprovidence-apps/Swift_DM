# SwiftDL — Free, Fast Download Manager

**SwiftDL** is a free, open-source download manager for **Windows, macOS and Linux**, with a companion browser extension.
It downloads files faster by splitting them into many connections, resumes interrupted downloads, and saves videos from YouTube and 1000+ other sites.

No ads. No account. No tracking.

---

## ✨ Features

### ⚡ Speed
- Up to **64 connections per file**
- When one part is slow, idle connections take over the rest of it
- Optional **aria2c** for even faster video downloads
- Global speed limit, so downloads don't use up your whole connection

### 🔁 Reliability
- **Pause and resume** at any time, even after a restart, crash or lost connection
- When a server is busy, SwiftDL slows down and retries instead of failing

### 🎬 Videos
- Download from **YouTube and 1000+ sites** (through yt-dlp)
- Choose the video quality before downloading
- Supports **HLS (.m3u8)** and **DASH (.mpd)** streams
- Audio and video are merged automatically (with FFmpeg)
- yt-dlp and FFmpeg are installed and updated automatically, with no setup

### 📋 Queues
- **Download later**: add downloads to a queue and start them when you want
- Create **as many queues as you like**, each started separately
- Choose **how many downloads run at a time** in each queue
- Add downloads to a queue that's already running

### 🔒 Privacy
- **Lock a queue with a PIN** so nobody else can see what's in it
- Locked queues lock again automatically when SwiftDL is minimised to the tray
- Everything stays on your computer. Nothing is uploaded.

### 🗂️ Duplicate detection
- Warns you when you **already have a file**
- The extension marks videos on a page that you've **already downloaded**
- Add your drives or folders to the library so SwiftDL can check them too

### 🖥️ Desktop
- Tray icon and minimise to tray
- Notifications when downloads finish
- Starts with your computer (optional)
- Picks up download links you copy
- Uninstall straight from Settings
- Works when **several users are signed in** to the same computer

### 🌐 Browser extension
- **Download with SwiftDL** button over videos
- A list of all the media found on the page
- Right-click any link → **Download with SwiftDL**
- Can take over the browser's own downloads (optional)
- Works with **Chrome, Edge, Brave and Firefox**

---

## 📥 Installation

### 1. Install the app

Download the latest version from the **[Releases](../../releases)** page:

| System  | File |
|---------|------|
| Windows | `SwiftDL_x.y.z_x64-setup.exe` (recommended) or `.msi` |
| macOS   | `.dmg` |
| Linux   | `.AppImage`, `.deb` or `.rpm` |

### 2. Install the browser extension

1. Download **`swiftdl-extension.zip`** from the same release.
2. **Unzip it into a folder you'll keep.** The browser loads the extension from this folder, so don't delete it.
3. Open the extensions page:
   - **Chrome:** `chrome://extensions`
   - **Edge:** `edge://extensions`
   - **Brave:** `brave://extensions`
4. Turn on **Developer mode** (top-right corner, or the left side in Edge).
5. Click **Load unpacked** and choose the unzipped folder.
6. Pin the SwiftDL icon to your toolbar.

> **Firefox:** open `about:debugging#/runtime/this-firefox` → **Load Temporary Add-on** → choose `manifest.json`.

### 3. Connect the extension

Start SwiftDL, then click the extension icon in your browser.
SwiftDL asks you to **Allow** the connection. Click it once, and you're done.

---

## 🚀 How to use

### Download a file
- **Paste a link** into the bar at the top of SwiftDL, **or**
- **Right-click** a link in your browser → **Download with SwiftDL**, **or**
- Turn on **Take over browser downloads** in the extension's options, so every download goes to SwiftDL.

### Download a video
1. Open the video page in your browser.
2. Click the **Download with SwiftDL** button that appears over the video, or click the extension icon to see every video on the page.
3. In the window that opens, choose the **quality**, file name and folder.
4. Click **Download now**.

### Download later (queues)
1. In the save window, choose **Download later**.
2. Pick an existing queue or create a new one.
3. Open the queue in the sidebar and click **Start** when you're ready.
4. Use **At a time** to set how many downloads run together.

### Lock a queue
1. Open a queue and click the **🔒 lock** button.
2. Set a PIN (at least 4 digits).
3. The queue's contents are now hidden until you enter the PIN.

### Pause, resume and speed up
- Click **Pause** or **Resume** on any download, even after closing SwiftDL.
- Change the **number of connections** on a running download to speed it up.
- Set a **speed limit** in Settings.

---

## ⚙️ Settings worth knowing

| Setting | What it does |
|---------|--------------|
| Default folder | Where downloads are saved |
| Connections per file | 1–64. More is usually faster |
| Downloads at a time | How many downloads run at the same time |
| Speed limit | Caps total download speed |
| Faster video downloads | Uses aria2c for videos |
| Start with computer | Runs SwiftDL in the tray when you sign in |
| Library | Folders to check for files you already have |
| Uninstall | Removes SwiftDL. Your downloaded files are kept |

---

## ❓ FAQ

**Is it really free?**
Yes. There are no ads, no premium version and no account.

**Does it send my data anywhere?**
No. Your history and settings stay on your computer. SwiftDL only connects to the sites you download from, and to the official yt-dlp and FFmpeg pages to set those tools up.

**Why does Windows or my antivirus warn me?**
New apps without a paid code-signing certificate often get a SmartScreen warning. Click **More info → Run anyway**. The source code is public, so you can check it yourself.

**The extension says "SwiftDL isn't running".**
Start the SwiftDL app first. Then click the extension icon again.

**Will uninstalling delete my downloads?**
No. Only the app is removed. To remove the extension, use your browser's extensions page.

---

## 🛠️ Build from source

```sh
npm install
npm run tauri dev      # run in development
npm run tauri build    # build installers
```

You need [Node.js](https://nodejs.org) 20+, [Rust](https://rustup.rs), and the [Tauri prerequisites](https://tauri.app/start/prerequisites/) for your system.

---

## Support SwiftDL ☕

SwiftDL is free, with no ads and no account. If it saves you time, you can support its development with a coffee:

**[☕ Buy me a coffee](https://buymeacoffee.com/divineprovidence)**

<a href="https://buymeacoffee.com/divineprovidence">
  <img src="PASTE-THE-IMAGE-URL-HERE" alt="Buy Me a Coffee QR code" width="180">
</a>

Scan the code with your phone, or click it.

If SwiftDL saves you time, give the project a ⭐ on GitHub. It helps others find it.
