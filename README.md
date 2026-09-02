# Minya Tourism Mobile App

A comprehensive Flutter mobile application showcasing the hidden treasures of Minya, Egypt. This app serves as a complete tourism guide featuring ancient attractions, local culture, hotels, restaurants, events, and travel experiences.

## 🌟 Features

### Core Functionality
- **Interactive Home Screen** with featured attractions carousel
- **Attractions Guide** with detailed information about historical sites
- **Hotels Directory** with ratings, amenities, and booking information
- **Restaurants Guide** featuring local cuisine and specialties
- **Events Calendar** showcasing cultural events and festivals
- **Trip Itineraries** with pre-planned and custom trip options
- **Visitor Information** including transportation, weather, and travel tips
- **Blog & Stories** featuring travel experiences and cultural insights
- **Interactive Map** with location-based services
- **Multilingual Support** (Arabic/English)

### Design Highlights
- **Outstanding UI/UX** with tourism-themed visuals
- **Egyptian Heritage Design** featuring authentic colors and patterns
- **Responsive Layout** optimized for mobile devices
- **Smooth Animations** and transitions
- **Custom Icons** and illustrations
- **Professional Typography** with excellent readability

### Technical Features
- **Flutter Framework** for cross-platform compatibility
- **Material Design 3** components
- **Local Asset Management** for offline functionality
- **Modular Architecture** with clean code structure
- **State Management** with proper data flow
- **Performance Optimized** with tree-shaking and asset optimization

## 🏛️ About Minya

Minya is a historic city in Upper Egypt, known for its rich archaeological heritage and stunning Nile River views. The city serves as a gateway to some of Egypt's most important historical sites, including:

- **Beni Hassan Tombs** - Middle Kingdom rock-cut tombs with preserved wall paintings
- **Tuna el-Gebel** - Ancient necropolis with Greco-Roman influences
- **Tell el-Amarna** - Capital city during Akhenaten's reign
- **Minya Corniche** - Beautiful Nile waterfront promenade

## 🚀 Getting Started

### Prerequisites
- Flutter SDK (3.1.0 or higher)
- Dart SDK
- Android Studio / VS Code
- Git

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd minya_tourism_app
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Run the app**
   ```bash
   # For web
   flutter run -d web-server --web-port=8080

   # For mobile (with connected device/emulator)
   flutter run
   ```

4. **Build for production**
   ```bash
   # Web build
   flutter build web

   # Android APK
   flutter build apk

   # iOS (requires macOS)
   flutter build ios
   ```

## 📱 App Structure

```
lib/
├── core/
│   ├── models/          # Data models
│   ├── services/        # Business logic and data services
│   └── theme/           # App theming and styling
├── features/
│   ├── attractions/     # Attractions screens and widgets
│   ├── blog/           # Blog and stories functionality
│   ├── events/         # Events and calendar features
│   ├── home/           # Home screen and navigation
│   ├── hotels/         # Hotels directory
│   ├── itineraries/    # Trip planning features
│   ├── map/            # Interactive map functionality
│   ├── restaurants/    # Restaurants guide
│   ├── splash/         # Splash screen
│   └── visitor_info/   # Visitor information and tips
└── main.dart           # App entry point
```

## 🎨 Design System

### Color Palette
- **Primary**: Deep Blue (#1A365D) - Representing the Nile River
- **Secondary**: Golden Sand (#D4A574) - Egyptian desert heritage
- **Accent**: Terracotta (#B85450) - Ancient pottery and artifacts
- **Background**: Light Cream (#F7F5F3) - Papyrus and limestone

### Typography
- **Headers**: Bold, readable fonts for titles
- **Body**: Clean, legible text for content
- **Captions**: Subtle styling for secondary information

### Visual Elements
- **Egyptian Patterns**: Subtle background textures
- **Authentic Photography**: High-quality images of Minya attractions
- **Custom Icons**: Tourism-specific iconography
- **Smooth Animations**: Engaging user interactions

## 🔧 Dependencies

### Core Dependencies
- `flutter`: SDK framework
- `cupertino_icons`: iOS-style icons
- `google_maps_flutter`: Interactive maps
- `carousel_slider`: Image carousels
- `http`: Network requests
- `cached_network_image`: Optimized image loading
- `flutter_rating_bar`: Star ratings
- `shared_preferences`: Local storage

### Development Dependencies
- `flutter_test`: Testing framework
- `flutter_lints`: Code quality analysis

## 📸 Screenshots

The app features:
- Elegant splash screen with Egyptian motifs
- Interactive home screen with attraction carousel
- Detailed attraction pages with image galleries
- Comprehensive hotel and restaurant listings
- Event calendar with cultural activities
- Trip planning and itinerary tools
- Interactive map with location markers
- Visitor information and travel tips

## 🌍 Localization

The app supports multiple languages:
- **Arabic** (العربية) - Primary language for local users
- **English** - International tourists and visitors

## 🚀 Performance

- **Optimized Assets**: Tree-shaken fonts and compressed images
- **Efficient Rendering**: Smooth 60fps animations
- **Memory Management**: Proper widget lifecycle handling
- **Network Optimization**: Cached images and efficient data loading

## 📱 Platform Support

- **Android**: API level 21+ (Android 5.0+)
- **iOS**: iOS 11.0+
- **Web**: Modern browsers with Flutter Web support
- **Desktop**: Windows, macOS, Linux (with Flutter Desktop)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Egyptian Ministry of Tourism** for cultural information
- **Minya Tourism Authority** for local insights
- **Flutter Community** for excellent documentation and support
- **Egyptian Heritage Foundation** for historical accuracy

## 📞 Support

For support and inquiries:
- **Email**: support@minyatourism.app
- **Website**: https://minyatourism.app
- **Documentation**: https://docs.minyatourism.app

---

**Discover the hidden treasures of Minya, Egypt** 🏛️✨

*Built with ❤️ using Flutter*
