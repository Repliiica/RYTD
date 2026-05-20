# 📘 راهنمای کامل پیاده‌سازی روی GitHub

این فایل به شما کمک می‌کند پروژه را قدم به قدم روی گیت‌هاب آپلود و فعال کنید.

---

## 🎯 مرحله ۱: ساخت ریپوزیتوری در گیت‌هاب

1. به [github.com](https://github.com) بروید و وارد حساب خود شوید
2. روی دکمه سبز **"New"** یا **"+"** بالا سمت راست کلیک کنید
3. تنظیمات زیر را وارد کنید:
   - **Repository name:** `youtube-to-drive`
   - **Description:** `🎬 Download YouTube videos directly to Google Drive via Colab`
   - **Visibility:** Public (تا بقیه هم بتونن استفاده کنن)
   - ✅ تیک **Add a README file** را بزنید (موقتی، بعداً جایگزین می‌شود)
   - **License:** MIT License
4. روی **"Create repository"** کلیک کنید

---

## 🎯 مرحله ۲: آپلود فایل‌ها

### روش الف: از طریق رابط وب گیت‌هاب (ساده‌ترین روش)

1. در صفحه ریپوزیتوری، روی **"Add file" > "Upload files"** کلیک کنید
2. این فایل‌ها را drag & drop کنید:
   - `YouTube_to_Drive.ipynb`
   - `README.md` (روی فایل قبلی overwrite می‌شه)
   - `LICENSE` (روی فایل قبلی overwrite می‌شه)
   - `DISCLAIMER.md`
   - `.gitignore`
3. در پایین صفحه، پیام commit بنویسید: `Initial commit`
4. روی **"Commit changes"** کلیک کنید

### روش ب: از طریق Git (برای کاربران حرفه‌ای)

```bash
# 1. ریپوزیتوری را کلون کنید
git clone https://github.com/replica/youtube-to-drive.git
cd youtube-to-drive

# 2. فایل‌ها را در این پوشه قرار دهید

# 3. کامیت و پوش کنید
git add .
git commit -m "Initial commit"
git push origin main
```

---

## 🎯 مرحله ۳: فعال‌سازی Open in Colab

بعد از آپلود فایل‌ها، دکمه **"Open in Colab"** که در README قرار داره خودکار کار می‌کنه. کاربر با کلیک روی اون، نوت‌بوک شما رو در Colab باز می‌کنه.

لینک Colab به این صورت ساخته می‌شه:
```
https://colab.research.google.com/github/replica/youtube-to-drive/blob/main/YouTube_to_Drive.ipynb
```

---

## 🎯 مرحله ۴: تنظیمات اضافی (اختیاری اما توصیه می‌شه)

### الف) اضافه کردن Topics به ریپوزیتوری

در صفحه ریپو، کنار قسمت About روی چرخ‌دنده ⚙️ کلیک کنید و این topic ها رو اضافه کنید:

```
youtube-downloader, google-colab, google-drive, yt-dlp,
python, jupyter-notebook, video-downloader, mp3-downloader
```

این کار باعث می‌شه پروژه شما در سرچ‌ها بهتر دیده بشه.

### ب) اضافه کردن توضیحات و وب‌سایت

- **Description:** `🎬 Download YouTube videos directly to Google Drive via Colab — No setup required!`
- **Website:** لینک Colab یا اگر بعداً سایت داشتید

### ج) فعال‌سازی Issues و Discussions

در `Settings > Features`:
- ✅ Issues (برای گزارش باگ)
- ✅ Discussions (برای پرسش و پاسخ)

---

## 🎯 مرحله ۵: تست نهایی

1. لینک ریپو خود را در یک مرورگر دیگه (یا حالت ناشناس) باز کنید
2. روی دکمه **"Open in Colab"** کلیک کنید
3. نوت‌بوک باید در Colab باز شه
4. کل فرآیند رو تست کنید تا مطمئن بشید همه چی درست کار می‌کنه

---

## 🎯 مرحله ۶: تبلیغ پروژه (اختیاری)

برای اینکه پروژه‌تون دیده بشه:

- در [Reddit](https://reddit.com/r/learnpython) معرفی کنید
- در توییتر/ایکس با هشتگ‌های `#opensource #python` پست کنید
- در گروه‌های تلگرامی برنامه‌نویسی به اشتراک بگذارید
- لینک پروژه را در LinkedIn قرار دهید

---

## 📁 ساختار نهایی پروژه

```
youtube-to-drive/
├── YouTube_to_Drive.ipynb    # نوت‌بوک اصلی Colab
├── README.md                  # توضیحات پروژه (دوزبانه)
├── LICENSE                    # مجوز MIT
├── DISCLAIMER.md              # سلب مسئولیت کامل
├── SETUP_GUIDE.md            # این فایل
└── .gitignore                # فایل‌های نادیده گرفته شده
```

---

## ❓ سوالات متداول

**س: آیا لازمه فایل‌ها رو در پوشه خاصی بذارم؟**
ج: نه. همه فایل‌ها در ریشه ریپوزیتوری قرار بگیرند کافیه.

**س: اگه اسم کاربری من در گیت‌هاب چیز دیگه‌ای باشه چی؟**
ج: در فایل‌های `README.md` و `LICENSE` کلمه `replica` رو با یوزرنیم خودتون جایگزین کنید.

**س: آیا می‌تونم بعداً تغییراتی اعمال کنم؟**
ج: بله. هر بار که فایلی رو ادیت یا اضافه کنید، یک commit جدید ایجاد می‌شه.

**س: چطور می‌تونم release ایجاد کنم؟**
ج: در صفحه ریپو، روی **"Releases" > "Create a new release"** کلیک کنید. نسخه (مثلاً `v1.0.0`)، عنوان و توضیحات اضافه کنید.

---

**موفق باشید!** 🚀

اگر سوالی داشتید، می‌تونید در issues پروژه مطرح کنید.
