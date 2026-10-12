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

[**🇮🇷 فارسی**](#-فارسی) &nbsp;·&nbsp; [**🇬🇧 English**](#-english)

<br>

<a href="#-english">
  <img src="https://img.shields.io/badge/🚀_Jump_to_English_Version-3b82f6?style=for-the-badge" alt="Jump to English" />
</a>

</div>

---

<div dir="rtl">

## 🇮🇷 فارسی

> ### 🎯 یک ابزار سبک، سریع و کاملاً آفلاین برای پیدا کردن آی‌پی‌های تمیز کلادفلر

---

### 📖 این پروژه چیه؟

**Yakuza Cloudflare Scanner** یک ابزار تحت وب و کاملاً **کلاینت‌ساید** است که به شما کمک می‌کند **آی‌پی‌های تمیز و کم‌تاخیر کلادفلر** را پیدا کنید. این آی‌پی‌ها برای اتصال مستقیم به سرویس‌های کلادفلر (مثل وب‌سایت‌ها، APIها و...)، ساخت کانفیگ‌های V2Ray/Xray، یا بهبود کیفیت اتصال در شرایطی که اینترنت شما محدود شده، بسیار کاربردی هستند.

تمام کار از داخل مرورگر شما انجام می‌شود؛ **هیچ داده‌ای به سرور ارسال نمی‌شود** و نیازی به نصب هیچ برنامه‌ای ندارید.

<br>

### ✨ امکانات

| | ویژگی | توضیح |
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

<br>

### 🚀 شروع سریع

سه راه برای اجرای این ابزار وجود دارد. ساده‌ترین راه را انتخاب کنید:

<table>
<tr>
<td width="70" align="center">

### 1️⃣

</td>
<td>

#### 🖱️ باز کردن مستقیم فایل `index.html`

**ساده‌ترین روش!** فقط کافیست فایل `index.html` را در مرورگر خود **Double Click** کنید یا آن را روی پنجره‌ی مرورگر بکشید و رها کنید.

ابزار بلافاصله باز می‌شود و می‌توانید اسکن را شروع کنید.

> 💡 **بدون نصب، بدون ترمینال، بدون تنظیمات!**

</td>
</tr>
<tr>
<td align="center">

### 2️⃣

</td>
<td>

#### 🐍 اجرا با Python HTTP Server

اگر Python روی سیستم شما نصب است:

```bash
# ۱. مخزن را کلون کنید
git clone https://github.com/davoodya/yakuza-cloudflare-scanner.git

# ۲. وارد پوشه شوید
cd yakuza-cloudflare-scanner

# ۳. وب‌سرور محلی اجرا کنید
python -m http.server 8080