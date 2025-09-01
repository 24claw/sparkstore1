# متجر الخدمات الرقمية - Discord Store

متجر إلكتروني متكامل لبيع خدمات Discord مثل Nitro وبوستات السيرفرات.

## المميزات

✅ **صفحة تسجيل دخول احترافية** مع تكامل Google  
✅ **تصميم متجاوب** يعمل على جميع الأجهزة  
✅ **سلة تسوق متقدمة** مع نظام دفع محاكي  
✅ **منتجات Discord** (Nitro وبوستات)  
✅ **ألوان متناسقة** (أزرق، أبيض، فيروزي، أسود)  
✅ **تأثيرات حركية** باستخدام Framer Motion  
✅ **مكونات UI حديثة** مع shadcn/ui  

## التقنيات المستخدمة

- **React 18** - مكتبة واجهة المستخدم
- **Vite** - أداة البناء السريعة
- **Tailwind CSS** - إطار عمل CSS
- **shadcn/ui** - مكونات UI جاهزة
- **Framer Motion** - تأثيرات الحركة
- **Lucide React** - أيقونات حديثة

## التشغيل المحلي

```bash
# تثبيت المتطلبات
npm install

# تشغيل خادم التطوير
npm run dev

# بناء المشروع للإنتاج
npm run build
```

## النشر على GitHub و Netlify

### 1. رفع المشروع على GitHub

```bash
# إنشاء مستودع Git
git init

# إضافة جميع الملفات
git add .

# إنشاء commit أول
git commit -m "Initial commit: Discord Store"

# ربط المستودع البعيد (استبدل USERNAME بمعرفك)
git remote add origin https://github.com/USERNAME/discord-store.git

# رفع الكود
git push -u origin main
```

### 2. النشر على Netlify

#### الطريقة الأولى: من خلال GitHub (مُوصى بها)

1. اذهب إلى [netlify.com](https://netlify.com)
2. سجل دخولك أو أنشئ حساب جديد
3. انقر على "New site from Git"
4. اختر GitHub وامنح الصلاحيات
5. اختر مستودع `discord-store`
6. اضبط إعدادات البناء:
   - **Build command**: `npm run build`
   - **Publish directory**: `dist`
7. انقر على "Deploy site"

#### الطريقة الثانية: رفع مباشر

```bash
# بناء المشروع
npm run build

# تثبيت Netlify CLI
npm install -g netlify-cli

# تسجيل الدخول
netlify login

# نشر الموقع
netlify deploy --prod --dir=dist
```

### 3. إعدادات إضافية

#### تخصيص الدومين
- في لوحة تحكم Netlify، اذهب إلى "Domain settings"
- يمكنك ربط دومين مخصص أو استخدام الدومين المجاني

#### متغيرات البيئة (إذا لزم الأمر)
- في لوحة تحكم Netlify، اذهب إلى "Site settings" > "Environment variables"
- أضف أي متغيرات مطلوبة للإنتاج

## هيكل المشروع

```
discord-store/
├── public/                 # الملفات العامة
├── src/
│   ├── assets/            # الصور والملفات الثابتة
│   │   └── logo.png       # شعار المتجر
│   ├── components/        # مكونات React
│   │   ├── ui/           # مكونات UI أساسية
│   │   ├── LoginPage.jsx # صفحة تسجيل الدخول
│   │   ├── HomePage.jsx  # الصفحة الرئيسية
│   │   └── CartModal.jsx # نافذة سلة التسوق
│   ├── App.jsx           # المكون الرئيسي
│   ├── App.css          # الأنماط المخصصة
│   └── main.jsx         # نقطة الدخول
├── package.json         # متطلبات المشروع
└── README.md           # هذا الملف
```

## المنتجات المتاحة

### Discord Nitro
- **شهر واحد**: $25 (بدلاً من $35)
- **3 أشهر**: $65 (بدلاً من $90)

### بوستات Discord
- **حزمة أساسية**: $15 (1000 بوست)
- **حزمة متقدمة**: $40 (5000 بوست)

## الدعم الفني

للحصول على المساعدة أو الإبلاغ عن مشاكل:
- البريد الإلكتروني: support@store.com
- الهاتف: +966 50 123 4567
- ساعات العمل: 24/7

## الترخيص

هذا المشروع مُرخص تحت رخصة MIT - راجع ملف [LICENSE](LICENSE) للتفاصيل.

---

**ملاحظة**: هذا مشروع تعليمي ونظام الدفع محاكي فقط. لا تستخدم بيانات دفع حقيقية.

