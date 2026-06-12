# Nur Project Structure

## Directory Organization

```
Nur/
├── Design/
│   └── ColorScheme.swift          # Design system with colors and themes
│
├── Models/
│   ├── PrayerModels.swift         # Prayer types, times, settings, calculation methods
│   ├── MosqueModels.swift         # Mosque data structures
│   └── QuranModels.swift          # Quran verses, surahs, recitation, tafsir
│
├── Services/
│   ├── PrayerTimeService.swift    # Prayer time calculation logic
│   ├── LocationService.swift      # Location management
│   └── ThemeService.swift         # Theme and personalization
│
├── Views/
│   ├── MainTabView.swift          # Main tab navigation
│   ├── ContentView.swift           # Root view
│   │
│   ├── Prayer/
│   │   ├── PrayerView.swift        # Main prayer view with 5-card layout
│   │   ├── CurrentPrayerCard.swift
│   │   ├── NextPrayerCard.swift
│   │   ├── DailyPrayerOverviewCard.swift
│   │   ├── MosquePrayerTimesCard.swift
│   │   ├── PrayerSettingsCard.swift
│   │   ├── PrayerSettingsView.swift
│   │   ├── PrayerCardView.swift
│   │   └── WuduSalahGuideCard.swift
│   │
│   ├── Quran/
│   │   ├── QuranView.swift         # Main Quran view with tabs
│   │   ├── RecitationView.swift    # Voice recognition for recitation
│   │   └── TafsirView.swift         # AI-powered tafsir display
│   │
│   ├── Wellness/
│   │   ├── WellnessView.swift      # Main wellness view
│   │   ├── DhikrView.swift          # Dhikr counter
│   │   ├── MeditationView.swift    # Meditation sessions
│   │   └── SleepPlaylistView.swift # Sleep audio playlists
│   │
│   ├── Mosque/
│   │   └── MosqueLocatorView.swift # Mosque finder with map integration
│   │
│   └── WuduSalah/
│       ├── WuduGuideView.swift     # Step-by-step wudu guide
│       └── SalahGuideView.swift    # Step-by-step salah guide
│
├── Info.plist                      # App permissions and configuration
└── NurApp.swift                     # App entry point
```

## Key Features Implementation

### Prayer Module ✅
- Complete 5-card layout implemented
- Real-time countdown for next prayer
- Location-based prayer time calculation
- Multiple calculation methods and madhabs
- Settings management

### Quran Module ✅
- Reading interface with verse display
- Recitation view with voice recognition structure
- Tafsir view with simple/advanced modes
- Memorization tracking structure

### Wellness Module ✅
- Dhikr counter with recommended counts
- Meditation sessions with timers
- Sleep playlists with auto-stop and fade-out

### Mosque Locator ✅
- Location-based search
- Filtering by facilities
- Distance calculation
- Map integration for directions

### Wudu & Salah Guides ✅
- Step-by-step wudu walkthrough
- Salah guide for all prayers
- Beginner/advanced modes

### Personalization ✅
- Auto theme switching based on time
- Soft neutral palette with gold accents
- Smooth animations

## Next Steps

1. **Widget Extension** (Lock Screen Widget)
   - Create a new Widget Extension target
   - Implement PrayerTimeWidget
   - Add timeline provider for updates

2. **Enhanced Features**
   - Integrate proper prayer time calculation library (e.g., Adhan-Swift)
   - Connect to mosque data API
   - Implement real voice recognition for recitation
   - Add cloud sync for user data
   - Implement offline mode for core features

3. **Testing**
   - Unit tests for services
   - UI tests for critical flows
   - Prayer time calculation accuracy tests

4. **Localization**
   - Arabic language support
   - Additional language support
   - RTL layout support

## Notes

- Prayer time calculation is currently simplified - integrate a proper library for production
- Mosque data is sample data - connect to real API
- Voice recognition structure is in place but needs actual implementation
- Widget requires separate extension target (not included in initial build)
