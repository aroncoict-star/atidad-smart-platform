# بخش فرانت‌اند نینی‌دون

<div dir="rtl">

این بخش، مسیر کاری فرانت‌اند محصول **نینی‌دون** در چتر **پلتفرم هوشمند آتیداد** است.

| مورد | نشانی |
|---|---|
| مخزن محصول | [aroncoict-star/NiniDon](https://github.com/aroncoict-star/NiniDon) |
| نقشهٔ کار کل | [WORKPLAN.md](https://github.com/aroncoict-star/NiniDon/blob/main/WORKPLAN.md) |
| نقشهٔ فرانت‌اند | [FRONTEND-ROADMAP.md](https://github.com/aroncoict-star/NiniDon/blob/main/docs/FRONTEND-ROADMAP.md) |
| گزارش فاز جاری | [FRONTEND-F1.md](https://github.com/aroncoict-star/NiniDon/blob/main/docs/reports/FRONTEND-F1.md) |

## دامنه

- رابط کاربری Next.js (App Router)، Tailwind، PWA و Service Worker.
- دسترس‌پذیری، RTL/LTR، موبایل ۳۷۵px، عملکرد و تست‌های Playwright/axe.
- دارایی‌های برند و تجربهٔ دوزبانهٔ فارسی/انگلیسی.

## دروازهٔ کیفیت

```powershell
pnpm --filter @ninidoon/web typecheck
pnpm --filter @ninidoon/web test
pnpm --filter @ninidoon/web build
cd apps\web; $env:E2E_PORT="3100"; pnpm exec playwright test
```

## وضعیت

- ناوبری، تاریخچهٔ گفتگو و سنجاق چت، لوگوی شفاف و سوییچ زبان پیاده‌سازی و تست شده‌اند.
- بدنهٔ مقالات پزشکی در نسخهٔ انگلیسی تا بازبینی شورای پزشکی به فارسی می‌ماند (مرز ایمنی).
- ساخت GitHub Project V2 به scope `project` نیاز دارد؛ اپیک چتر در Issues موجود است.

</div>
