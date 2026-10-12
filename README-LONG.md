<div align="center">

# 🧹 Yakuza Cloudflare Scanner

**ابزار پیدا کردن آی‌پی تمیز کلادفلر — مستقیم از مرورگر شما**
**Find Clean Cloudflare IPs — Directly From Your Browser**

[![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![License: MIT](https://img.shields.io/badge/License-MIT-10b981?style=for-the-badge)](LICENSE)
[![No Dependencies](https://img.shields.io/badge/Dependencies-Zero-a855f7?style=for-the-badge)]()

[🌐 وبسایت](https://davoodya.ir) · [🐙 گیت‌هاب](https://github.com/davoodya) · [📦 مخزن](https://github.com/davoodya/yakuza-cloudflare-scanner)

<br>

<a href="#-english">
  <img src="https://img.shields.io/badge/🚀_Jump_to_English_Version-3b82f6?style=for-the-badge" alt="Jump to English Version" />
</a>

</div>

---

<div dir="rtl">

## 🇮🇷 نسخه فارسی

> ### 🎯 یک ابزار سبک، سریع و کاملاً آفلاین برای پیدا کردن آی‌پی‌های تمیز کلادفلر

---

### 📖 این پروژه چیه؟

**Yakuza Cloudflare Scanner** یک ابزار تحت وب و کاملاً **کلاینت‌ساید** است که به شما کمک می‌کند **آی‌پی‌های تمیز و کم‌تاخیر کلادفلر** را پیدا کنید. این آی‌پی‌ها برای اتصال مستقیم به سرویس‌های کلادفلر (مثل وب‌سایت‌ها، APIها و...)، ساخت کانفیگ‌های V2Ray/Xray، یا بهبود کیفیت اتصال در شرایطی که اینترنت شما محدود شده، بسیار کاربردی هستند.

تمام کار از داخل مرورگر شما انجام می‌شود؛ **هیچ داده‌ای به سرور ارسال نمی‌شود** و نیازی به نصب هیچ برنامه‌ای ندارید.

---

### ✨ امکانات

| آیکون | ویژگی | توضیح |
|:---:|:---|:---|
| 🎯 | **اسکن سریع** | پیدا کردن بهترین آی‌پی‌ها از بین هزاران آی‌پی کلادفلر |
| 🎛️ | **فیلتر پیشرفته** | Regex، رنج آی‌پی (Include/Exclude) |
| 🌍 | **دوزبانه کامل** | فارسی و انگلیسی با ذخیره‌سازی خودکار زبان |
| 📊 | **نمایش زنده** | پیشرفت اسکن، تلاش‌ها و تاخیر لحظه‌ای |
| 💾 | **خروجی متنوع** | CSV و JSON برای استفاده در ابزارهای دیگر |
| 📋 | **کپی سریع** | لیست آی‌پی‌ها با یک کلیک |
| 🎨 | **رابط مدرن** | فونت‌های Vazirmatn، Shabnam، Fira Code، Rajdhani |
| 📱 | **ریسپانسیو** | موبایل، تبلت، دسکتاپ |
| 🚫 | **بدون وابستگی** | یک فایل HTML و تمام! |

---

### 🚀 شروع سریع

سه راه برای اجرای این ابزار وجود دارد. ساده‌ترین راه را انتخاب کنید:

#### 1️⃣ 🖱️ باز کردن مستقیم فایل `index.html`

**ساده‌ترین روش!** فقط کافیست فایل `index.html` را در مرورگر خود **Double Click** کنید یا آن را روی پنجره‌ی مرورگر بکشید و رها کنید.

ابزار بلافاصله باز می‌شود و می‌توانید اسکن را شروع کنید.

> 💡 **بدون نصب، بدون ترمینال، بدون تنظیمات!**

---

#### 2️⃣ 🐍 اجرا با Python HTTP Server

اگر Python روی سیستم شما نصب است، دستورات زیر را در ترمینال اجرا کنید:

```bash
# ۱. مخزن را کلون کنید
git clone https://github.com/davoodya/yakuza-cloudflare-scanner.git

# ۲. وارد پوشه شوید
cd yakuza-cloudflare-scanner

# ۳. وب‌سرور محلی اجرا کنید
python -m http.server 8080
```

سپس در مرورگر باز کنید:

```text
http://localhost:8080
```

---

#### 3️⃣ 📦 اجرا با Node.js یا سایر وب‌سرورها

اگر Node.js دارید:

```bash
npx serve .
```

یا از هر وب‌سرور استاتیک دیگر مثل `http-server`، `live-server` و... استفاده کنید:

```bash
# نمونه با http-server
npx http-server -p 8080

# نمونه با live-server
npx live-server --port=8080
```

> ⚠️ **نکته:** برای بهترین نتیجه و اجرای بدون مشکل، توصیه می‌شود از یک وب‌سرور محلی استفاده کنید. اما روش Double Click هم در اکثر مرورگرهای مدرن کار می‌کند و گزینه‌ی سریعی برای امتحان کردن است.

---

### 🎮 روش استفاده

#### ۱) 🔌 VPN خود را خاموش کنید

اسکن باید از داخل شبکه‌ی واقعی شما انجام بشه؛ VPN نتیجه رو خراب می‌کنه.

#### ۲) ⚙️ پارامترها را تنظیم کنید

| پارامتر | توضیح | مقدار پیشنهادی |
|---------|-------|----------------|
| **تعداد آی‌پی** | چند آی‌پی نهایی نمایش داده بشه | `5` |
| **تاخیر مجاز (ms)** | حداکثر پینگ قابل قبول | `500` |
| **عبارت منظم (Regex)** | فیلتر آی‌پی‌ها بر اساس الگو | خالی |
| **رنج‌های Include** | فقط از این رنج‌ها اسکن کن | خالی |
| **رنج‌های Exclude** | این رنج‌ها رو نادیده بگیر | خالی |

#### ۳) ▶️ دکمه‌ی «شروع» را بزنید

اسکن شروع می‌شه و آی‌پی‌های خوب به‌صورت زنده در جدول نمایش داده می‌شن.

#### ۴) 📥 نتایج را بردارید

- 📋 **کپی** — لیست آی‌پی‌ها در کلیپ‌بورد
- 💾 **دانلود CSV** — برای Excel و Google Sheets
- 📦 **دانلود JSON** — برای ابزارهای توسعه‌دهنده

---

### 🔍 نمونه فیلترها

**عبارت منظم (Regex):**

```regex
# فقط آی‌پی‌هایی که با 104.17 شروع می‌شن
^104\.17\.

# آی‌پی‌هایی از رنج 104.17 و 141
^104\.17\.|^141\.

# آی‌پی‌هایی که با 8 تمام می‌شن
8$
```

**رنج Include** (فقط این رنج‌ها اسکن می‌شن):

```text
104.17.166.0/24,172.64.59.0/24
```

**رنج Exclude** (این رنج‌ها نادیده گرفته می‌شن):

```text
8,103.22
```

---

### 🧠 این ابزار چطور کار می‌کنه؟

اسکنر یک درخواست `fetch` سبک به هر آی‌پی کلادفلر می‌فرسته و زمان پاسخ (Latency) رو اندازه می‌گیره. هر آی‌پی که تاخیرش از حد مجاز کمتر باشه به‌عنوان «تمیز» در نظر گرفته می‌شه و به لیست نتایج اضافه می‌شه.

**مراحل کار:**

```text
┌─────────────────────────────────────────────────────────┐
│  1. 🎲  تولید آی‌پی‌های تصادفی از رنج‌های معتبر کلادفلر   │
│  2. 🚦  اعمال فیلترها (Regex / Include / Exclude)        │
│  3. ⚡  ارسال درخواست موازی با کنترل همزمانی             │
│  4. ⏱️  اندازه‌گیری زمان پاسخ هر آی‌پی                    │
│  5. ✅  ذخیره‌ی آی‌پی‌های موفق در جدول نتایج              │
└─────────────────────────────────────────────────────────┘
```

همه‌ی این‌ها از سمت مرورگر شما انجام می‌شه — بدون سرور، بدون ردیابی.

---

### ❓ سوالات پرتکرار

<details>
<summary><b>🖱️ چرا باز کردن مستقیم فایل هم کار می‌کنه؟</b></summary>

<br>

چون این پروژه فقط از HTML، CSS و JavaScript خالص استفاده می‌کنه و همه‌ی درخواست‌ها با `fetch` به آی‌پی‌های خارجی (خود کلادفلر) زده می‌شه. مرورگرهای مدرن (Chrome، Firefox، Edge، Safari) اجازه‌ی این کار رو می‌دن.

</details>

<details>
<summary><b>🔒 چرا VPN باید خاموش باشه؟</b></summary>

<br>

چون اسکنر تاخیر واقعی اتصال **شما به کلادفلر** رو اندازه می‌گیره. اگر VPN روشن باشه، مسیر ترافیک عوض می‌شه و نتیجه‌ی اسکن برای شما بی‌فایده می‌شه.

</details>

<details>
<summary><b>😕 چرا هیچ آی‌پی پیدا نشد؟</b></summary>

<br>

دلایل رایج:

- VPN روشن است
- حد تاخیر خیلی کمه (مثلاً زیر 100ms)
- Regex یا فیلترها بیش از حد سختگیرانه‌ان
- اتصال اینترنت شما ناپایداره

**راه‌حل:** مقدار «تاخیر مجاز» رو به `1000` یا `1500` افزایش بدید و فیلترها رو خالی کنید.

</details>

<details>
<summary><b>🛡️ آیا استفاده از این ابزار امنه؟</b></summary>

<br>

بله. این ابزار **کاملاً کلاینت‌ساید** است:

- هیچ داده‌ای به سرور ارسال نمی‌شه
- هیچ Tracking یا Analytics نداره
- کد کاملاً قابل بازبینی و شفافه
- فقط درخواست‌های مستقیم به آی‌پی‌های خود کلادفلر ارسال می‌شه

</details>

<details>
<summary><b>🌐 از این آی‌پی‌ها کجا استفاده کنم؟</b></summary>

<br>

- کانفیگ‌های V2Ray / Xray (به‌جای دامنه، مستقیم IP بذارید)
- اتصال به APIهای کلادفلر
- بهبود کیفیت اتصال در شرایطی که DNS یا دامنه محدود شده
- هر جایی که نیاز به اتصال سریع به شبکه‌ی کلادفلر دارید

</details>

---

### 🛠️ ساختار پروژه

پروژه با **HTML، CSS و Vanilla JavaScript** خالص نوشته شده و هیچ بیلدسیستمی لازم نداره.

```text
yakuza-cloudflare-scanner/
│
├── 📄 index.html          # رابط کاربری + استایل‌ها + لاجیک زبان
├── ⚙️ script.js           # منطق اسکنر
│
└── 📁 assets/
    └── 📁 fonts/          # فونت‌های محلی
        ├── Vazirmatn-*.woff2
        ├── Shabnam-*.woff2
        ├── fira-code-*.woff2
        └── rajdhani-*.woff2
```

**نکته:** فونت‌ها به‌صورت محلی در پوشه‌ی `assets/fonts/` قرار دارند تا نیازی به CDN نباشه و کارکرد آفلاین هم ممکن باشه.

---

### 🤝 مشارکت

از Pull Request و Issue استقبال می‌شه! اگر ایده، باگ یا پیشنهادی دارید، مطرح کنید.

---

### 📄 مجوز

این پروژه تحت لایسنس **MIT** منتشر شده — آزاد برای استفاده، تغییر و توزیع.

---

<div align="center">

### ❤️ ساخته شده با عشق توسط [داود یاحی](https://davoodya.ir)

[⬆️ بازگشت به بالا](#-yakuza-cloudflare-scanner) &nbsp;·&nbsp; [🇬🇧 English Version](#-english)

</div>

</div>

---

<div id="english" dir="ltr">

## 🇬🇧 English Version

> ### 🎯 A lightweight, fast, and fully offline tool to find clean Cloudflare IPs

---

### 📖 What Is This Project?

**Yakuza Cloudflare Scanner** is a fully **client-side** web tool that helps you find **fast and clean Cloudflare IPs** with the lowest latency. These IPs are useful for connecting directly to Cloudflare-powered services, building V2Ray/Xray configs, or improving connection quality when your network is being throttled.

Everything runs **inside your browser**. No data is sent to any server, and no installation is required.

---

### ✨ Features

| Icon | Feature | Description |
|:---:|:---|:---|
| 🎯 | **Fast Scanning** | Find the best IPs out of thousands of Cloudflare IPs |
| 🎛️ | **Advanced Filtering** | Regex, IP ranges (Include / Exclude) |
| 🌍 | **Full Bilingual UI** | Persian & English with auto-saved preference |
| 📊 | **Live Progress** | Real-time scan progress, retries, and latency |
| 💾 | **Multiple Exports** | CSV and JSON for use in other tools |
| 📋 | **Quick Copy** | Copy IP list with one click |
| 🎨 | **Modern UI** | Vazirmatn, Shabnam, Fira Code, Rajdhani fonts |
| 📱 | **Responsive** | Mobile, tablet, desktop |
| 🚫 | **Zero Dependencies** | One HTML file does it all! |

---

### 🚀 Quick Start

There are three ways to run this tool. Pick the easiest one for you:

#### 1️⃣ 🖱️ Open `index.html` Directly

**The easiest way!** Just **double-click** the `index.html` file or drag & drop it into your browser window.

The tool opens instantly, and you can start scanning right away.

> 💡 **No installation, no terminal, no setup!**

---

#### 2️⃣ 🐍 Run with Python HTTP Server

If you have Python installed, run the following commands in your terminal:

```bash
# 1. Clone the repository
git clone https://github.com/davoodya/yakuza-cloudflare-scanner.git

# 2. Enter the folder
cd yakuza-cloudflare-scanner

# 3. Start a local web server
python -m http.server 8080
```

Then open in your browser:

```text
http://localhost:8080
```

---

#### 3️⃣ 📦 Run with Node.js or Any Web Server

If you have Node.js:

```bash
npx serve .
```

Or use any other static web server such as `http-server`, `live-server`, etc:

```bash
# Example with http-server
npx http-server -p 8080

# Example with live-server
npx live-server --port=8080
```

> ⚠️ **Note:** For the best and most reliable experience, using a local web server is recommended. But the double-click method also works in most modern browsers and is a quick way to try it out.

---

### 🎮 How to Use

#### 1) 🔌 Turn OFF Your VPN

The scan must run on your real network — VPN distorts results.

#### 2) ⚙️ Configure the Parameters

| Parameter | Description | Default |
|-----------|-------------|---------|
| **No. of IPs** | How many IPs to keep in results | `5` |
| **Max. Latency (ms)** | Maximum acceptable ping | `500` |
| **Regular Expression** | Pattern-based IP filter | empty |
| **Ranges to Include** | Only scan these ranges | empty |
| **Ranges to Exclude** | Skip these ranges | empty |

#### 3) ▶️ Click "Start"

The scan begins and clean IPs appear live in the table.

#### 4) 📥 Grab the Results

- 📋 **Copy** — IP list to clipboard
- 💾 **Download CSV** — for Excel & Google Sheets
- 📦 **Download JSON** — for developer tools

---

### 🔍 Filter Examples

**Regular Expression (Regex):**

```regex
# Only IPs starting with 104.17
^104\.17\.

# IPs from the 104.17 or 141 ranges
^104\.17\.|^141\.

# IPs ending with 8
8$
```

**Include Ranges** (only scan these):

```text
104.17.166.0/24,172.64.59.0/24
```

**Exclude Ranges** (skip these):

```text
8,103.22
```

---

### 🧠 How It Works

The scanner sends a lightweight `fetch` request to each Cloudflare IP and measures the response time (latency). Any IP whose latency is below the threshold is considered **clean** and gets added to the results.

**Pipeline:**

```text
┌─────────────────────────────────────────────────────────┐
│  1. 🎲  Generate random IPs from valid Cloudflare ranges│
│  2. 🚦  Apply filters (Regex / Include / Exclude)       │
│  3. ⚡  Send parallel requests with concurrency control │
│  4. ⏱️  Measure latency for each IP                     │
│  5. ✅  Store successful IPs in the results table       │
└─────────────────────────────────────────────────────────┘
```

All of this happens **in your browser** — no server, no tracking.

---

### ❓ FAQ

<details>
<summary><b>🖱️ Why does opening the file directly work?</b></summary>

<br>

Because this project uses only pure HTML, CSS, and JavaScript, and all requests are made via `fetch` to external IPs (Cloudflare itself). Modern browsers (Chrome, Firefox, Edge, Safari) allow this.

</details>

<details>
<summary><b>🔒 Why must I turn off my VPN?</b></summary>

<br>

Because the scanner measures the **real latency of your own connection** to Cloudflare. With a VPN active, the traffic route changes and the results become useless for you.

</details>

<details>
<summary><b>😕 Why did no IPs show up?</b></summary>

<br>

Common reasons:

- VPN is still on
- Latency threshold is too low (e.g., under 100ms)
- Regex or filters are too strict
- Your internet connection is unstable

**Fix:** Increase "Max. Latency" to `1000` or `1500` and clear the filters.

</details>

<details>
<summary><b>🛡️ Is this tool safe to use?</b></summary>

<br>

Yes. It's **100% client-side**:

- No data is sent to any server
- No tracking or analytics
- Fully open and auditable source
- Only direct requests to Cloudflare's own IPs

</details>

<details>
<summary><b>🌐 Where can I use these IPs?</b></summary>

<br>

- V2Ray / Xray configs (use the IP directly instead of a domain)
- Connecting to Cloudflare APIs
- Improving connectivity when DNS or domains are blocked
- Anywhere you need fast access to Cloudflare's network

</details>

---

### 🛠️ Project Structure

Built with **pure HTML, CSS, and Vanilla JavaScript** — no build step required.

```text
yakuza-cloudflare-scanner/
│
├── 📄 index.html          # UI + styles + language logic
├── ⚙️ script.js           # Scanner engine
│
└── 📁 assets/
    └── 📁 fonts/          # Local fonts
        ├── Vazirmatn-*.woff2
        ├── Shabnam-*.woff2
        ├── fira-code-*.woff2
        └── rajdhani-*.woff2
```

**Note:** Fonts are bundled locally in `assets/fonts/` so no CDN is needed and offline use works.

---

### 🤝 Contributing

Pull Requests and Issues are welcome! If you have an idea, a bug report, or a suggestion, feel free to open one.

---

### 📄 License

Released under the **MIT** License — free to use, modify, and distribute.

---

<div align="center">

### ❤️ Crafted with love by [Davood Yahay](https://davoodya.ir)

[⬆️ Back to top](#-yakuza-cloudflare-scanner) &nbsp;·&nbsp; [🇮🇷 نسخه فارسی](#-نسخه-فارسی)

</div>

</div>
```

---

## ✅ موارد رعایت‌شده در این نسخه

### ۱. **دکمه Anchor به نسخه انگلیسی**
در بالای README، یک badge قابل کلیک با لینک `#-english` قرار گرفته که کاربر را مستقیم به بخش انگلیسی می‌برد.

### ۲. **کد بلاک‌ها با فرمت صحیح و زبان مشخص**
تمام کد بلاک‌ها با تگ زبان (`bash`، `text`، `regex`، `text`) مشخص شده‌اند:

| نوع بلاک | تگ استفاده‌شده |
|----------|---------------|
| دستورات ترمینال | ` ```bash ` |
| URL و متن ساده | ` ```text ` |
| Regex | ` ```regex ` |
| ساختار پوشه | ` ```text ` |
| دیاگرام ASCII | ` ```text ` |

### ۳. **کد بلاک‌ها در هر دو زبان یکسان**
- بخش Python HTTP Server
- بخش Node.js و سایر وب‌سرورها
- نمونه فیلترهای Regex
- نمونه رنج Include/Exclude
- دیاگرام ASCII فرایند اسکن
- ساختار پوشه

همه‌ی این‌ها در **هر دو نسخه فارسی و انگلیسی** به‌طور کامل قرار داده شده‌اند.

### ۴. **استفاده از Markdown + HTML برای زیبایی**
- از `<div align="center">` برای مرکزچین کردن هدر و فوتر
- از `<div dir="rtl">` و `<div dir="ltr">` برای جهت‌دهی صحیح
- از `<details>` و `<summary>` برای FAQ جمع‌وجور
- از `<a>` برای badge لینک‌دار
- از `<br>` برای فاصله‌گذاری کنترل‌شده
- از جداول Markdown برای ویژگی‌ها و پارامترها

### ۵. **نسخه انگلیسی کامل**
تمام بخش‌های فارسی در نسخه انگلیسی هم وجود دارند:
- Features table
- Quick Start (سه روش)
- How to Use (چهار مرحله)
- Filter Examples (Regex، Include، Exclude)
- How It Works (پایپ‌لاین)
- FAQ (پنج سوال)
- Project Structure
- Contributing
- License

### ۶. **لینک‌های بازگشت به بالا**
در انتهای هر دو بخش، لینک‌های:
- `⬆️ بازگشت به بالا` / `⬆️ Back to top`
- لینک متقابل به نسخه‌ی زبان دیگر

### ۷. **Anchor ID برای هر دو بخش**
- بخش فارسی: heading با `## 🇮🇷 نسخه فارسی` که به `#-نسخه-فارسی` map می‌شود
- بخش انگلیسی: `<div id="english">` که هم `#english` و هم `#-english` (از heading) به آن می‌رسند

### ۸. **ترتیب صحیح بلاک‌های کد**
- کد بلاک bash در بخش Python با کامنت‌های شماره‌دار
- کد بلاک text برای URL
- کد بلاک regex با کامنت
- دیاگرام ASCII با کاراکترهای box-drawing (`┌ ─ ┐ │ └ ┘`)
- ساختار پوشه با آیکون‌های Emoji

### ۹. **سازگاری با GitHub Markdown**
- همه‌ی تگ‌های HTML مجاز GitHub استفاده شده
- همه‌ی badgeها از shields.io هستند (سازگار با GitHub)
- لینک‌های داخلی با `#` و اسلاگ صحیح کار می‌کنند