<div align="center">
  
# 📚 Scribd-Downloader-js

### 🚀 Download any document from Scribd as PDF or Images — for free!

<br/>

[![GitHub stars](https://img.shields.io/github/stars/AllLiveSupport/Scribd-Downloader-js?style=for-the-badge&logo=github&color=yellow)](https://github.com/AllLiveSupport/Scribd-Downloader-js/stargazers)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge&logo=opensourceinitiative&logoColor=white)](LICENSE)
[![User Script](https://img.shields.io/badge/User%20Script-Install-670000?style=for-the-badge&logo=tampermonkey&logoColor=white)](scribd.user.js)


<br/>

<img src="https://img.shields.io/badge/Chrome-Supported-success?style=flat-square&logo=googlechrome&logoColor=white"/>
<img src="https://img.shields.io/badge/Firefox-Supported-success?style=flat-square&logo=firefox&logoColor=white"/>
<img src="https://img.shields.io/badge/Edge-Supported-success?style=flat-square&logo=microsoftedge&logoColor=white"/>

---

**✨ Dual Mode • 🎯 Toggle Control • 🧹 Clean PDF Output • 🖼️ Image Export**

</div>

<br/>

---

## 🎯 Three Methods

| Method | Best For | Difficulty |
|:-------|:---------|:-----------|
| 🌐 **Tampermonkey** | Quick & easy browser use (Toggle Button) | ⭐ Easy |
| 🔖 **Bookmarklet** | Quick use without extensions | ⭐ Easy |
| 💻 **Console** | Developers, one-time use | ⭐⭐ Medium |

---

<br/>

## 🌐 Method 1: Tampermonkey (Recommended)

### Step 1: Install Tampermonkey Extension

| Browser | Install Link |
|:-------:|:------------:|
| <img src="https://img.shields.io/badge/Chrome-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white"/> | [Install](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo) |
| <img src="https://img.shields.io/badge/Firefox-FF7139?style=for-the-badge&logo=firefox&logoColor=white"/> | [Install](https://addons.mozilla.org/en-US/firefox/addon/tampermonkey/) |
| <img src="https://img.shields.io/badge/Edge-0078D7?style=for-the-badge&logo=microsoftedge&logoColor=white"/> | [Install](https://microsoftedge.microsoft.com/addons/detail/tampermonkey/iikmkjmpaadaobahmlepeloendndfphd) |

### Step 2: Install the Script

1. Open [**`scribd.user.js`**](scribd.user.js) in this repository.
2. Click the **"Raw"** button.
3. Tampermonkey will automatically detect the script and ask to install. Click **"Install"**.

### Step 3: Use It!

1. 🌐 Go to any **Scribd document** page.
2. 📥 Tap the floating green **"Download"** button at the bottom-right.
3. ⚙️ Select **IMAGES** or **PDF** mode.
4. 🚀 Adjust page range if needed and click **"START DOWNLOAD"**.
5. ⏳ **Keep the PiP window open!** It ensures the download continues in the background.

<br/>

---

## 🔖 Method 2: Bookmarklet

1.  **Create Bookmark**: Add a new bookmark to your browser.
2.  **Name**: Set it to `Scribd Downloader`.
3.  **URL**: Paste everything from [**`Scribd Downloader Bookmark.txt`**](Scribd%20Downloader%20Bookmark.txt).
4.  **Action**: Click the bookmark while on a Scribd page to launch.

<br/>

---

## 💻 Method 3: Console

1.  **F12**: Open Developer Tools (Console tab).
2.  **Paste**: Copy code from [**`Scribd Downloader.txt`**](Scribd%20Downloader.txt).
3.  **Enter**: Run the script to show the panel.

<br/>

---

## 🛠️ Features Detailed

- 🖼️ **Image Mode**: Saves every page as a `.jpg` file. Great for preserving exact layout.
- 📄 **PDF Mode**: Combines all captured images into a single, high-quality PDF.
- 📱 **PiP Background Hack**: A small Picture-in-Picture window opens to keep the browser process active even when the tab is not in focus.
- 🔄 **Toggle Button**: (Tampermonkey only) Easily show/hide the downloader UI without refreshing the page.
- 🚫 **No Premium Required**: Works on all publicly embeddable documents.

<br/>

---

## 🖨️ PDF Generation Settings

> For the best output quality:

| Setting | Value |
|:--------|:------|
| **PDF Library** | `jsPDF` (Auto-loaded) |
| **Parallel Downloads** | `4` (Bookmarklet / Console, adjustable in the panel) |
| **Retry Attempts** | `3 times` |

<br/>

---

## 📂 Project Structure

```bash
📦 Scribd-Downloader-js
 ┣ 📂 docs/images
 ┃ ┣ 🖼️ Downloader.PNG
 ┃ ┗ 🖼️ PIP.PNG
 ┣ 📜 LICENSE
 ┣ 📜 README.md
 ┣ 📜 scribd.user.js                # Tampermonkey Script
 ┣ 📜 Scribd Downloader.txt         # Console Script
 ┗ 📜 Scribd Downloader Bookmark.txt # Bookmarklet Script
```

<br/>

---

## ⚠️ Disclaimer

> [!CAUTION]
> **Legal Notice:** This tool is provided for **personal and educational purposes only**.

- 📚 **Respect Copyright:** Do not use this tool to download material you do not have rights to.
- 👤 **Responsibility:** You are solely responsible for your actions and compliance with Scribd's Terms of Service.
- 🚫 **No Liability:** The authors are not responsible for any misuse.

<br/>

---

<details>
<summary><h2>🔧 How It Works (For Developers)</h2></summary>

### 🎯 Core Concept

Scribd's content is often accessible via the `/embeds/` endpoint. This tool:
1.  **Extracts** the document ID from the URL.
2.  **Wraps** the content in a custom UI panel.
3.  **Automates Scrolling**: Triggers lazy-loading of all pages.
4.  **Captures Images**: Intercepts the `.absimg` elements from the DOM.
5.  **Generates PDF**: Uses `jsPDF` to stitch images into a single document.
6.  **Background Survival**: Uses a `canvas` + `video` stream in a PiP window to prevent the browser from throttling the script when the tab is hidden.

</details>

<br/>

---

<div align="center">

### ⭐ Star this repo if it helped you!

<br/>

[![GitHub](https://img.shields.io/badge/AllLiveSupport-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/AllLiveSupport)

</div>
