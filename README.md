 <div align="center">

# 🧹 Yakuza Cloudflare Scanner

**ابزار پیدا کردن IPهای تمیز Cloudflare با کمترین تأخیر**  
**Find Clean Cloudflare IPs with Low Latency**

<p>
  <a href="https://github.com/davoodya/yakuza-cloudflare-scanner"><img src="https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge&logo=github" alt="GitHub Repository"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-10b981?style=for-the-badge" alt="MIT License"></a>
  <img src="https://img.shields.io/badge/Dependencies-Zero-a855f7?style=for-the-badge" alt="Zero Dependencies">
  <img src="https://img.shields.io/badge/HTML5-CSS3-JavaScript-blue?style=for-the-badge" alt="HTML CSS JavaScript">
</p>

<p>
  <a href="https://davoodya.ir">🌐 Website</a> ·
  <a href="https://github.com/davoodya">🐙 GitHub Profile</a> ·
  <a href="https://github.com/davoodya/yakuza-cloudflare-scanner">📦 Source Code</a>
</p>

<p>
  <a href="#english"><img src="https://img.shields.io/badge/🚀_Jump_to_English-2563eb?style=for-the-badge" alt="Jump to English"></a>
</p>

</div>

---

<div dir="rtl">

## 🇮🇷 نسخه فارسی

> ابزاری سبک، بدون نیاز به نصب و مبتنی بر مرورگر برای بررسی IPهای Cloudflare و شناسایی IPهای دارای تأخیر کمتر.

### 📖 معرفی

**Yakuza Cloudflare Scanner** یک ابزار تحت وب برای اسکن IPهای Cloudflare، اندازه‌گیری زمان پاسخ و فیلتر کردن نتایج بر اساس معیارهای دلخواه است.

این ابزار با HTML، CSS و JavaScript ساخته شده و برای اجرا به Node.js، فریم‌ورک یا فرایند Build نیاز ندارد. درخواست‌های اسکن از مرورگر کاربر ارسال می‌شوند.

**کاربردها:**
- بررسی تأخیر اتصال به IPهای Cloudflare
- فیلتر کردن نتایج با Regex و محدوده‌های IP
- خروجی گرفتن برای استفاده در ابزارهای دیگر
- بررسی IPهای مناسب برای سناریوهای شبکه و پیکربندی‌های V2Ray/Xray

> **نکته:** کم بودن تأخیر به‌تنهایی به معنی سالم بودن IP، دسترسی تضمین‌شده به یک سرویس یا مناسب بودن آن برای تمام پروتکل‌ها نیست. نتیجه به شبکه، مرورگر و مقصد درخواست وابسته است.

### ✨ امکانات

| ویژگی | توضیحات |
|:--|:--|
| ⚡ اسکن IP | بررسی IPها و اندازه‌گیری زمان پاسخ |
| 🎛️ فیلترهای پیشرفته | پشتیبانی از Regex و محدوده‌های Include/Exclude |
| 🌐 رابط دوزبانه | زبان فارسی و انگلیسی |
| 📊 نمایش زنده | مشاهده پیشرفت اسکن و نتایج |
| 📋 کپی سریع | کپی فهرست IPها |
| 💾 خروجی گرفتن | دانلود نتایج در قالب CSV و JSON |
| 📱 طراحی واکنش‌گرا | مناسب دسکتاپ، تبلت و موبایل |
| 📦 بدون وابستگی | بدون نصب پکیج یا Build |

### 🚀 شروع سریع

#### روش اول: اجرای مستقیم

1. مخزن را از GitHub دریافت یا Clone کنید.
2. فایل `index.html` را در مرورگر باز کنید.
3. پارامترها را تنظیم کرده و اسکن را شروع کنید.

<a href="https://github.com/davoodya/yakuza-cloudflare-scanner/archive/refs/heads/main.zip"><img src="https://img.shields.io/badge/⬇️_Download-Source_Code-2563eb?style=for-the-badge" alt="Download Source Code"></a>

