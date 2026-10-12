# Vortex Gateway (Fixed for Iran & Railway)

نسخه اصلاح‌شده و بهینه‌سازی‌شده برای عبور از فیلترینگ ایران و اتصال پایدار در Railway.

## فایل‌های پروژه:
- `Dockerfile`: فایل ساخت کانتینر در Railway
- `railway.toml`: تنظیمات دیپلوی در Railway
- `entrypoint.sh`: اسکریپت راه‌اندازی و تنظیم دسترسی دیسک `/data`
- `main.py`: هسته اصلی پایتون مجهز به تفکیک Clean IP و اصلاح سابسکریپشن برای v2rayNG
- `requirements.txt`: وابستگی‌های پروژه
- `templates.py` و `pages.py`: رابط کاربری و صفحات وب

## نحوه دیپلوی در Railway:
1. این فایل‌ها را در یک ریپازیتوری جدید در گیت‌هاب خود آپلود کنید.
2. در Railway پروژه جدید بسازید و ریپازیتوری را متصل کنید.
3. در بخش Settings > Volumes یک ولوم به مسیر `/data` اضافه کنید.
4. در بخش Variables متغیر `ADMIN_PASSWORD` را تنظیم کنید.
5. دامنه عمومی را بسازید (Generate Domain).
