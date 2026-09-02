# Quick Setup Guide - Attraction Details Update

## Prerequisites
- Flutter SDK (3.5.4 or higher)
- Android Studio / Xcode
- Google Maps API Key (for both Android and iOS)

## Installation Steps

### 1. Extract and Setup Project
```bash
# Extract the project
unzip minya_tourism_app_updated.zip
cd minya_tourism_app

# Install dependencies
flutter pub get
```

### 2. Configure Google Maps API Key

#### For Android:
1. Open `android/app/src/main/AndroidManifest.xml`
2. Find the line with `YOUR_GOOGLE_MAPS_API_KEY`
3. Replace it with your actual Google Maps API key:
```xml
<meta-data
    android:name="com.google.android.geo.API_KEY"
    android:value="AIzaSy...your-actual-key-here"/>
```

#### For iOS:
1. Open `ios/Runner/AppDelegate.swift`
2. Add the following import at the top:
```swift
import GoogleMaps
```
3. Add this line in the `application` method before `return`:
```swift
GMSServices.provideAPIKey("YOUR_GOOGLE_MAPS_API_KEY")
```

### 3. Get Google Maps API Key

If you don't have a Google Maps API key:

1. Go to [Google Cloud Console](https://console.cloud.google.com/)
2. Create a new project or select existing one
3. Enable these APIs:
   - Maps SDK for Android
   - Maps SDK for iOS
   - Directions API (for route information)
4. Go to "Credentials" and create an API key
5. (Optional) Restrict the API key to your app's package name

### 4. Run the Application

```bash
# For Android
flutter run

# For iOS (on macOS only)
cd ios
pod install
cd ..
flutter run
```

### 5. Grant Permissions

When you first run the app:
- Allow location permissions when prompted
- This is required for the directions and route features

## Key Features to Test

1. **Open Attraction Details**: Tap any attraction from the list
2. **View Map**: See the attraction location on Google Maps
3. **Get Directions**: Tap "Directions" button to open Google Maps
4. **Check Route Info**: View driving and walking duration estimates
5. **Save to Favorites**: Tap "Save" button to add to favorites
6. **Share Location**: Tap share icon to share the attraction
7. **Check Ticket Info**: See "Free" or "Tickets" button based on attraction

## Troubleshooting

### Map Not Showing
- Verify Google Maps API key is correctly added
- Check that Maps SDK for Android/iOS is enabled in Google Cloud Console
- Ensure internet permission is granted

### Location Not Working
- Check location permissions in device settings
- Verify location services are enabled on the device
- Check AndroidManifest.xml and Info.plist have correct permissions

### Directions Not Opening
- Ensure Google Maps app is installed on the device
- Check internet connection
- Verify url_launcher package is working

### Share Not Working
- Check that share_plus package is properly installed
- Run `flutter pub get` again
- Verify platform-specific configurations

## File Structure

```
lib/
├── core/
│   ├── data/
│   │   └── attractions_data.dart          # Updated with isFree and bookingUrl
│   ├── models/
│   │   └── tourism_models.dart            # Updated Attraction model
│   └── providers/
│       └── favorites_provider.dart        # Updated with add/remove methods
└── features/
    └── attractions/
        └── attraction_details_screen.dart # Completely rewritten
```

## Important Notes

1. **API Key Security**: Never commit your API key to version control
2. **Production Build**: Add API key restrictions before deploying to production
3. **Route Calculation**: Current implementation uses approximate calculations. For production, integrate Google Directions API
4. **Booking URLs**: Update the `bookingUrl` field in `attractions_data.dart` for attractions with online booking

## Next Steps

1. Add your Google Maps API key
2. Test all features on both Android and iOS
3. Update booking URLs for attractions that support online booking
4. Customize the route calculation with Google Directions API (optional)
5. Add more attractions with complete data

## Additional Resources

- [Google Maps Flutter Plugin](https://pub.dev/packages/google_maps_flutter)
- [Geolocator Package](https://pub.dev/packages/geolocator)
- [Share Plus Package](https://pub.dev/packages/share_plus)
- [Google Maps Platform Documentation](https://developers.google.com/maps/documentation)

## Support

For detailed information about the changes, see `ATTRACTION_DETAILS_UPDATE.md`