#### روش دوم: اجرا با Python

ابتدا مخزن را Clone کنید و سپس وب‌سرور محلی را اجرا کنید:

```bash
git clone https://github.com/davoodya/yakuza-cloudflare-scanner.git
cd yakuza-cloudflare-scanner
python -m http.server 8080
```

اکنون آدرس زیر را در مرورگر باز کنید:

```text
http://localhost:8080
```

برای توقف وب‌سرور، در ترمینال `Ctrl+C` را فشار دهید.

#### روش سوم: اجرا با Node.js

اگر Node.js و npm در دسترس هستند، از یکی از دستورهای زیر استفاده کنید:

```bash
npx serve .
```

یا:

```bash
npx http-server -p 8080
```

آدرس محلی نمایش‌داده‌شده در ترمینال را در مرورگر باز کنید.

> **توصیه:** استفاده از وب‌سرور محلی روش پیشنهادی است؛ زیرا رفتار درخواست‌های شبکه ممکن است هنگام اجرای مستقیم فایل با `file://` در مرورگرهای مختلف متفاوت باشد.

### 🎮 راهنمای استفاده

**۱. اتصال شبکه را آماده کنید.**

اگر می‌خواهید تأخیر مسیر اتصال مستقیم خود را اندازه بگیرید، VPN یا Proxy را غیرفعال کنید. در غیر این صورت، نتایج مربوط به مسیر شبکه‌ای خواهند بود که از آن استفاده می‌کنید.

**۲. پارامترهای اسکن را تنظیم کنید.**

| پارامتر | توضیحات | مقدار پیشنهادی اولیه |
|:--|:--|:--|
| تعداد IPها | تعداد نتایج موردنظر | `5` |
| حداکثر تأخیر (ms) | آستانه پذیرش زمان پاسخ | `500` |
| Regex | الگوی فیلتر IPها | خالی |
| Include Ranges | محدوده‌های مجاز برای بررسی | خالی |
| Exclude Ranges | محدوده‌های حذف‌شده از بررسی | خالی |

**۳. اسکن را شروع کنید.**

روی دکمه شروع اسکن کلیک کنید. نتایج با توجه به عملکرد ابزار و معیارهای انتخاب‌شده نمایش داده می‌شوند.

**۴. نتایج را ذخیره کنید.**

- 📋 **Copy:** کپی کردن فهرست IPها
- 💾 **CSV:** مناسب Excel و Google Sheets
- 📦 **JSON:** مناسب پردازش و استفاده در اسکریپت‌ها

### 🔍 نمونه فیلترها

#### فیلتر Regex

فقط IPهایی که با `104.17` شروع می‌شوند:

```regex
^104\.17\.
```

IPهایی که با `104.17` یا `141` شروع می‌شوند:

```regex
^104\.17\.|^141\.
```

IPهایی که به عدد `8` ختم می‌شوند:

```regex
8$
```

> در Regex، نقطه `.` یک کاراکتر خاص است؛ برای تطبیق نقطه واقعی در IP از `\.` استفاده کنید.

#### محدوده Include

نمونه محدوده‌هایی که می‌خواهید بررسی شوند:

```text
104.17.166.0/24,172.64.59.0/24
```

#### محدوده Exclude

نمونه مقادیر برای حذف:

```text
8,103.22
```

> **توجه:** رفتار دقیق فیلترها به پیاده‌سازی برنامه بستگی دارد. نمونه‌های بالا باید مطابق قالب ورودی پذیرفته‌شده در رابط کاربری استفاده شوند؛ مقادیر Exclude لزوماً معادل CIDR معتبر نیستند.

### 🧠 نحوه عملکرد

فرایند کلی اسکن به این صورت است:

```text
Generate IP candidates
        ↓
Apply configured filters
        ↓
Send browser-based requests
        ↓
Measure response time
        ↓
Filter and display results
        ↓
Export or copy selected IPs
```

