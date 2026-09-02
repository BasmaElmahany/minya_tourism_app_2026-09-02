# Minya Tourism App - Redesigned

## 🎨 What's New

This redesigned version of the Minya Tourism App features a modern, trendy UI/UX with comprehensive theming and localization support.

### ✨ Key Features

#### 1. **Modern Dark & Light Themes**
- **Light Mode**: Clean, professional design with vibrant orange accents (#FF6B35) and deep blue-gray primary colors (#2E5266)
- **Dark Mode**: Sophisticated dark slate background (#0F172A) with the same vibrant accents for consistency
- Smooth transitions between themes
- Theme preference saved automatically

#### 2. **English & Arabic Language Support**
- Full bilingual support with instant language switching
- RTL (Right-to-Left) layout for Arabic
- All UI elements translated
- Language preference saved automatically

#### 3. **Redesigned Screens**

##### Home Screen
- Modern header with quick access to theme, language, and settings
- Beautiful hero carousel with gradient overlays
- Grid-based quick actions with colorful icons
- Popular attractions with modern card design
- Upcoming events section

##### Attractions Screen
- Category filtering with modern pill buttons
- Grid and list view options
- Beautiful image cards with ratings and prices
- Smooth navigation

##### Restaurants Screen
- Full-width cards with large images
- Rating badges and price indicators
- "Book Now" call-to-action buttons
- Modern layout inspired by top travel apps

##### Hotels Screen
- Grid layout with compact cards
- Star ratings and price ranges
- Favorite button for quick access
- Clean, modern design

##### Settings Screen
- Dedicated settings page for theme and language control
- Visual theme selector with light/dark mode options
- Language selector with flag indicators
- About section with app information

### 🎨 Design Inspiration

The redesign draws inspiration from modern travel apps like:
- Clean, card-based layouts
- Bold, vibrant accent colors
- Generous use of white space (or dark space in dark mode)
- Modern rounded corners (20px radius)
- Subtle shadows and elevation
- Beautiful imagery with gradient overlays

### 🎯 Color Palette

#### Light Mode
- **Primary**: #2E5266 (Deep Blue-Gray)
- **Secondary**: #FF6B35 (Vibrant Orange)
- **Accent**: #6C63FF (Modern Purple)
- **Background**: #F8F9FA (Soft White)
- **Surface**: #FFFFFF (Pure White)

#### Dark Mode
- **Primary**: #1E293B (Dark Slate)
- **Secondary**: #FF6B35 (Vibrant Orange - same)
- **Accent**: #8B7EFF (Lighter Purple)
- **Background**: #0F172A (Very Dark Blue)
- **Surface**: #1E293B (Dark Slate)
- **Card Background**: #334155 (Medium Dark Slate)

### 📦 New Dependencies

The following packages were added to support the new features:

```yaml
dependencies:
  provider: ^6.1.1  # State management for theme and language
```

### 🏗️ Architecture

#### New Files Added:
- `lib/core/providers/theme_provider.dart` - Theme state management
- `lib/core/providers/language_provider.dart` - Language state management
- `lib/core/localization/app_localizations.dart` - Localization strings
- `lib/features/settings/settings_screen.dart` - Settings UI

#### Modified Files:
- `lib/main.dart` - Added providers and theme support
- `lib/core/theme/app_theme.dart` - Complete theme redesign
- `lib/features/home/home_screen.dart` - Modern UI redesign
- `lib/features/attractions/attractions_screen.dart` - Modern UI redesign
- `lib/features/restaurants/restaurants_screen.dart` - Modern UI redesign
- `lib/features/hotels/hotels_screen.dart` - Modern UI redesign
- `lib/features/splash/splash_screen.dart` - Theme support added

### 🚀 How to Use

#### Theme Switching
1. Tap the sun/moon icon in the home screen header
2. Or go to Settings → Theme and select your preference

#### Language Switching
1. Tap the language button (EN/ع) in the home screen header
2. Or go to Settings → Language and select your preference

#### Settings Access
- Tap the settings icon (⚙️) in the home screen header
- Or navigate through the app menu

### 📱 Responsive Design

The app is fully responsive and adapts to:
- Different screen sizes
- Portrait and landscape orientations
- RTL layout for Arabic language
- Dark and light themes

### 🎭 Theme Persistence

Both theme and language preferences are automatically saved using SharedPreferences and persist across app restarts.

### 🌍 Localization Coverage

All major UI elements are localized including:
- Navigation labels
- Screen titles
- Buttons and actions
- Common phrases
- Settings options

### 💡 Best Practices Implemented

1. **Provider Pattern**: Clean state management
2. **Material Design 3**: Modern UI components
3. **Responsive Layouts**: Adapts to all screen sizes
4. **Accessibility**: High contrast colors, readable fonts
5. **Performance**: Efficient rebuilds with Consumer widgets
6. **Code Organization**: Clear separation of concerns

### 🔧 Installation & Running

```bash
# Extract the archive
tar -xzf minya_tourism_app_redesigned.tar.gz

# Navigate to the project
cd minya_tourism_app

# Install dependencies
flutter pub get

# Run the app
flutter run
```

### 📝 Notes

- All images and assets from the original app are preserved
- The app maintains backward compatibility with existing data
- No breaking changes to the core functionality
- All existing features work as before with enhanced UI

### 🎉 Enjoy the New Design!

The app now features a modern, professional design that rivals top travel applications while maintaining the unique character of Minya Tourism.
