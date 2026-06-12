# Nur - Islamic Lifestyle App

A holistic Islamic lifestyle mobile application designed to support Muslims in their daily worship, spiritual growth, and mental well-being.

## Features

### 🕌 Prayer Module
- **5-Card Layout:**
  - Current prayer display
  - Next prayer with countdown timer
  - Daily prayer overview
  - Nearby mosque prayer times
  - Settings & adjustments
- Accurate prayer times based on location and calculation method
- Multiple calculation methods (Muslim World League, Egyptian, Karachi, etc.)
- Madhab selection (Hanafi, Shafi'i)
- Location-based prayer time calculation

### 📖 Quran Module
- **Reading Mode:** Browse and read Quran verses
- **Recitation Mode:** Voice recognition for recitation practice with AI-assisted feedback
- **Memorization Tracker:** Track your memorization progress verse by verse
- **AI-Powered Tafsir:** Context-aware explanations with simple and advanced modes

### 🧘 Wudu & Salah Guidance
- Step-by-step wudu walkthrough with visual and audio guidance
- Step-by-step salah guide for all five daily prayers
- Beginner-friendly mode with detailed instructions
- Option to hide guidance for advanced users

### 🕌 Mosque Locator
- Location-based mosque finder
- Distance calculation and navigation support
- Display of mosque prayer times
- Filter by facilities (Jumu'ah, women's area, parking)
- Detailed mosque information and contact details

### 💚 Wellness & Mindfulness
- **Dhikr Counter:** Guided dhikr with recommended counts
- **Meditation Sessions:** Islamic meditation with breath-focused exercises
- **Sleep Playlists:** Quran recitation, duas, and adhkar for peaceful sleep
- Auto-stop and fade-out options for sleep content

### 🎨 Design & Personalization
- Soft neutral color palette with gold accents
- Minimalist, calming UI
- Automatic light/dark theme switching based on time
- Night theme before Fajr
- Smooth animations and subtle transitions
- Accessible typography for Arabic and translations

## Architecture

### Models
- `PrayerModels.swift` - Prayer types, times, settings, calculation methods
- `MosqueModels.swift` - Mosque data structures and filters
- `QuranModels.swift` - Quran verses, surahs, recitation sessions, tafsir

### Services
- `PrayerTimeService.swift` - Prayer time calculation
- `LocationService.swift` - Location management and permissions
- `ThemeService.swift` - Theme management and auto-switching

### Views
- **Prayer:** Complete prayer module with 5-card layout
- **Quran:** Reading, recitation, and memorization views
- **Wellness:** Dhikr, meditation, and sleep playlists
- **Mosque:** Locator with search and filters
- **Wudu/Salah:** Step-by-step guidance views

## Requirements

- iOS 17.0+
- Xcode 15.0+
- Swift 5.9+

## Permissions

The app requires the following permissions:
- **Location:** For accurate prayer times and mosque locator
- **Microphone:** For Quran recitation practice (optional)

## Setup

1. Clone the repository
2. Open `Nur.xcodeproj` in Xcode
3. Build and run on a simulator or device

## Future Enhancements

- Lock screen widget for prayer times
- Community features (circles, shared goals)
- Scholar-verified content badges
- Wearable device integration
- Multilingual support
- Enhanced prayer time calculation library integration
- Real-time mosque data from APIs
- Cloud sync for memorization progress

## License

Copyright © 2026 Shieraaz Williams. All rights reserved.