اندازه‌گیری زمان پاسخ در مرورگر انجام می‌شود. نتیجه ممکن است تحت تأثیر DNS، اتصال شبکه، محدودیت‌های مرورگر، CORS، Timeout و دسترسی‌پذیری مقصد قرار بگیرد؛ بنابراین زمان اندازه‌گیری‌شده الزاماً معادل Ping شبکه‌ای ICMP نیست.

### ❓ پرسش‌های متداول

<details>
<summary><strong>آیا برای اجرای ابزار به نصب وابستگی نیاز دارم؟</strong></summary>

خیر. پروژه به ابزار Build یا پکیج‌های زمان اجرای اضافی نیاز ندارد. برای اجرای مطمئن‌تر، استفاده از Python HTTP Server یا یک وب‌سرور استاتیک توصیه می‌شود.

</details>

<details>
<summary><strong>چرا هیچ IPای پیدا نمی‌شود؟</strong></summary>

دلایل احتمالی عبارت‌اند از:

- آستانه تأخیر بیش از حد پایین است.
- فیلترهای Regex یا Include/Exclude بیش از حد محدودکننده هستند.
- درخواست‌ها به دلیل CORS، Timeout یا محدودیت شبکه شکست می‌خورند.
- اتصال اینترنت ناپایدار است یا مقصدها پاسخ نمی‌دهند.

**راهکار:** فیلترها را موقتاً پاک کنید، آستانه تأخیر را افزایش دهید و با وب‌سرور محلی دوباره امتحان کنید.

</details>

<details>
<summary><strong>آیا خاموش کردن VPN الزامی است؟</strong></summary>

خیر؛ این موضوع به هدف شما بستگی دارد. اگر می‌خواهید مسیر مستقیم اینترنت خود را بررسی کنید، VPN را خاموش کنید. اگر می‌خواهید مسیر VPN را ارزیابی کنید، اسکن را با همان VPN انجام دهید.

</details>

<details>
<summary><strong>آیا این ابزار داده‌های من را ارسال می‌کند؟</strong></summary>

اسکن از سمت مرورگر انجام می‌شود. برای بررسی دقیق حریم خصوصی، کد منبع و درخواست‌های شبکه را بازبینی کنید. درخواست‌های اسکن به مقصدهای شبکه ارسال می‌شوند؛ بنابراین نباید آن را به معنای نبود هرگونه ترافیک شبکه دانست.

</details>

<details>
<summary><strong>آیا IPهای پیدا‌شده برای V2Ray/Xray مناسب هستند؟</strong></summary>

ممکن است در برخی پیکربندی‌ها قابل استفاده باشند، اما نتیجه اسکن به‌تنهایی سازگاری IP با پروتکل، پورت، TLS، SNI یا مقصد موردنظر را تضمین نمی‌کند. IP را در سناریوی واقعی خود آزمایش کنید.

</details>

### 🗂️ ساختار پروژه

```text
yakuza-cloudflare-scanner/
├── index.html
├── script.js
└── assets/
    └── fonts/
        ├── Vazirmatn-*.woff2
        ├── Shabnam-*.woff2
        ├── fira-code-*.woff2
        └── rajdhani-*.woff2
```

- `index.html`: رابط کاربری، استایل‌ها و اجزای صفحه
- `script.js`: منطق اسکن و پردازش نتایج
- `assets/fonts/`: فایل‌های فونت محلی

### 🤝 مشارکت

برای گزارش باگ، پیشنهاد قابلیت جدید یا مشارکت در توسعه، از بخش Issues و Pull Requests مخزن استفاده کنید.

<a href="https://github.com/davoodya/yakuza-cloudflare-scanner/issues"><img src="https://img.shields.io/badge/Report_a_Bug-Issues-dc2626?style=for-the-badge&logo=github" alt="Report a Bug"></a>
<a href="https://github.com/davoodya/yakuza-cloudflare-scanner/pulls"><img src="https://img.shields.io/badge/Contribute-Pull_Requests-16a34a?style=for-the-badge&logo=github" alt="Contribute"></a>

