---
name: powershell-execution
description: اجرای دستورات PowerShell برای مدیریت فایل‌ها و پوشه‌ها
---

# اجرای دستورات PowerShell

## دستورات پرکاربرد

### ساخت پوشه
New-Item -ItemType Directory -Path "مسیر\پوشه" -Force

### کپی فایل
Copy-Item -Path "منبع" -Destination "مقصد" -Recurse -Force

### انتقال فایل
Move-Item -Path "منبع" -Destination "مقصد" -Force

### حذف فایل (با احتیاط)
Remove-Item -Path "مسیر\فایل" -Force

### لیست فایل‌ها
Get-ChildItem -Path "مسیر" | Select-Object Name, Length, LastWriteTime

### بررسی وجود فایل
Test-Path "مسیر\فایل"

## قوانین
- قبل از حذف، حتماً تأییدیه از مهندس بگیر.
- مسیرها را با نقل‌قول بنویس تا فاصله‌ها مشکل نسازند.
- پس از هر عملیات، نتیجه را گزارش بده.
