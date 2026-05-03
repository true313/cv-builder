# 📄 CV Builder - AI سے چلنے والا CV بنانے کا نظام

یہ ایک جدید، مکمل حل ہے جو صارفین کو اپنا CV بنانے، اپ لوڈ کرنے، اور AI سے بہتر بنانے کی سہولت فراہم کرتا ہے۔

## ✨ خصوصیات

- ✅ **CV بنانے کے دو طریقے**: فارم سے یا اپ لوڈ کر کے
- ✅ **AI سے بہتری**: Google Gemini سے ATS کے لیے CV بہتر بنائیں
- ✅ **دو زبانیں**: اردو اور انگریزی میں CV
- ✅ **خوبصورت PDF**: Professional دکھنے والے PDF download کریں
- ✅ **User Dashboard**: اپنے تمام CVs کو ایک جگہ دیکھیں
- ✅ **Admin Panel**: ادائیگیوں کو منظور کریں
- ✅ **Email Notifications**: اہم اطلاعات براہ ای میل
- ✅ **Secure Authentication**: NextAuth.js سے محفوظ لاگ ان

## 🚀 شروع کریں

### ضروری چیزیں
- Node.js 18+
- PostgreSQL
- Google OAuth credentials
- Google Gemini API key

### Installation

1. Repository clone کریں:
```bash
git clone <repository-url>
cd cv-builder
```

2. Dependencies install کریں:
```bash
npm install
```

3. `.env.local` فائل بنائیں (دیکھیں: `.env.example`):
```bash
DATABASE_URL=postgresql://...
NEXTAUTH_URL=http://localhost:3000
NEXTAUTH_SECRET=your-secret-key
GOOGLE_ID=...
GOOGLE_SECRET=...
GEMINI_API_KEY=...
```

4. Database منتقل کریں:
```bash
npx prisma migrate dev
```

5. Server شروع کریں:
```bash
npm run dev
```

6. http://localhost:3000 کھولیں

## 📚 Project Structure

```
src/
├── app/
│   ├── api/              # API routes
│   ├── admin/            # Admin panel
│   ├── cv/               # CV pages
│   ├── dashboard/        # صارف کا dashboard
│   └── ...
├── components/           # UI components
├── lib/                  # Core logic
└── types/                # TypeScript types
```

## 🔧 Development

```bash
npm run dev       # Server شروع کریں
npm run build     # Production build
npm run test      # Tests چلائیں
npm run lint      # Code lint کریں
```

## 📧 Email Setup

فی الوقت console میں logging ہے۔ Production کے لیے `.env.local` میں email service سیٹ کریں۔

## 📝 More Info

دیکھیں `.env.example` اور مزید تفصیلات کے لیے دستاویزات۔
