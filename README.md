# 🦫 Beavor - Financial Nebula & Shared Expense Tracker

A premium, glassmorphic financial management and expense-splitting application built with **Flutter**, **GetX**, and **Supabase**. **Beavor** (also known as *Luminous Ledger*) transforms tracking expenses and splitting household/group bills into a seamless ambient visual experience with atomic data integrity.

---

## ✨ Features

- **💎 Fluid Glassmorphic Design**: Powered by the "Financial Nebula" design system, featuring custom glassmorphism, radial ambient glows, dynamic dark themes, and curated Google Fonts (*Manrope* & *Inter*).
- **🏦 Multi-Wallet Intelligence**: Track and manage multiple funding sources (Cash, Card, Savings) with real-time balance updates.
- **✍️ Atomic Transaction & Category Management**: Easily create, edit, and categorize transactions with slidable item actions and instant balance calculations.
- **🤝 Expense Splitter & Member Management**: Manage group or household members, record shared expenses, and automatically compute debt/repayment balances.
- **📊 Intuitive Spending Analytics**: Visual financial insights with interactive donut charts and trend analysis powered by `fl_chart`.
- **🗓️ Interactive Calendar View**: Track daily income and expenditure timeline with integrated calendar views powered by `table_calendar`.
- **🇻🇳 Multi-Language Support**: Native localization for Vietnamese (`vi_VN`) and English (`en_US`).
- **☁️ Supabase Cloud Sync & Local Storage**: Real-time cloud persistence with Supabase PostgreSQL, complemented by local offline storage via `get_storage`.
- **🔄 In-App Auto Update**: Automatic version checking and background APK download/installation powered by `dio` and `open_filex`.

---

## 🎨 Design Philosophy

Beavor prioritizes **Visual Excellence**:
- **Ambient Glows**: Soft radial background gradients that visually reflect financial status.
- **Deep Contrast Dark Mode**: Designed for high legibility and reduced eye strain.
- **No-Boundary Layouts**: Modern, borderless cards and glass containers for a smooth visual hierarchy.

---

## 🛠️ Technology Stack

- **Framework**: [Flutter](https://flutter.dev) (Dart SDK `^3.10.0`)
- **State Management & Navigation**: [GetX](https://pub.dev/packages/get)
- **Backend & Authentication**: [Supabase Flutter](https://pub.dev/packages/supabase_flutter)
- **Local Storage**: [GetStorage](https://pub.dev/packages/get_storage)
- **Data Visualization**: [fl_chart](https://pub.dev/packages/fl_chart)
- **Calendar Component**: [table_calendar](https://pub.dev/packages/table_calendar)
- **HTTP Client**: [Dio](https://pub.dev/packages/dio)
- **Environment Configuration**: [flutter_dotenv](https://pub.dev/packages/flutter_dotenv)
- **UI Enhancements**: `flutter_slidable`, `image_picker`, `google_fonts`, `share_plus`, `open_filex`

---

## 📁 Project Structure

```text
lib/
├── controllers/          # GetX Controllers for app logic & state
├── core/                 # Core utilities, app theme, i18n, and Supabase config
│   ├── i18n/            # Internationalization (EN / VI)
│   ├── services/        # Core services (Supabase initialization)
│   └── theme/           # App design tokens & dark glassmorphic theme
├── models/               # Data models (Transaction, Category, Wallet, Member, etc.)
├── screens/              # UI Screen views
│   ├── dashboard/       # Main dashboard overview
│   ├── analysis/        # Chart analytics & spending reports
│   ├── calendar/        # Calendar timeline view
│   ├── expense_splitter/# Group bill splitting & debt settlement
│   ├── members/         # Member management for shared expenses
│   ├── transaction_history/ # Full transaction log & filtering
│   └── profile/         # User profile & settings
├── services/             # Application services (Expense Splitter, Auto-Update, Local Storage)
└── widgets/              # Custom reusable glassmorphic UI components
```

---

## 🚀 Getting Started

### Prerequisites

- [Flutter SDK](https://flutter.dev/docs/get-started/install) (v3.10.0 or higher)
- A [Supabase](https://supabase.com/) project with PostgreSQL database and Authentication configured.

### Environment Setup

Create a `.env` file in the project root:

```env
SUPABASE_URL=https://your-supabase-project.supabase.co
SUPABASE_ANON_KEY=your-supabase-anon-key

# Optional: Remote JSON URL for in-app APK auto-update checks
UPDATE_METADATA_URL=https://your-domain.com/update_metadata.json
```

### Installation & Execution

1. **Clone the repository**:
   ```bash
   git clone https://github.com/trieu-dev/beavor.git
   cd beavor
   ```

2. **Install dependencies**:
   ```bash
   flutter pub get
   ```

3. **Run the app**:
   ```bash
   flutter run
   ```

---

## 📈 Roadmap

- [ ] 🎯 **Monthly Budgeting & Goals**: Set visual spending limits per category.
- [ ] 🤖 **Smart Financial Insights**: AI-powered spending tips and summary reports.
- [ ] 🔒 **Biometric Security**: FaceID / Fingerprint application lock.
- [ ] 🗓️ **Recurring Subscription Tracker**: Scheduled notifications for recurring bills.

---

Developed with ❤️ by **Trieu Dev**.
