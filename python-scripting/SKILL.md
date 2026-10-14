---
name: python-scripting
description: اجرای اسکریپت‌های Python برای پردازش داده‌ها
---

# اسکریپت‌نویسی Python

## کتابخانه‌های مورد استفاده
- pandas: خواندن و پردازش داده‌های جدولی
- openpyxl: خواندن و نوشتن فایل‌های اکسل
- numpy: محاسبات عددی
- matplotlib: رسم نمودار

## الگوی خواندن اکسل
import pandas as pd
df = pd.read_excel(r'مسیر\فایل.xlsx', sheet_name='Data (Input)')
print(df.head())

## الگوی نوشتن اکسل
from openpyxl import Workbook
wb = Workbook()
ws = wb.active
ws.title = "گزارش"
ws.append(["ستون ۱", "ستون ۲"])
wb.save(r'مسیر\خروجی.xlsx')

## الگوی محاسبات آماری
mean = df['مقاومت'].mean()
std_sample = df['مقاومت'].std(ddof=1)
std_pop = df['مقاومت'].std(ddof=0)
cv = (std_sample / mean) * 100

## قوانین
- همیشه با encoding='utf-8' کار کن.
- مسیرها را با r'...' بنویس.
- خطاها را با try/except مدیریت کن.
- نتیجه را با print گزارش بده.