### 📄 مجوز

این پروژه تحت مجوز [MIT](LICENSE) منتشر شده است. برای جزئیات استفاده، تغییر و توزیع، فایل مجوز مخزن را مطالعه کنید.

</div>

### ساخته شده با 🧠 توسط [داوود یاحی - Davood Yahay](https://davoodya.ir)

---

<div id="english" dir="ltr">

## 🇬🇧 English Version

> A lightweight, browser-based tool for scanning Cloudflare IPs, measuring response latency, and filtering results.

### 📖 Overview

**Yakuza Cloudflare Scanner** is a web-based utility for evaluating Cloudflare IP addresses and identifying endpoints with lower measured response times.

Built with HTML, CSS, and JavaScript, it requires no framework, package installation, or build process. Scanning requests are initiated by the user's browser.

**Use cases:**
- Measuring response latency to Cloudflare IPs
- Filtering results with regular expressions and IP ranges
- Exporting results for other tools
- Evaluating IPs for networking and V2Ray/Xray configurations

> **Note:** Low latency alone does not guarantee that an IP is healthy, accessible to a particular service, or suitable for every protocol. Results depend on your network, browser, and request destination.

### ✨ Features

| Feature | Description |
|:--|:--|
| ⚡ IP Scanning | Evaluate IP addresses and measure response time |
| 🎛️ Advanced Filters | Regex and Include/Exclude IP ranges |
| 🌐 Bilingual UI | Persian and English |
| 📊 Live Results | View scan progress and results |
| 📋 Quick Copy | Copy IP lists |
| 💾 Export Options | Download results as CSV or JSON |
| 📱 Responsive Design | Desktop, tablet, and mobile |
| 📦 Zero Dependencies | No package installation or build step |

### 🚀 Quick Start

#### Option 1: Open the HTML File

1. Download or clone the repository.
2. Open `index.html` in your browser.
3. Configure the parameters and start scanning.

<a href="https://github.com/davoodya/yakuza-cloudflare-scanner/archive/refs/heads/main.zip"><img src="https://img.shields.io/badge/⬇️_Download-Source_Code-2563eb?style=for-the-badge" alt="Download Source Code"></a>

#### Option 2: Run with Python

Clone the repository and start a local HTTP server:

```bash
git clone https://github.com/davoodya/yakuza-cloudflare-scanner.git
cd yakuza-cloudflare-scanner
python -m http.server 8080
```

Open the following URL in your browser:

```text
http://localhost:8080
```

Press `Ctrl+C` in the terminal to stop the server.

#### Option 3: Run with Node.js

If Node.js and npm are available, run:

```bash
npx serve .
```

Alternatively:

```bash
npx http-server -p 8080
```

Open the local URL printed in the terminal.

> **Recommendation:** Using a local HTTP server is the preferred approach because browser behavior for network requests can vary when an HTML file is opened directly via `file://`.

### 🎮 How to Use

**1. Prepare your network.**

Disable your VPN or proxy if you want to measure latency over your direct connection. Otherwise, results reflect the network route currently in use.

**2. Configure the parameters.**

| Parameter | Description | Suggested Initial Value |
|:--|:--|:--|
| Number of IPs | Number of desired results | `5` |
| Maximum Latency (ms) | Maximum acceptable response time | `500` |
| Regex | Pattern-based IP filter | Empty |
| Include Ranges | Ranges to include in the scan | Empty |
| Exclude Ranges | Ranges to skip | Empty |

**3. Start scanning.**

Click the Start button. Results are displayed according to the application's behavior and your configured filters.

**4. Export your results.**

- 📋 **Copy:** Copy the IP list
- 💾 **CSV:** For Excel and Google Sheets
- 📦 **JSON:** For scripts and developer tools

### 🔍 Filter Examples

#### Regular Expressions

Match IPs starting with `104.17`:

```regex
^104\.17\.
```

Match IPs starting with `104.17` or `141`:

