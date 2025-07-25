# Claude Code GitHub Actions
# دستیار هوشمند و اتوماسیون Claude Code با قابلیت شخصی سازی
## توضیحات پروژه

این پروژه یک سیستم اتوماسیون قدرتمند برای GitHub است که از Claude AI برای بهبود workflow های توسعه نرم‌افزار استفاده می‌کند[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions). با این سیستم می‌توانید issue ها را به صورت خودکار به Pull Request تبدیل کنید، کد review انجام دهید و مسائل برنامه‌نویسی را حل کنید[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions).

## ویژگی‌های اصلی

### 🤖 اتوماسیون هوشمند
- **ایجاد فوری PR**: توضیح دهید چه نیاز دارید، کلود PR کاملی با تمام تغییرات لازم ایجاد می‌کند[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions)
- **پیاده‌سازی خودکار کد**: issue ها را با یک دستور به کد کاری تبدیل می‌کند[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions)
- **پیروی از استانداردهای شما**: کلود به راهنماهای CLAUDE.md و الگوهای کد موجود احترام می‌گذارد[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions)
- **رفع سریع باگ‌ها**: کلود باگ را پیدا کرده، راه‌حل پیاده‌سازی می‌کند و PR ایجاد می‌کند[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions)

### 🔧 پیکربندی آسان
- **راه‌اندازی ساده**: در چند دقیقه با installer و API key شروع کنید[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions)
- **پشتیبانی از AWS Bedrock و Google Vertex AI**: برای محیط‌های enterprise[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions)
- **تنظیمات سفارشی**: کنترل کامل بر data residency و billing[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions)

### 🛡️ امنیت بالا
- **امن به صورت پیش‌فرض**: کد شما روی GitHub runners باقی می‌ماند[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions)
- **استفاده از GitHub Secrets**: همیشه از GitHub Secrets برای API key ها استفاده کنید[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions)
- **محدود کردن مجوزهای action**: فقط مجوزهای ضروری اعطا کنید[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions)

## نصب و راه‌اندازی

### روش سریع
ساده‌ترین راه راه‌اندازی این action از طریق Claude Code در terminal است[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions). فقط claude را باز کرده و دستور زیر را اجرا کنید:

`/install-github-app`

این دستور شما را در راه‌اندازی GitHub app و secret های مورد نیاز راهنمایی می‌کند[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions).

### راه‌اندازی دستی
اگر دستور `/install-github-app` کار نکرد یا راه‌اندازی دستی را ترجیح می‌دهید[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions):

1. **Claude GitHub app را نصب کنید**: https://github.com/apps/claude[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions)
2. **ANTHROPIC_API_KEY را به repository secrets اضافه کنید**[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions)
3. **فایل workflow را کپی کنید** از examples/claude.yml به `.github/workflows/` پروژه خود[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions)

پس از تکمیل راه‌اندازی، action را با mention کردن `@claude` در issue یا PR comment تست کنید[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions)!

## نحوه استفاده

### مثال‌های کاربردی

**تبدیل issue ها به PR ها**:
در کامنت issue: `@claude implement this feature based on the issue description`[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions)

کلود issue را تجزیه و تحلیل می‌کند، کد را می‌نویسد و PR ایجاد می‌کند[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions).

**دریافت کمک پیاده‌سازی**:
در کامنت PR: `@claude how should I implement user authentication for this endpoint?`[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions)

کلود کد شما را تجزیه و تحلیل کرده و راهنمایی مشخص برای پیاده‌سازی ارائه می‌دهد[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions).

**رفع سریع باگ‌ها**:
در issue: `@claude fix the TypeError in the user dashboard component`[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions)

کلود باگ را پیدا کرده، راه‌حل پیاده‌سازی می‌کند و PR ایجاد می‌کند[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions).

## پیکربندی پیشرفته

### استفاده با AWS Bedrock و Google Vertex AI
برای محیط‌های enterprise، می‌توانید Claude Code GitHub Actions را با زیرساخت cloud خودتان استفاده کنید[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions). این روش کنترل بر data residency و billing را در اختیار شما قرار می‌دهد[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions).

### پیش‌نیازها

**برای Google Cloud Vertex AI**[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions):
1. یک Google Cloud Project با Vertex AI فعال
2. Workload Identity Federation پیکربندی شده برای GitHub Actions
3. یک service account با مجوزهای مورد نیاز
4. یک GitHub App (پیشنهادی) یا استفاده از GITHUB_TOKEN پیش‌فرض

**برای AWS Bedrock**[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions):
1. یک AWS account با Amazon Bedrock فعال
2. GitHub OIDC Identity Provider پیکربندی شده در AWS
3. یک IAM role با مجوزهای Bedrock
4. یک GitHub App (پیشنهادی) یا استفاده از GITHUB_TOKEN پیش‌فرض


## بهترین روش‌ها

### پیکربندی CLAUDE.md
فایل `CLAUDE.md` در root repository خود ایجاد کنید تا راهنماهای code style، معیارهای review، قوانین مخصوص پروژه و الگوهای ترجیحی را تعریف کنید[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions). این فایل درک کلود از استانداردهای پروژه شما را راهنمایی می‌کند[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions).

### ملاحظات امنیتی
هرگز API key ها را مستقیماً در repository commit نکنید[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions)!

همیشه از GitHub Secrets برای API key ها استفاده کنید[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions):
- API key خود را به عنوان repository secret با نام `ANTHROPIC_API_KEY` اضافه کنید
- مجوزهای action را فقط به آنچه ضروری است محدود کنید
- پیشنهادات کلود را قبل از merge بررسی کنید

### بهینه‌سازی عملکرد
از issue template ها برای ارائه context استفاده کنید، `CLAUDE.md` خود را مختصر و متمرکز نگه دارید، و timeout مناسب برای workflow هایتان پیکربندی کنید[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions).

### هزینه‌های CI
هنگام استفاده از Claude Code GitHub Actions، از هزینه‌های مرتبط آگاه باشید[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions):

**هزینه‌های GitHub Actions**:
- Claude Code روی GitHub-hosted runner ها اجرا می‌شود که دقیقه‌های GitHub Actions شما را مصرف می‌کند[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions)

**هزینه‌های API**:
- هر تعامل کلود بر اساس طول prompt ها و پاسخ‌ها، token های API مصرف می‌کند[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions)
- استفاده token بسته به پیچیدگی task و اندازه codebase متفاوت است[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions)

## مثال‌های پیکربندی
برای پیکربندی‌های workflow آماده برای موارد استفاده مختلف، شامل راه‌اندازی پایه workflow برای issue و PR comment ها، code review خودکار روی pull request ها، و پیاده‌سازی‌های سفارشی برای نیازهای خاص، از examples directory در Claude Code Action repository دیدن کنید[(1)](https://docs.anthropic.com/en/docs/claude-code/github-actions).

## مشکلات رایج و راه‌حل

### خطای Authentication
- API key را در repository secrets بررسی کنید
- مجوزهای GitHub token را تأیید کنید

### عدم پاسخ Claude
- Trigger phrase (`@claude`) را بررسی کنید
- Workflow permissions را چک کنید

## مشارکت

برای مشارکت در بهبود این پروژه:
1. Repository را fork کنید
2. تغییرات خود را اعمال کنید
3. Pull Request با توضیحات کامل ایجاد کنید

## لایسنس

این پروژه تحت شرایط و ضوابط edrispapi منتشر شده است.
