# بخش فرانت‌اند نینی‌دون

<div dir="rtl">

این بخش، مسیر کاری فرانت‌اند محصول **نینی‌دون** در چتر **پلتفرم هوشمند آتیداد** است.

| مورد | نشانی |
|---|---|
| مخزن محصول | [aroncoict-star/NiniDon](https://github.com/aroncoict-star/NiniDon) |
| نقشهٔ کار فرانت‌اند | [FRONTEND-ROADMAP.md](https://github.com/aroncoict-star/NiniDon/blob/main/docs/FRONTEND-ROADMAP.md) |
| گزارش فاز F5 | [FRONTEND-F5.md](https://github.com/aroncoict-star/NiniDon/blob/main/docs/reports/FRONTEND-F5.md) |
| گزارش فاز F1 | [FRONTEND-F1.md](https://github.com/aroncoict-star/NiniDon/blob/main/docs/reports/FRONTEND-F1.md) |

## دامنه

- رابط Next.js (App Router)، Tailwind، PWA و Service Worker.
- دسترس‌پذیری، RTL/LTR، موبایل ۳۷۵px، عملکرد و تست‌های Playwright/axe.
- دارایی‌های برند و تجربهٔ دوزبانهٔ فارسی/انگلیسی.

## وضعیت فاز F5

- ناوبری بخش‌ها با Back/Forward، کشوی موبایل با focus trap، تاریخچهٔ گفتگو با refresh روی ۴۰۱ و سنجاق با rollback.
- گفتگوها به حساب کاربر مقید شده‌اند و در logout پاک می‌شوند؛ لغو پاسخ در جریان با «گفتگوی جدید».
- رابط انگلیسی داشبوردها پاک‌سازی شد؛ عنوان/خلاصه/FAQ/بدنهٔ مقالات پزشکی تا بازبینی انسانی فارسی و حفاظت‌شده می‌مانند.
- آیکون‌های مات Apple/maskable و کارت OG اضافه شدند.

## دروازهٔ کیفیت

```powershell
pnpm --filter @ninidoon/web typecheck
pnpm --filter @ninidoon/web test
pnpm --filter @ninidoon/web build
cd apps\web; $env:E2E_PORT="3100"; pnpm exec playwright test
```

نتیجهٔ آخر: typecheck ✅، Vitest ۱۴ ✅، build ✅، Playwright ۶۴ گذر / ۱۰ skip، axe ✅.

## محدودیت‌ها

- بدنهٔ مقالات پزشکی در نسخهٔ انگلیسی تا بازبینی شورای پزشکی فارسی می‌ماند (مرز ایمنی).
- رابط انگلیسی پس از hydration اعمال می‌شود؛ HTML عمومی static و فارسی است.
- Lighthouse در فاز F6 اجرا می‌شود.
- ساخت GitHub Project V2 به scope `project` نیاز دارد؛ milestone و issue فرانت‌اند موجود است.

</div>
