# SwiftDL — Free, Fast Download Manager

**SwiftDL** is a free download manager for **Windows, macOS and Linux**, with a companion browser extension.
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
- **Force start ⚡**: download one item right now, without waiting in line and without taking a slot from the queue

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
- **Select several downloads** and remove them together, with or without their files
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

### Skip the line (Force start)
Click **⚡** on any download that is waiting or queued. It starts right away, and the rest of the queue carries on as before.

### Lock a queue
1. Open a queue and click the **🔒 lock** button.
2. Set a PIN (at least 4 digits).
3. The queue's contents are now hidden until you enter the PIN.

### Delete several downloads
1. Tick the box next to each download, or use **Select all** at the top of the list.
2. Click **Delete selected…**.
3. Choose **Remove from list** to keep the files, or **Remove and delete files** to move finished files to the Recycle Bin / Trash.

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

## ☕ Support SwiftDL

SwiftDL is free, with no ads and no account, and it's made in spare time. If it saves you time, you can support its development in whichever way suits you:

| Buy Me a Coffee | Ko-fi | Liberapay |
|:---:|:---:|:---:|
| <a href="https://buymeacoffee.com/divineprovidence"><img src="https://github.com/divineprovidence-apps/Swift_DM/releases/download/v0.1.0/qr-code.png" alt="Buy Me a Coffee QR code" width="160"></a> | <a href="https://ko-fi.com/divineprovidence"><img src="https://github.com/divineprovidence-apps/Swift_DM/releases/download/v1.0.0/kofi-qrcode.png" alt="Ko-fi QR code" width="160"></a> | <a href="https://liberapay.com/divineprovidence/donate"><img src="https://liberapay.com/assets/widgets/donate.svg" alt="Donate using Liberapay" height="40"></a> |
| **[One-time coffee](https://buymeacoffee.com/divineprovidence)** | **[One-time or monthly](https://ko-fi.com/divineprovidence)** | **[Weekly, monthly or yearly](https://liberapay.com/divineprovidence/donate)** |

Scan a code with your phone, or click it. You can also find these in the app under **♥ Support SwiftDL**.

Not able to donate? Giving the project a ⭐ on GitHub and telling a friend help a lot too.

Windows App : 
<img width="1915" height="1043" alt="image" src="https://github.com/user-attachments/assets/6b381d47-c36e-4cae-831e-8d54d43a9a5c" />
Browser Extention - Youtube : 
<img width="1367" height="968" alt="image" src="https://github.com/user-attachments/assets/5755f62d-c2ef-4dbf-b216-6f671fe5e38d" />
Browser Extention - Instagram : 
<img width="1490" height="945" alt="image" src="https://github.com/user-attachments/assets/6562fe8e-c95f-4692-85b7-8c0b178eef59" />
Queue :

<img width="673" height="498" alt="image" src="https://github.com/user-attachments/assets/e3227d4d-f20f-416d-9540-b7de98b4027b" />
Settings 1 : 

<img width="767" height="1039" alt="image" src="https://github.com/user-attachments/assets/65cc11a7-6d19-4ca9-b756-b462a5f3a43a" />
Settings 2 : 

<img width="707" height="1038" alt="image" src="https://github.com/user-attachments/assets/9afb0d60-721f-4155-914a-a1126bf29db7" />
