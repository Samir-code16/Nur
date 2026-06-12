# Setting Up Permissions in Xcode

Since this project uses auto-generated Info.plist, you need to add permissions via Xcode's project settings.

## Steps to Add Permissions:

1. **Open the Project in Xcode**
   - Open `Nur.xcodeproj`

2. **Select the Target**
   - Click on "Nur" in the Project Navigator (left sidebar)
   - Select the "Nur" target (under TARGETS)

3. **Go to Info Tab**
   - Click on the "Info" tab at the top

4. **Add Custom iOS Target Properties**
   - Click the "+" button to add new keys
   - Add the following keys with their descriptions:

### Required Permissions:

#### Location Permission (When In Use)
- **Key:** `Privacy - Location When In Use Usage Description`
- **Type:** String
- **Value:** `Nur needs your location to provide accurate prayer times and find nearby mosques.`

#### Location Permission (Always)
- **Key:** `Privacy - Location Always and When In Use Usage Description`
- **Type:** String
- **Value:** `Nur needs your location to provide accurate prayer times and find nearby mosques.`

#### Microphone Permission
- **Key:** `Privacy - Microphone Usage Description`
- **Type:** String
- **Value:** `Nur needs microphone access for Quran recitation practice and voice recognition.`

### Background Modes (Optional)

If you want background location updates:
1. Go to the "Signing & Capabilities" tab
2. Click "+ Capability"
3. Add "Background Modes"
4. Check "Location updates" and "Audio, AirPlay, and Picture in Picture"

## Alternative: Using Info.plist File

If you prefer using an Info.plist file:

1. Remove `GENERATE_INFOPLIST_FILE = YES` from build settings
2. Set `INFOPLIST_FILE = Nur/Info.plist` in build settings
3. Keep the Info.plist file in the project

The current setup uses auto-generated Info.plist, so permissions should be added via the Info tab as described above.
