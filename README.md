# NOOR-E-ISLAM (نورِ اسلام)
## Complete Islamic Super App & Platform (مکمل اسلامی ڈیجیٹل پلیٹ فارم اور سورس کوڈ)

A complete, responsive Islamic platform and Progressive Web App (PWA) built with **React 19**, **TypeScript**, **Tailwind CSS 4**, and **Vite**.

---

## 🇵🇰 اردو ہدایات برائے وی ایس کوڈ (VS Code Setup in Urdu)

### 1. فولڈر کو ٹرسٹ کریں (Trust Folder in VS Code)
جب آپ وی ایس کوڈ (VS Code) میں پروجیکٹ کھولتے ہیں تو اوپر لکھا آتا ہے:
> *"Restricted Mode is intended for safe code browsing. Trust this folder to enable features"*
آپ اوپر **"Manage"** یا **"Trust"** پر کلک کر کے **"Trust Folder and all files"** منتخب کریں۔

### 2. ٹرمینل کھولیں (Open Terminal)
وی ایس کوڈ کے اوپر مینیو سے **Terminal > New Terminal** پر کلک کریں (یا کی بورڈ سے \`Ctrl + \`\` دبائیں)۔

### 3. ڈیپینڈینسیز انسٹال کریں (Install Dependencies)
ٹرمینل میں یہ کمانڈ لکھ کر Enter دبائیں:
\`\`\`bash
npm install
\`\`\`
*(نوٹ: اگر آپ کے پاس Node.js انسٹال نہیں ہے تو پہلے [nodejs.org](https://nodejs.org) سے Node.js کا LTS ورژن ڈاؤنلوڈ کر کے انسٹال کر لیں)*

### 4. ویب سائٹ لائیو چلائیں (Run Live)
انسٹالیشن مکمل ہونے کے بعد یہ کمانڈ چلائیں:
\`\`\`bash
npm run dev
\`\`\`

ٹرمینل میں لنک آئے گا:
\`\`\`
➜  Local:   http://localhost:3000/
\`\`\`
اس لنک پر کلک کریں یا براؤزر میں کھولیں، آپ کی پوری **نورِ اسلام** ویب سائٹ تمام سکرینز اور فیچرز کے ساتھ لائیو چل پڑے گی!

---

## 🇬🇧 English Setup Instructions

### Prerequisites
- [Node.js](https://nodejs.org/) (Version 18 or 20+ LTS recommended)
- VS Code or any text editor

### Quick Start in 3 Steps:

1. **Open project in VS Code**
2. **Install dependencies:**
   \`\`\`bash
   npm install
   \`\`\`
3. **Start Development Server:**
   \`\`\`bash
   npm run dev
   \`\`\`
4. Open [http://localhost:3000](http://localhost:3000) in your browser.

---

## 📱 Mobile & PWA Installation / Android
This project includes standard Progressive Web App (PWA) manifest support in \`public/manifest.json\`:
- In Chrome / Edge / Mobile browsers, click the **"Install App"** icon in the address bar.
- On Android, open the website in Chrome, tap **⋮ (Menu) > Add to Home screen / Install app**.

To package as native Android APK using Capacitor:
\`\`\`bash
npm install @capacitor/core @capacitor/cli @capacitor/android
npx cap init "Noor-e-Islam" "com.nooreislam.app"
npm run build
npx cap add android
npx cap copy
npx cap open android
\`\`\`

---

## 📁 Project Directory Structure (اے سے لے کر زیڈ تک مکمل فائلیں)

\`\`\`
NOOR-E-ISLAM/
├── public/
│   ├── manifest.json                  # PWA Manifest configuration
│   └── assets/                        # Islamic Mosque & Logo images
├── src/
│   ├── main.tsx                       # React application entry point
│   ├── App.tsx                        # Master application component & navigation router
│   ├── index.css                      # Tailwind 4, Arabic & Urdu typography, styling
│   ├── types/
│   │   └── index.ts                   # All TypeScript models & interfaces
│   ├── data/
│   │   ├── translations.ts            # English, Urdu (اردو), Arabic (العربية), Hindi (हिन्दी)
│   │   ├── quranData.ts               # Complete 114 Surahs, Uthmani script, audio streams
│   │   ├── prayerTimesData.ts         # Astronomical solar calculator & cities database
│   │   ├── adhanData.ts               # Makkah, Madinah, Al-Aqsa Adhans & post-Adhan Dua
│   │   ├── booksData.ts               # Sahih Bukhari, Sealed Nectar, Stories of Prophets
│   │   ├── duasData.ts                # Hisn al-Muslim daily Azkar & supplications
│   │   ├── prophetsData.ts            # Detailed stories of Prophets (AS) & moral lessons
│   │   ├── historyData.ts             # Khulafa-e-Rashideen & Islamic history timeline
│   │   ├── tasbeehData.ts             # Dhikr presets, targets, virtues
│   │   ├── calendarData.ts            # Hijri conversion, sacred months & fasting days
│   │   ├── learningData.ts            # Wudu, Salah, Tajweed steps & interactive Quiz
│   │   └── wallpapersData.ts          # Curated HD & 4K wallpapers
│   └── components/
│       ├── Header.tsx                 # Mosque hero banner, Gregorian & Hijri live dates
│       ├── Sidebar.tsx                # Desktop gold & emerald sidebar navigation
│       ├── MobileNav.tsx              # Sticky mobile bottom bar + menu drawer
│       ├── HomeScreen.tsx             # Complete dashboard matching the mockup design
│       ├── QuranScreen.tsx            # Complete Quran browser with 114 Surahs & audio
│       ├── PrayerTimesScreen.tsx      # 5 daily prayers, Hanafi/Shafi'i, weekly schedule
│       ├── AdhanScreen.tsx            # Adhan audio player, notifications & test alerts
│       ├── BooksScreen.tsx            # Islamic library & reader with chapters & night mode
│       ├── DuasScreen.tsx             # Daily Duas with Arabic, Urdu, English & audio
│       ├── TasbeehScreen.tsx          # Interactive digital beads, sound, haptic & confetti
│       ├── CalendarScreen.tsx         # Hijri calendar, Ayyam-e-Beed & Sunnah fasts
│       ├── QiblaScreen.tsx            # Real-time Qibla compass dial & distance to Kaaba
│       ├── DiaryScreen.tsx            # 5-Salah checklist, Quran tracker & spiritual journal
│       ├── WallpapersScreen.tsx       # HD Islamic wallpapers with fullscreen download
│       ├── LearningScreen.tsx         # Wudu & Salah step-by-step guides & quiz
│       ├── ProphetsScreen.tsx         # Stories of Prophets with lessons
│       ├── HistoryScreen.tsx          # Islamic history and historical personalities
│       ├── UserProfileScreen.tsx      # User profile, streaks & bookmarks
│       ├── SettingsScreen.tsx         # Language selector, juristic settings & cache
│       ├── AdminDashboard.tsx         # Passcode-protected owner management panel
│       └── Modals/
│           ├── WelcomeModal.tsx       # First-time onboarding dialog
│           ├── LanguageModal.tsx      # Language switcher modal
│           ├── LocationModal.tsx      # GPS permission & manual city selector
│           └── ExportSourceZipModal.tsx # Download complete source code ZIP
├── .env.example                       # Environment template
├── .gitignore                         # Git ignore definitions
├── index.html                         # HTML5 template with Google fonts
├── metadata.json                      # AI Studio applet metadata
├── package.json                       # Dependencies & scripts
├── tsconfig.json                      # TypeScript configuration
└── vite.config.ts                     # Vite + React + Tailwind configuration
\`\`\`

---

## 🕌 Religious Authenticity (شرعی تحقیق و تصدیق)
All Quranic verses are in authentic Uthmanic script. Hadiths are cited from canonical verified works (*Sahih al-Bukhari*, *Sahih Muslim*, *Riyadh as-Saliheen*). No artificial intelligence is used to generate religious rulings or sacred texts.

---
**Noor-e-Islam (نورِ اسلام) — Faith • Knowledge • Peace**
\`\`\`
May Allah accept this humble endeavor. Ameen.
\`\`\`
