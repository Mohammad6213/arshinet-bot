# Telegram Config Shop Bot

ربات فروش کانفیگ با تحویل دستی.

## امکانات
- منوی خرید
- 10/20/30/50/100 گیگ
- ثبت سفارش در SQLite
- دریافت تصویر رسید
- ارسال رسید برای ادمین
- تأیید/رد پرداخت توسط ادمین
- ارسال کانفیگ با دستور `/config ORDER_ID CONFIG`
- نمایش سفارش‌های کاربر
- پشتیبانی

## نصب

Python 3.10+ پیشنهاد می‌شود.

```bash
python -m venv venv
```

Windows:
```bash
venv\Scripts\activate
```

Linux/macOS:
```bash
source venv/bin/activate
```

سپس:
```bash
pip install -r requirements.txt
```

فایل `.env.example` را به `.env` تغییر نام بده و مقادیرش را پر کن.

بعد:
```bash
python bot.py
```

## ساخت ربات
در تلگرام به `@BotFather` برو، `/newbot` را بزن و توکن را داخل `.env` قرار بده.

## پیدا کردن ADMIN_ID
می‌توانی از یک ربات نمایش‌دهنده Telegram User ID استفاده کنی یا از روش مورداعتماد خودت ID عددی حسابت را به دست بیاوری.

## تحویل کانفیگ
پس از تأیید رسید:
```text
/config 123 vless://...
```

ربات کانفیگ را برای مشتری سفارش 123 ارسال می‌کند.

## نکته امنیتی
`.env` و `bot.db` را عمومی یا داخل GitHub منتشر نکن.