```regex
^104\.17\.|^141\.
```

Match IPs ending with the digit `8`:

```regex
8$
```

> In regular expressions, `.` is a special character. Use `\.` to match a literal dot in an IP address.

#### Include Ranges

Example ranges to include:

```text
104.17.166.0/24,172.64.59.0/24
```

#### Exclude Ranges

Example exclusion values:

```text
8,103.22
```

> **Note:** Exact filter behavior depends on the application's implementation. Use values compatible with the input format accepted by the UI; Exclude entries are not necessarily valid CIDR ranges.

### 🧠 How It Works

The general scanning pipeline is:

```text
Generate IP candidates
        ↓
Apply configured filters
        ↓
Send browser-based requests
        ↓
Measure response time
        ↓
Filter and display results
        ↓
Export or copy selected IPs
```

Latency measurements run in the browser. Results may be affected by DNS, network connectivity, browser restrictions, CORS, timeouts, and destination availability. The measured response time is therefore not necessarily equivalent to an ICMP ping.

### ❓ FAQ

<details>
<summary><strong>Do I need to install any dependencies?</strong></summary>

No. The project does not require a build tool or additional runtime packages. For more reliable execution, use Python's HTTP server or another static web server.

</details>

<details>
<summary><strong>Why are no IPs found?</strong></summary>

Possible causes include:

- The latency threshold is too low.
- Regex or Include/Exclude filters are too restrictive.
- Requests fail because of CORS, timeouts, or network restrictions.
- Your connection is unstable or the destinations are unavailable.

**Fix:** Clear the filters, increase the latency threshold, and retry using a local HTTP server.

</details>

<details>
<summary><strong>Must I disable my VPN?</strong></summary>

No. It depends on what you want to measure. Disable your VPN to evaluate your direct internet route, or keep it enabled if you want to evaluate the VPN route.

</details>

<details>
<summary><strong>Does this tool send my data to a server?</strong></summary>

Scanning requests originate from your browser. Review the source code and browser network activity to verify the implementation. Scanning does generate network traffic to destination IPs, so client-side execution does not mean that no network communication occurs.

</details>

<details>
<summary><strong>Are the discovered IPs suitable for V2Ray/Xray?</strong></summary>

They may be usable in some configurations, but scan results alone cannot guarantee compatibility with your protocol, port, TLS settings, SNI, or target service. Test each IP in your actual configuration.

</details>

### 🗂️ Project Structure

```text
yakuza-cloudflare-scanner/
├── index.html
├── script.js
└── assets/
    └── fonts/
        ├── Vazirmatn-*.woff2
        ├── Shabnam-*.woff2
        ├── fira-code-*.woff2
        └── rajdhani-*.woff2
```

- `index.html`: User interface, styles, and page components
- `script.js`: Scanning logic and result processing
- `assets/fonts/`: Local font files

### 🤝 Contributing

Bug reports, feature suggestions, and pull requests are welcome. Use the repository's Issues and Pull Requests sections to participate.

<a href="https://github.com/davoodya/yakuza-cloudflare-scanner/issues"><img src="https://img.shields.io/badge/Report_a_Bug-Issues-dc2626?style=for-the-badge&logo=github" alt="Report a Bug"></a>
<a href="https://github.com/davoodya/yakuza-cloudflare-scanner/pulls"><img src="https://img.shields.io/badge/Contribute-Pull_Requests-16a34a?style=for-the-badge&logo=github" alt="Contribute"></a>

### 📄 License

Released under the [MIT License](LICENSE). Refer to the repository's license file for the terms of use, modification, and distribution.

</div>

---

<div align="center">

### Created by 🧠 [Davood Yahay](https://davoodya.ir)

<p>
  <a href="#-yakuza-cloudflare-scanner">⬆️ Back to Top</a> ·
  <a href="#-نسخه-فارسی">🇮🇷 نسخه فارسی</a> ·
  <a href="#english">🇬🇧 English</a>
</p>

</div>