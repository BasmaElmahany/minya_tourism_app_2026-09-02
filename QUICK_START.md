# Quick Start Guide - Minya Tourism App

## 🚀 Getting Started

### 1. Extract the App
```bash
unzip minya_tourism_app_updated.zip
cd minya_tourism_app_corrected/modified_app
```

### 2. Install Dependencies
```bash
flutter pub get
```

### 3. Run the App
```bash
# On Android emulator/device
flutter run

# On iOS simulator (Mac only)
flutter run -d ios

# On Chrome (for testing)
flutter run -d chrome
```

---

## 🌤️ Enable Real-Time Weather (Optional but Recommended)

### Step 1: Get API Key
1. Visit https://openweathermap.org/api
2. Click "Sign Up" (it's free!)
3. Verify your email
4. Go to "API Keys" section
5. Copy your API key

### Step 2: Add API Key to App
1. Open `lib/core/services/weather_service.dart`
2. Find line 8: `static const String apiKey = 'YOUR_API_KEY_HERE';`
3. Replace `YOUR_API_KEY_HERE` with your actual API key
4. Save the file

### Step 3: Test Weather
1. Run the app
2. Navigate to "Weather" from the More tab
3. You should see real-time weather for Minya!

---

## 📱 New Features to Try

### 1. Services Page
- Open the app
- Go to "More" tab (bottom navigation)
- Tap on "Services"
- Try filtering by category (Hospitals, Banks, etc.)

### 2. Updated Card Designs
- Check the home page
- Scroll through "Popular Places"
- Notice the improved card designs with proper images and text

### 3. Weather with Refresh
- Go to Weather page
- Tap the refresh icon (top right)
- See updated weather data

---

## 🎨 Color Scheme

The app now uses a **sandy gold pyramid theme**:
- Primary: Sandy Gold (#C9A961)
- Secondary: Saddle Brown (#8B4513)
- Accents: Light gold, bronze, terracotta

---

## 📂 Project Structure

```
lib/
├── core/
│   ├── models/           # Data models
│   ├── services/         # API and data services
│   ├── theme/           # App theme and colors
│   └── providers/       # State management
├── features/
│   ├── home/            # Home screen
│   ├── services/        # NEW: Services page
│   ├── weather/         # Updated weather
│   ├── hotels/          # Hotels listing
│   ├── attractions/     # Tourist attractions
│   └── ...
└── main.dart            # App entry point
```

---

## 🔧 Troubleshooting

### Issue: "Packages not found"
**Solution**: Run `flutter pub get`

### Issue: "Weather not updating"
**Solution**: Make sure you've added your API key (see above)

### Issue: "Build failed"
**Solution**: 
```bash
flutter clean
flutter pub get
flutter run
```

### Issue: "Images not loading"
**Solution**: Make sure all images are in `assets/images/` folder

---

## 📝 Important Notes

1. **Weather API**: Free tier allows 1,000 calls/day (more than enough!)
2. **Images**: Make sure to add your actual images to `assets/images/`
3. **Data**: Services data is integrated; other data can be added similarly
4. **Testing**: Test on both light and dark modes

---

## ✅ Checklist

- [ ] Extracted the app
- [ ] Ran `flutter pub get`
- [ ] App runs successfully
- [ ] Added weather API key (optional)
- [ ] Tested Services page
- [ ] Checked card designs
- [ ] Tested on different screen sizes
- [ ] Verified dark mode works

---

## 🎯 Next Steps

1. **Add Your Images**: Replace placeholder images with actual photos
2. **Customize Content**: Update text and descriptions
3. **Add More Services**: Expand the services database
4. **Test Thoroughly**: Try all features on different devices
5. **Deploy**: Build for production when ready

---

## 📞 Need Help?

If you encounter any issues or need modifications, just let me know!

---

**Happy Coding! 🚀**

