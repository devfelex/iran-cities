# iran-cities

Iran-cities is the most accurate database of Iran city, county and provinces.

این بانک اطلاعاتی شامل تمامی استانها، شهرستانها و شهرهای ایران می باشد.

این بانک را زمانی ایجاد کردم که ناامید شدم. برای پروژه ای نیاز به بانک اطلاعاتی دقیق تمامی شهرهای ایران را داشتم، اما با جستجوی فراوان در اینترنت حتی یک نمونه کامل و بدون نقص پیدا نکردم.
قبل از اینکه جستجو کنم به نظرم یافتن چنین چیزی بسیار ساده و پیش پا افتاده بود، اما در کمال تعجب نبود!


#  1.0نسخه
این بانک براساس براساس آخرین تقسیمات کشوری تا پایان سال ۱۳۹۴ که توسط مرکز آمار ایران ارائه شده است ایجاد گردیده است. در زمان ایجاد این نسخه(فروردین 1396) این آخرین اطلاعات ارائه شده توسط مرکز آمار است که براساس آن  کشور ایران از ۳۱ استان، ۴۲۹ شهرستان، ۱۰۵۷ بخش، ۲۵۸۹ دهستان و ۱۲۴۵ شهر تشکیل یافته‌است. 
بدیهی است در صورت به روز رسانی آمار رسمی، نسخه جدید این بانک هم براساس آخرین داده ها به روزآوری خواهد شد.

# نقاط قوت
با بررسی بانک های موجود بر روی اینترنت اشکالات زیر مشاهده گردید:
- برخی از آنها بسیار قدیمی بودند و بسیاری از مناطق و شهرها در آنها لیست نشده بود، مثلا شامل استان البرز نبودند.
- برخی از آنها تنها شامل برخی از شهرهای ایران بودند
- برخی از آنها به اشتباه نام شهرستان های ایران را به عنوان لیست شهرهای ایران درج کرده بودند.
- برخی از آنها بسیاری از شهرهای ایران را از قلم انداخته بودند، مثلا در یک بررسی سطحی مشخص شد که به عنوان مثال فاقد شهرهای لواسان در استان تهران و ساوه در استان مرکزی هستند.
- علاوه بر اینها در اکثر آنها به جای استفاده از حروف فارسی از حروف معادل عربی (ي و ك) استفاده شده بود که برای جستجوی کاربران در اغلب سیستم عامل ها مشکل زا است.

به طور خلاصه اغلب بانک های موجود از روی چند منبع ناقص و قدیمی کپی شده بودند و دارای ایرادات فراوانی بودند.

این بانک تمام این اشکالات را برطرف کرده است و به طور کامل از روی آخرین داده های رسمی ایجاد گردیده است.

# ساختار
این بانک در دو نسخه SQL و CSV ارائه گردیده است.
نسخه SQL به طور مستقیم قابلیت وارد کردن به MySQL را دارد و از نسخه CSV می توان برای وارد کردن به سایر بانکها استفاده کرد.
در این بانک سه جدول اصلی وجود دارد:
-- جدول استانها: شامل لیست تمای استانهای کشور است
-- جدول شهرستانها: شامل لیست تمامی شهرستانهای ایران و رابطه آن با استانها می باشد.
-- جدول شهرها: شامل تمامی شهرهای ایران و رابطه آنها با شهرستانها و استانهای کشور می باشد.

