<div align="center">
  
# 📚 Scribd-Downloader-js

### 🚀 Download any document from Scribd as crisp PDF or Images — 100% Free!

<br/>

[![GitHub stars](https://img.shields.io/github/stars/AllLiveSupport/Scribd-Downloader-js?style=for-the-badge&logo=github&color=yellow)](https://github.com/AllLiveSupport/Scribd-Downloader-js/stargazers)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge&logo=opensourceinitiative&logoColor=white)](LICENSE)
[![User Script](https://img.shields.io/badge/User%20Script-v3.5%20Ultra-1abc9c?style=for-the-badge&logo=tampermonkey&logoColor=white)](scribd.user.js)

<br/>

<img src="https://img.shields.io/badge/Chrome-Supported-success?style=flat-square&logo=googlechrome&logoColor=white"/>
<img src="https://img.shields.io/badge/Firefox-Supported-success?style=flat-square&logo=firefox&logoColor=white"/>
<img src="https://img.shields.io/badge/Edge-Supported-success?style=flat-square&logo=microsoftedge&logoColor=white"/>
<img src="https://img.shields.io/badge/Smart%20Detection-Image%20vs%20DOCX-blueviolet?style=flat-square"/>
<img src="https://img.shields.io/badge/Full%20Bleed%20PDF-Per--Page%20Exact%20Size-brightgreen?style=flat-square"/>

---

**✨ Smart Engine • 🎯 Auto Book vs DOCX Detection • 📐 Full-Bleed Landscape/Portrait PDF • 🚀 Zero A4 Margin Clipping**

<br/><br/>

<img src="docs/images/Downloader.png" alt="Scribd Downloader Ultra v3.5" width="360" style="border-radius: 10px; box-shadow: 0 8px 30px rgba(0,0,0,0.5);"/>

<br/><br/>

### 🌐 Select Language / Dil Seçimi
[![English](https://img.shields.io/badge/Language-English-1abc9c?style=for-the-badge&logo=googlechrome&logoColor=white)](#-english-documentation)
[![Türkçe](https://img.shields.io/badge/Dil-Türkçe-e74c3c?style=for-the-badge)](#-türkçe-dokümantasyon)

</div>

<br/>

---

# 🇬🇧 English Documentation

<details open>
<summary><b>Click to collapse / expand English guide</b></summary>
<br/>

## ⚡ What's New in v3.5 ULTRA?

- 📚 **Default Books Mode (`AUTO PDF`)**: Each page is directly compiled into PDF via `jsPDF` using its **exact native pixel dimensions and orientation**. Zero forced A4 paper cropping, zero large white letterbox margins, and no browser print dialog required.
- 🧠 **Bulletproof Document Detection**: Automatically differentiates between **Scanned / Raster Books** (KPSS, textbooks, encyclopedias, novels) and **DOCX / Vector Documents** (Word files, nested HTML tables). Trims false-positive 1px border clips.
- 📐 **Dynamic Variable Landscape / Portrait Matching**: Wide / horizontal cover pages remain landscape, and interior portrait pages remain portrait—100% edge-to-edge full bleed.
- 📝 **On-Demand Vector Print for DOCX**: For Word/DOCX documents with vector fonts and complex table sprite sheets, switch to `VEKTÖR BASKI` with one click.
- 🔤 **Accurate Auto Filename**: Automatically locks `document.title` to the clean document name before saving (`${bookName}.pdf`).
- 🔓 **Automatic Paywall Unblur**: Strips Scribd paywall blurs automatically during page acquisition.

---

## 🎯 Three Installation Methods

| Method | Best For | Difficulty | Engine |
|:-------|:---------|:-----------|:-------|
| 🌐 **Tampermonkey** | Automatic launcher button, easiest (Recommended) | ⭐ Easy | **v3.5 ULTRA** |
| 💻 **Console** | Developers, one-off use via F12 | ⭐⭐ Medium | **v3.5 ULTRA** |
| 🔖 **Bookmarklet** | Quick execution without extensions | ⭐ Easy | **v3.5 ULTRA** |

---

### 🌐 Method 1: Tampermonkey (Recommended)

#### Step 1: Install Tampermonkey Extension

| Browser | Install Link |
|:-------:|:------------:|
| <img src="https://img.shields.io/badge/Chrome-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white"/> | [Install](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo) |
| <img src="https://img.shields.io/badge/Firefox-FF7139?style=for-the-badge&logo=firefox&logoColor=white"/> | [Install](https://addons.mozilla.org/en-US/firefox/addon/tampermonkey/) |
| <img src="https://img.shields.io/badge/Edge-0078D7?style=for-the-badge&logo=microsoftedge&logoColor=white"/> | [Install](https://microsoftedge.microsoft.com/addons/detail/tampermonkey/iikmkjmpaadaobahmlepeloendndfphd) |

#### Step 2: Install the Script

1. Open [**`scribd.user.js`**](scribd.user.js) in this repository.
2. Click the **"Raw"** button.
3. Tampermonkey will automatically detect the script and prompt to install. Click **"Install"**.

#### Step 3: Usage

1. 🌐 Navigate to any document on Scribd.
2. 📥 Click the floating green **"Download"** button at the bottom-right.
3. ⚡ If prompted, switch to **Content Mode** for the best unblurred resolution.
4. ⚙️ Mode defaults to **📚 AUTO PDF (Full Page / Books)**.
5. 🚀 Click **"START DOWNLOAD"**. The PDF will download directly with native page dimensions!

---

### 🔖 Method 2: Bookmarklet

1. **Create Bookmark**: Add a new bookmark to your browser bookmark bar.
2. **Name**: Set it to `Scribd Downloader`.
3. **URL**: Copy and paste everything from [**`Scribd Downloader Bookmark.txt`**](Scribd%20Downloader%20Bookmark.txt).
4. **Action**: Click the bookmark while viewing any Scribd document to launch the downloader panel.

---

### 💻 Method 3: Developer Console

1. **F12**: Open Developer Tools (`F12` or `Ctrl + Shift + I`) and switch to the **Console** tab.
2. **Paste**: Copy all code from [**`Scribd Downloader.txt`**](Scribd%20Downloader.txt).
3. **Enter**: Paste and press `Enter` to display the panel.

---

## 🛠️ Detailed Features

- 📄 **Full-Bleed PDF Mode**: Captures high-resolution pages and outputs a single PDF matching each page's exact pixel dimensions without white borders.
- 🖼️ **Image Mode**: Saves individual high-quality `.jpg` pages on demand.
- 🧠 **Hybrid Engine**: Direct fast-path for image-only books; clean vector mode for DOCX, Word, tables, and formula sheets.
- 📱 **PiP Background Survival**: PiP video canvas stream keeps the browser tab active when navigating to other tabs or windows.
- 🔓 **No Paywall Barrier**: Works on all embeddable Scribd content.

</details>

<br/>

---

# 🇹🇷 Türkçe Dokümantasyon

<details open>
<summary><b>Türkçe rehberi açmak / daraltmak için tıklayın</b></summary>
<br/>

## ⚡ v3.5 ULTRA ile Neler Yeni?

- 📚 **Varsayılan Kitaplar Modu (`AUTO PDF`)**: Her sayfa kendi orijinal boyutunda ve yönünde (kapak yatay, iç sayfalar dikey) A4 sınırı veya kenar boşluğu olmadan sıfır kayıpla direkt indirilir. Tarayıcı baskı penceresi açılmaz.
- 🧠 **Hatasız Belge Tespiti**: KPSS kitapları, taranmış romanlar ve sunumlar 1px kırpma sınırlarına takılmadan anında `📚 RESİMLİ KİTAP (Tam Sayfa)` olarak tanınır.
- 📐 **Dinamik Yatay/Dikey Eşleme**: Yatay kapaklar ve dikey sayfalar PDF içerisinde tam sayfa yerleşir, sayfa kenarlarında gereksiz beyaz şeritler kalmaz.
- 📝 **İsteğe Bağlı Vektör Baskı**: Gerçek Word/DOCX ve vektörel tablolu metinler için kullanıcı istediğinde tek tıkla `VEKTÖR BASKI` seçebilir.
- 🔤 **Otomatik Temiz Dosya Adı**: İndirilen PDF gerçek kitap adını alır (`document.title` kilitlenmesi).
- 🔓 **Otomatik Bulanıklık Kaldırma**: Sayfalar taranırken Scribd'in koyduğu paywall bulanıklıkları kendiliğinden temizlenir.

---

## 🎯 Üç Kolay Kullanım Yöntemi

| Yöntem | En Uygun | Zorluk | Motor |
|:-------|:---------|:-------|:------|
| 🌐 **Tampermonkey** | Otomatik başlatıcı buton, en kolayı (Önerilen) | ⭐ Kolay | **v3.5 ULTRA** |
| 💻 **Konsol** | Geliştiriciler, F12 üzerinden tek seferlik kullanım | ⭐⭐ Orta | **v3.5 ULTRA** |
| 🔖 **Yer İmi (Bookmarklet)** | Eklentisiz hızlı kullanım | ⭐ Kolay | **v3.5 ULTRA** |

---

### 🌐 Yöntem 1: Tampermonkey (Önerilen)

#### Adım 1: Tampermonkey Eklentisini Kurun

| Tarayıcı | Yükleme Bağlantısı |
|:-------:|:------------:|
| <img src="https://img.shields.io/badge/Chrome-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white"/> | [Yükle](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo) |
| <img src="https://img.shields.io/badge/Firefox-FF7139?style=for-the-badge&logo=firefox&logoColor=white"/> | [Yükle](https://addons.mozilla.org/en-US/firefox/addon/tampermonkey/) |
| <img src="https://img.shields.io/badge/Edge-0078D7?style=for-the-badge&logo=microsoftedge&logoColor=white"/> | [Yükle](https://microsoftedge.microsoft.com/addons/detail/tampermonkey/iikmkjmpaadaobahmlepeloendndfphd) |

#### Adım 2: Scripti Ekleyin

1. Bu repodaki [**`scribd.user.js`**](scribd.user.js) dosyasını açın.
2. **"Raw"** butonuna tıklayın.
3. Tampermonkey scripti otomatik olarak algılayıp yükleme ekranı getirecektir. **"Yükle"** (Install) butonuna tıklayın.

#### Adım 3: Kullanım

1. 🌐 Scribd üzerinde herhangi bir belgeye gidin.
2. 📥 Sağ altta beliren yeşil **"Download"** butonuna tıklayın.
3. ⚡ Eğer Content Mode aktif değilse **Content Mode**'a geçiş yapın.
4. ⚙️ Mod varsayılan olarak **📚 AUTO PDF (Tam Sayfa / Kitaplar)** seçilidir.
5. 🚀 **"START DOWNLOAD"** butonuna tıklayın. Belgeniz orijinal sayfa boyutlarıyla doğrudan inecektir!

---

### 🔖 Yöntem 2: Yer İmi (Bookmarklet)

1. **Yer İmi Oluşturun**: Tarayıcınızın yer imleri çubuğuna sağ tıklayıp yeni bir yer imi ekleyin.
2. **İsim**: `Scribd Downloader` yapın.
3. **URL**: [**`Scribd Downloader Bookmark.txt`**](Scribd%20Downloader%20Bookmark.txt) dosyasının tüm içeriğini kopyalayıp URL kutusuna yapıştırın.
4. **Çalıştırma**: Scribd belgesi açıkken bu yer imine tıklayın; indirme paneli hemen açılacaktır.

---

### 💻 Yöntem 3: Geliştirici Konsolu (F12)

1. **F12**: Geliştirici Araçlarını açın (`F12` veya `Ctrl + Shift + I`) ve **Console** sekmesine gelin.
2. **Kopyala**: [**`Scribd Downloader.txt`**](Scribd%20Downloader.txt) dosyasının tüm içeriğini kopyalayın.
3. **Yapıştır**: Konsola yapıştırıp `Enter` tuşuna basın.

---

## 🛠️ Detaylı Özellikler

- 📄 **Tam Sayfa PDF Modu**: Sayfaları orijinal piksel boyutunda yakalar ve kenar boşluğu olmadan tek bir PDF dosyası üretir.
- 🖼️ **Görsel Modu**: Tüm sayfaları orijinal yüksek çözünürlükte `.jpg` olarak tek tek kaydeder.
- 🧠 **Akıllı Hibrit Motor**: Taranmış kitaplar için hızlı ve doğrudan indirme; DOCX ve tablolu metinler için vektörel baskı.
- 📱 **PiP Arka Plan Desteği**: Resim İçinde Resim (PiP) video akışı sayesinde başka sekmeye geçseniz bile indirme duraksamaz.
- 🔓 **Önizleme / Paywall Sınırı Yok**: Scribd'de gömülebilen tüm sayfalarda engelsiz çalışır.

</details>

<br/>

---

## 📂 Project Structure

```bash
📦 Scribd-Downloader-js
 ┣ 📂 docs/images
 ┃ ┣ 🖼️ Downloader.png
 ┃ ┗ 🖼️ PIP.PNG
 ┣ 📜 LICENSE
 ┣ 📜 README.md
 ┣ 📜 scribd.user.js                 # Tampermonkey Userscript (v3.5 ULTRA)
 ┣ 📜 Scribd Downloader.txt          # Developer Console Script (v3.5 ULTRA)
 ┗ 📜 Scribd Downloader Bookmark.txt  # Bookmarklet Script (v3.5 ULTRA)
```

<br/>

---

## ⚠️ Disclaimer / Yasal Uyarı

> [!CAUTION]
> **Legal Notice:** This tool is provided for **personal, research, and educational backup purposes only**.
> - Respect copyright laws and original authors.
> - You are responsible for your own actions and adherence to Scribd's Terms of Service.
>
> **Yasal Uyarı:** Bu araç yalnızca **kişisel, araştırma ve eğitim amaçlı yedekleme** amacıyla sunulmuştur. Telif haklarına saygı gösteriniz.

---

<div align="center">

### ⭐ Star this repo if it helped you!

<br/>

[![GitHub](https://img.shields.io/badge/AllLiveSupport-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/AllLiveSupport)

</div>
