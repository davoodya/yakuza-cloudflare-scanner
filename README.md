<div align="center">

# 🧹 Yakuza Cloudflare Scanner

**ابزار پیدا کردن آی‌پی تمیز کلادفلر — مستقیم از مرورگر شما**
**Find Clean Cloudflare IPs — Directly From Your Browser**

[![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![License: MIT](https://img.shields.io/badge/License-MIT-10b981?style=flat-square)](LICENSE)
[![No Dependencies](https://img.shields.io/badge/Dependencies-Zero-a855f7?style=flat-square)]()

<br>

[🇬🇧 **Jump to English**](#-english) &nbsp;·&nbsp; [📖 **مشاهده‌ی مستندات کامل**](README-LONG.md)

</div>

---

<div dir="rtl">

## 🇮🇷 نسخه فارسی

**Yakuza Cloudflare Scanner** یک ابزار کاملاً **کلاینت‌ساید** برای پیدا کردن **آی‌پی‌های تمیز و کم‌تاخیر کلادفلر** است. مناسب برای ساخت کانفیگ V2Ray/Xray و بهبود کیفیت اتصال. بدون سرور، بدون ردیابی، بدون نصب.

---

### ✨ امکانات

- 🎯 **اسکن سریع** هزاران آی‌پی کلادفلر
- 🎛️ **فیلتر پیشرفته** — Regex، Include، Exclude
- 🌍 **دوزبانه** (فارسی / انگلیسی) با ذخیره‌سازی خودکار
- 📊 **نمایش زنده** پیشرفت و تاخیر
- 💾 **خروجی CSV و JSON**
- 📋 **کپی سریع** با یک کلیک
- 📱 **کاملاً ریسپانسیو**
- 🚫 **بدون وابستگی خارجی**

---

### 🚀 شروع سریع

**روش ۱ — ساده‌ترین:** فایل `index.html` را **Double Click** کنید. تمام!

**روش ۲ — وب‌سرور محلی:**

```bash
git clone https://github.com/davoodya/yakuza-cloudflare-scanner.git
cd yakuza-cloudflare-scanner
python -m http.server 8080
```
سپس باز کنید: http://localhost:8080

روش ۳ — با Node.js:
bash

npx serve .

🎮 روش استفاده

۱. VPN را خاموش کنید 🔌

۲. پارامترها را تنظیم کنید ⚙️
پارامتر	پیشنهادی
تعداد آی‌پی	5
تاخیر مجاز (ms)	500
Regex	خالی
Include	خالی
Exclude	خالی

۳. دکمه‌ی «شروع» را بزنید ◀️

۴. نتایج را کپی یا دانلود کنید 📥
🔍 نمونه فیلترها
regex

^104\.17\.          # فقط رنج 104.17
^104\.17\.|^141\.   # رنج‌های 104.17 و 141
8$                  # آی‌پی‌های پایانیافته با 8

🧠 چطور کار می‌کند؟

یک درخواست fetch سبک به هر آی‌پی زده می‌شود و زمان پاسخ اندازه‌گیری می‌شود. آی‌پی‌هایی که زیر حد مجاز باشند در جدول نتایج ذخیره می‌شوند.
📖 مستندات بیشتر

برای توضیحات کامل، سوالات پرتکرار، ساختار پروژه و راهنمای مشارکت:
<a href="README-LONG.md">
  <img src="https://img.shields.io/badge/📖_مشاهده‌ی_مستندات_کامل-3b82f6?style=for-the-badge" alt="Full Documentation" />
</a>
🧠 ساخته شده توسط داود یاحی

⬆️ بازگشت به بالا  ·  🇬🇧 English Version
</div></div><div id="english" dir="ltr">
🇬🇧 English Version

Yakuza Cloudflare Scanner is a fully client-side tool to find clean, low-latency Cloudflare IPs. Perfect for V2Ray/Xray configs and improving connection quality. No server, no tracking, no installation.
✨ Features

    🎯 Fast scanning of thousands of Cloudflare IPs

    🎛️ Advanced filtering — Regex, Include, Exclude

    🌍 Bilingual UI (Persian / English) with auto-save

    📊 Live progress and latency display

    💾 CSV & JSON export

    📋 One-click copy

    📱 Fully responsive

    🚫 Zero dependencies

🚀 Quick Start

Option 1 — Easiest: Just double-click index.html. Done!

Option 2 — Local web server:
bash

git clone https://github.com/davoodya/yakuza-cloudflare-scanner.git
cd yakuza-cloudflare-scanner
python -m http.server 8080

Then open: http://localhost:8080

Option 3 — With Node.js:
bash

npx serve .

🎮 How to Use

    Turn off your VPN 🔌

    Configure parameters ⚙️

Parameter	Default
No. of IPs	5
Max. Latency (ms)	500
Regex	empty
Include	empty
Exclude	empty

    Click "Start" ◀️

    Copy or download the results 📥

🔍 Filter Examples
regex

^104\.17\.          # Only 104.17 range
^104\.17\.|^141\.   # 104.17 and 141 ranges
8$                  # IPs ending with 8

🧠 How It Works

A lightweight fetch request is sent to each IP, and the response time is measured. IPs below the threshold are saved to the results table.
📖 Full Documentation

For complete details, FAQ, project structure, and contribution guide:
<a href="README-LONG.md"> <img src="https://img.shields.io/badge/📖_View_Full_Documentation-3b82f6?style=for-the-badge" alt="Full Documentation" /> </a><div align="center">
❤️ Made by Davood Yahay

⬆️ Back to top  ·  🇮🇷 نسخه فارسی
</div></div>