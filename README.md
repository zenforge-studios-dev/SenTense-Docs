# 🌸 SenTense - Anime-Inspired Daily Quotes Widget

[![Android API](https://img.shields.io/badge/API-24%2B-brightgreen)](https://developer.android.com/about/versions/android-7.0)
[![Kotlin](https://img.shields.io/badge/Kotlin-100%25-purple)](https://kotlinlang.org/)
[![Jetpack Compose](https://img.shields.io/badge/Jetpack%20Compose-Latest-blue)](https://developer.android.com/jetpack/compose)
[![Play Store](https://img.shields.io/badge/Google%20Play-Published-green)](https://play.google.com/store/apps/details?id=com.zenforge.studios.sentense)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> A production-grade Android widget application delivering daily anime-inspired quotes directly to your home screen. Built with cutting-edge Android technologies, featuring 7 customizable widget styles, real-time group sharing, and a zero-distraction philosophy.

**[👉 Download on Google Play Store](https://play.google.com/store/apps/details?id=com.zenforge.studios.sentense)**

---

## 📋 Table of Contents

- [Overview](#overview)
- [Key Features](#key-features)
- [Widget Showcase](#widget-showcase)
- [Technical Stack](#technical-stack)
- [Architecture & Design Patterns](#architecture--design-patterns)
- [Installation & Setup](#installation--setup)
- [Core Implementation Details](#core-implementation-details)
- [Contributing Guidelines](#contributing-guidelines)

---

## 🎯 Overview

**SenTense** is a production-ready Android widget application transforming your home screen into a canvas of daily anime-inspired wisdom. Currently published on Google Play Store, it combines beautiful design with powerful functionality.

### Core Mission
Deliver meaningful quotes without friction, focusing on discipline, sacrifice, growth, and elite mindset—all from your home screen.

### Target Users
- Anime enthusiasts seeking daily inspiration
- Builders and entrepreneurs valuing growth mindset
- Users demanding minimal distractions and aesthetic home screens
- Communities sharing focused, intentional messaging

### Business Model
- **Free with optional premium features**
- Google Play monetization via ads and in-app purchases
- Real-time social networking through private/public groups

---

## ✨ Key Features

### 🎨 Widget Customization (7 Styles)

SenTense offers **7 fully customizable widget styles** with live previews:

| Widget Style | Description | Use Case |
|---|---|---|
| **Minimal** | Clean, distraction-free quote display | Minimalists, zen users |
| **Classic** | Traditional elegant card layout | Professional, timeless look |
| **Modern** | Contemporary flat design | Tech-savvy users |
| **Elegant** | Sophisticated with decorative elements | Premium, luxury aesthetic |
| **Card** | Material Design 3 card format | Modern Material users |
| **Gradient** | Eye-catching gradient backgrounds | Visual creators |
| **Glass** | Glassmorphism with blur effects | Design-forward users |

**Customization Controls:**
- ✅ Custom typography (font, size, weight, style)
- ✅ Spacing & padding adjustments
- ✅ Color scheme customization
- ✅ Text alignment options
- ✅ Background patterns
- ✅ Live in-app preview before deployment
- ✅ Multiple widget instances with different styles

### 🔄 Real-time Quote Updates

- **Automatic refresh:** Every 30 minutes (configurable)
- **Manual refresh:** Tap widget to instantly fetch new quote
- **Offline support:** Favorites display even without network
- **Socket.io live stream:** Real-time quote notifications
- **Firebase Cloud Messaging:** Push notifications for group posts

### 👥 Friends & Groups (Social Networking)

**Unique SenTense Feature:** Post quotes directly from widgets to private/public groups

**Group Features:**
- Create private groups (invite-only) or public groups
- Post quotes instantly to group (group members see on widgets)
- Ephemeral quotes: Posted quotes vanish after **2 hours** for fresh inspiration stream
- Like quotes directly from widget (no app open required)
- Curated moderation: Only approved members can post
- No algorithms, no strangers, no noise

**Group Permissions:**
```
Admin:     Create, post, remove members, moderate
Moderator: Post, remove inappropriate content
Member:    Post, like, view group quotes
Viewer:    View-only access
```

### 📚 Curated Quote Categories

**Pre-built Category System:**

| Category | Focus | Example Quotes |
|---|---|---|
| **Anime-Inspired** | Discipline, Sacrifice, Growth, Perseverance | "The only time it's impossible is when you don't try" |
| **Elite Mindset** | Ambition, Clarity, Focus, Excellence | "Success is not final, failure is not fatal" |
| **Motivational** | Resilience, Momentum, Intentional Living | "Your limitations are only in your mind" |
| **Wisdom** | Life lessons, philosophy, growth | "Every master was once a beginner" |
| **Grit** | Determination, perseverance, grit | "Success demands sacrifices" |

**Filtering:**
- Filter by single or multiple categories
- Personalized quote streams
- Category-specific widget presets

### 💾 Save & Share

- **Like/Heart System:** Build personal offline quote library
- **Export Widget as Image:** Share exactly what you see on your home screen
- **Direct Sharing:** Share quotes to social media, messaging apps
- **Collection Management:** Organize favorites into custom lists

### 🎯 Designed for Focus

**Zero-Distraction Philosophy:**
- ❌ No onboarding tours cluttering UI
- ❌ No notification spam
- ❌ No dark patterns or manipulation tactics
- ❌ No feeds, timelines, or algorithmic recommendations
- ✅ Just the words that matter

---

## 🖼️ Widget Showcase

### Minimal Style
```
┌─────────────────────┐
│  "The only time      │
│   it's impossible    │
│   is when you        │
│   don't try"         │
│                      │
│    — Gintoki         │
│      Gintama         │
└─────────────────────┘
```

### Modern Style with Gradient
```
┌─────────────────────────────────┐
│ ╔═══════════════════════════╗  │
│ ║ 🌸 DAILY INSPIRATION      ║  │
│ ║                           ║  │
│ ║ "Success is not final,    ║  │
│ ║  failure is not fatal"    ║  │
│ ║                           ║  │
│ ║ — Churchill               ║  │
│ ║   Elite Mindset           ║  │
│ ╚═══════════════════════════╝  │
└─────────────────────────────────┘
```

### Glassmorphism Style
```
┌──────────────────────────────────┐
│░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░│
│░  "Discipline equals freedom"   ░│
│░                                ░│
│░  — Jocko Willink             ░│
│░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░│
└──────────────────────────────────┘
```

---

## 🛠️ Technical Stack

### Core Framework
| Component | Version | Purpose | Notes |
|-----------|---------|---------|-------|
| **Android SDK** | API 24-36 | Broad compatibility | Android 7.0 - Android 15 |
| **Kotlin** | Latest | Type-safe language | 100% codebase |
| **Jetpack Compose** | 2024.x+ | Modern declarative UI | Primary UI framework |
| **Glance** | Latest | App widget composition | Widget layer |

### Architecture & State Management
| Library | Version | Role | Implementation |
|---------|---------|------|-----------------|
| **Lifecycle** | Latest | Component lifecycle | Activity/Fragment mgmt |
| **ViewModel** | Latest | UI state preservation | Survives config changes |
| **Navigation Compose** | Latest | Type-safe routing | Screen navigation |
| **Coroutines** | Latest | Async programming | Dispatcher allocation |
| **Flow/StateFlow** | Latest | Reactive streams | State observation |

### Data & Persistence
| Library | Version | Use Case | Features |
|---------|---------|----------|----------|
| **Room** | Latest | Local database | Quote caching, offline |
| **DataStore** | Latest | Encrypted storage | User preferences, tokens |
| **Firebase Realtime DB** | BOM Latest | Cloud sync | Group quotes, sync |
| **Socket.io Client** | 2.1.0 | WebSocket | Real-time updates, groups |

### Networking & APIs
| Library | Version | Function | Security |
|---------|---------|----------|----------|
| **OkHttp** | Latest | HTTP client | Interceptors, TLS pinning |
| **Gson** | Latest | JSON parsing | Type-safe serialization |
| **Firebase Messaging** | Latest | Push notifications | Cloud messaging |
| **Coil** | Latest | Image loading | GPU acceleration, caching |

### Background Tasks & Sync
| Library | Version | Purpose | Scheduling |
|---------|---------|---------|-----------|
| **WorkManager** | Latest | Background work | Persistent scheduling |
| **Firebase Cloud Messaging** | Latest | Remote notifications | Push delivery |

### Analytics & Monetization
| Library | Version | Role | Data |
|---------|---------|------|------|
| **Firebase Analytics** | BOM Latest | Event tracking | User behavior metrics |
| **Google Play Services Ads** | Latest | Ad delivery | Banner/interstitial ads |
| **Google Play Services Auth** | Latest | Authentication | OAuth 2.0 sign-in |
| **Facebook SDK** | 18.1.3 | Social sharing | Share to Facebook |

---

## 🏗️ Architecture & Design Patterns

### Overall Architecture: MVVM (Model-View-ViewModel)

SenTense implements clean, scalable MVVM architecture with clear separation of concerns:

```
┌─────────────────────────────────────────────────────────────┐
│                  PRESENTATION LAYER                          │
│  ┌───────────────────────────────────────────────────────┐  │
│  │        Jetpack Compose UI Components                  │  │
│  │  • Screens (Home, Detail, Settings, Groups)           │  │
│  │  • Widgets (Custom reusable components)               │  │
│  │  • Previews (Development & testing)                   │  │
│  │  • Animations (Smooth transitions, scroll physics)    │  │
│  └───────────────────────────────────────────────────────┘  │
│                        ↓                                      │
│  ┌───────────────────────────────────────────────────────┐  │
│  │   ViewModel & State Management                        │  │
│  │  • StateFlow/LiveData (Reactive state)                │  │
│  │  • SharedFlow (One-time events)                       │  │
│  │  • Event handling & business logic                    │  │
│  └───────────────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────────────┘
                         ↓
┌─────────────────────────────────────────────────────────────┐
│                    DOMAIN LAYER                              │
│  ┌───────────────────────────────────────────────────────┐  │
│  │      Use Cases & Business Logic                       │  │
│  │  • GetDailyQuoteUseCase                               │  │
│  │  • FilterQuotesUseCase                                │  │
│  │  • UpdateWidgetUseCase                                │  │
│  │  • ShareToGroupUseCase                                │  │
│  │  • CreateGroupUseCase                                 │  │
│  └───────────────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────────────┘
                         ↓
┌─────────────────────────────────────────────────────────────┐
│                     DATA LAYER                               │
│  ┌──────────────────────────────────────────────────────┐   │
│  │         Repositories (Abstraction)                    │   │
│  │  • QuoteRepository                                    │   │
│  │  • UserRepository                                     │   │
│  │  • GroupRepository                                    │   │
│  └──────────────────────────────────────────────────────┘   │
│                 ↓            ↓            ↓                  │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐       │
│  │ Local Data   │  │ Remote Data  │  │   Cache      │       │
│  │ Source       │  │ Source       │  │   Layer      │       │
│  │ (Room DB)    │  │ (API/Socket) │  │ (In-memory)  │       │
│  └──────────────┘  └──────────────┘  └──────────────┘       │
│         ↓                   ↓                ↓                │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐       │
│  │ Room         │  │ OkHttp +     │  │ LRU Cache    │       │
│  │ Database     │  │ Socket.io    │  │ with TTL     │       │
│  │              │  │ + Firebase   │  │              │       │
│  └──────────────┘  └──────────────┘  └──────────────┘       │
└────────────────────────────────────────────────���────────────┘
```

### Design Patterns Implemented

#### 1. **Repository Pattern** (Data Abstraction)
Decouples UI from data sources, enabling testing and offline support through multiple data source coordination.

#### 2. **ViewModel Pattern with StateFlow**
Survives configuration changes, provides cancellation-safe operations, and reactive state management.

#### 3. **Singleton Pattern with Dependency Injection (Hilt)**
Ensures single instances of repositories and services across the application lifecycle.

#### 4. **Strategy Pattern** (Data Source Selection)
Switches between local, remote, and cached data sources based on network state and requirements.

#### 5. **Observer Pattern** (Flow-based Reactive)
UI observes state changes reactively through Kotlin Flow and StateFlow.

#### 6. **Factory Pattern** (Quote Creation)
Centralized quote creation with automatic ID generation and timestamp management.

---

## 💻 Installation & Setup

### Prerequisites
- **Android Studio:** Hedgehog or Flamingo+
- **JDK:** 17 or higher
- **Android SDK:** API 24+ (Android 7.0)
- **Gradle:** 8.x
- **Git:** Version control

### Step 1: Clone Repository
```bash
git clone https://github.com/zenforge-studios-dev/SenTense.git
cd SenTense
```

### Step 2: Configure Environment
```bash
# Verify gradle.properties
cat gradle.properties

# Expected:
# org.gradle.jvmargs=-Xmx2048m -Dfile.encoding=UTF-8
# org.gradle.configuration-cache=true
# android.useAndroidX=true
# kotlin.code.style=official
# android.nonTransitiveRClass=true
```

### Step 3: Set Up Firebase
```bash
# 1. Go to https://firebase.google.com/console
# 2. Create new project or select existing
# 3. Add Android app (Package: com.zenforge.studios.sentense)
# 4. Download google-services.json
# 5. Place file: app/google-services.json

# File structure:
app/
├── google-services.json    # ← Place here
└── build.gradle.kts
```

### Step 4: Configure API Keys
Create `local.properties` (if needed for local development):
```properties
api.base_url=https://api.sentense.com
api.socket_url=wss://socket.sentense.com
google_play_services_key=YOUR_FIREBASE_KEY
```

### Step 5: Open & Build
```bash
# Open in Android Studio
open -a "Android Studio" .

# Or build from command line
./gradlew clean build

# Build debug APK
./gradlew assembleDebug

# Install on device
./gradlew installDebug

# Run instrumented tests
./gradlew connectedAndroidTest

# Generate APK for testing
./gradlew bundleRelease
```

### Step 6: Verify Installation
```kotlin
// In MainActivity.kt:
override fun onCreate(savedInstanceState: Bundle?) {
    super.onCreate(savedInstanceState)
    
    Log.d("SenTense", "App initialized successfully")
    // Check Firebase initialization
    FirebaseApp.initializeApp(this)
}
```

---

## 🔧 Core Implementation Details

### 1. Real-time Quote Widget System

The widget system supports 7 different styles with live preview capabilities. Each style is a composable that can be customized through the settings screen.

**Key Features:**
- Dynamic styling based on user preferences
- Material Design 3 theming support
- Smooth animations and transitions
- Efficient rendering with Glance

### 2. Socket.io Real-time Updates

Real-time bidirectional communication for group quotes using Socket.io with automatic reconnection and comprehensive error handling.

**Key Features:**
- Automatic reconnection with exponential backoff
- Connection state tracking
- Real-time group quote delivery
- Event acknowledgment support

### 3. Group Management Repository

Coordinates Firebase Realtime Database, local Room database, and Socket.io for seamless group functionality.

**Key Features:**
- Multi-source data coordination
- Ephemeral quotes (2-hour expiration)
- Permission-based access control
- Offline group quote caching

### 4. Data Layer Architecture

Multi-layered caching strategy:
1. **L1 Cache:** In-memory LRU cache with TTL
2. **L2 Database:** Room local database for persistence
3. **L3 Remote:** API/Socket.io for fresh data

---

## 🤝 Contributing Guidelines

We welcome contributions! Please follow these guidelines:

### Code Standards
- **Language:** 100% Kotlin
- **Style:** Official Kotlin code style (ktlint)
- **Architecture:** Follow MVVM + Clean Architecture principles
- **Testing:** Write unit tests for business logic

### Commit Message Format
```
[type]: Brief description

[type] can be:
- feat: New feature
- fix: Bug fix
- docs: Documentation
- refactor: Code refactoring
- test: Adding/updating tests
- perf: Performance improvements
```

### Pull Request Process
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes with descriptive messages
4. Push to the branch
5. Open a Pull Request with a clear description

### Testing
- Write unit tests for all business logic
- Test edge cases and error scenarios
- Ensure all tests pass before submitting PR

---

## 📊 Project Statistics

- **Language:** Kotlin (100%)
- **Architecture:** MVVM + Clean Architecture
- **Minimum SDK:** API 24 (Android 7.0)
- **Target SDK:** API 36+ (Android 15+)
- **Widget Styles:** 7 customizable designs
- **Group Permissions:** 4 role-based levels
- **Quote Categories:** 5 curated categories

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🔗 Links

- **[Google Play Store](https://play.google.com/store/apps/details?id=com.zenforge.studios.sentense)**
- **[Zenforge Studios](https://github.com/zenforge-studios-dev)**
- **[Android Documentation](https://developer.android.com/)**
- **[Jetpack Compose](https://developer.android.com/jetpack/compose)**

---

**Built with ❤️ by Zenforge Studios**