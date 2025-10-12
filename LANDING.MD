# 📖 Quran Hafiz - Master the Quran, One Ayah at a Time

<div align="center">
  <img src="assets/img/logo.svg" alt="Quran Hafiz Logo" width="120" height="120">
  
  **A Flutter application designed to help Muslims test and improve their Quran memorization skills through interactive audio-based testing.**
  
  [![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)](https://flutter.dev/)
  [![Dart](https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white)](https://dart.dev/)
  [![License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
  [![Version](https://img.shields.io/badge/Version-25.10.08%2B13-blue.svg?style=for-the-badge)](https://github.com/bynalab/hafiz_test)
</div>

### 🎨 **App Color Scheme**
- **Primary Color**: `#004B40` (Dark Teal) - Main brand color
- **Light Theme**: Clean white background with dark teal accents
- **Dark Theme**: Dark backgrounds (`#0E0E0E`, `#121212`) with teal highlights (`#0BB38A`)
- **Card Colors**: 
  - Quran Reading: `#2BFF00` (Bright Green)
  - Surah Testing: `#FF8E6F` (Coral Orange)  
  - Juz Testing: `#FBBE15` (Golden Yellow)
  - Random Testing: `#6E81F6` (Purple Blue)
- **Splash Screen**: Gradient from `#0D324D` to `#093028` with star animations

---

## 🌟 Key Features

### 🎯 **Interactive Memorization Testing**
- **Random Verse Testing**: Generate random verses from random chapters and complete them where the reciter stops
- **Multiple Test Modes**:
  - 📖 **Test by Surah (Chapter)** - Focus on specific chapters
  - 📚 **Test by Juz (Part)** - Test by 30 parts of the Quran
  - 🎲 **Random Testing** - Test across the entire Quran
- **Progress Tracking**: Save and continue from your last read position
- **Smart Analytics**: Track your memorization progress and improvement

### 🎵 **Premium Audio Experience**
- **20+ Renowned Reciters**: Choose from Abdul Basit, Sudais, Alafasy, Maher Al Muaiqly, and many more
- **Multi-language Support**: Arabic, English, French, Chinese, Russian, Urdu, and Persian recitations
- **Advanced Playback Controls**: Play, pause, seek, and adjust playback speed
- **Background Playback**: Continue listening while using other apps
- **Loop Modes**: Repeat verses for better memorization
- **High-Quality Audio**: Crystal clear recitation for optimal learning

### 🎨 **Beautiful User Experience**
- **Modern UI Design**: Clean, intuitive interface with Arabic typography support
- **Responsive Design**: Optimized for phones, tablets, and different screen sizes
- **Dark/Light Theme**: Customizable appearance to match your preference
- **Interactive User Guide**: Built-in showcase to help new users navigate the app
- **Last Read Card**: Quick access to continue from where you left off

### ⚙️ **Advanced Features**
- **Settings Management**: Customize reciter, autoplay, and other preferences
- **Offline Support**: Download and listen without internet connection
- **Progress Analytics**: Detailed insights into your memorization journey
- **Rating System**: Built-in feedback system for continuous improvement
- **Bug Reporting**: Easy way to report issues and suggest improvements

---

## 📱 Screenshots & Demo

### Main Menu Interface
<div align="center">
  <img src="assets/img/card_quran.png" alt="Quran Reading Card - Bright Green" width="200">
  <img src="assets/img/card_surah.png" alt="Surah Testing Card - Coral Orange" width="200">
  <img src="assets/img/card_juz.png" alt="Juz Testing Card - Golden Yellow" width="200">
  <img src="assets/img/card_random.png" alt="Random Testing Card - Purple Blue" width="200">
</div>

### App Visual Elements
<div align="center">
  <img src="assets/img/quran_opened_star.png" alt="Quran Reading Interface" width="200">
  <img src="assets/img/vector_quran.png" alt="Quran Vector Design" width="200">
  <img src="assets/img/faded_vector_quran.png" alt="Quran Background" width="200">
</div>

### Color-Coded Features
- 🟢 **Quran Reading**: Bright green (`#2BFF00`) for easy access to Quran text
- 🟠 **Surah Testing**: Coral orange (`#FF8E6F`) for chapter-based memorization
- 🟡 **Juz Testing**: Golden yellow (`#FBBE15`) for part-based learning
- 🔵 **Random Testing**: Purple blue (`#6E81F6`) for comprehensive challenges

---

## 🚀 Download & Installation

### 📱 **Mobile Apps**

#### Android
- **Google Play Store**: [Download APK](https://github.com/bynalab/hafiz_test/releases) *(Coming Soon)*
- **Direct APK**: Download from [Releases](https://github.com/bynalab/hafiz_test/releases/latest)
- **Minimum Requirements**: Android 5.0 (API level 21)

#### iOS
- **App Store**: [Download](https://apps.apple.com/app/quran-hafiz) *(Coming Soon)*
- **Minimum Requirements**: iOS 12.0 or later

### 💻 **Desktop Support**
- **Windows**: Available through Flutter desktop
- **macOS**: Available through Flutter desktop
- **Linux**: Available through Flutter desktop

---

## 🛠️ Development Setup

### Prerequisites
- Flutter SDK (>=3.4.0)
- Dart SDK
- Android Studio / VS Code
- Android device or emulator (iOS support available)

### Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/bynalab/hafiz_test.git
   cd hafiz_test
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Run the app**
   ```bash
   flutter run
   ```

### Building for Production

#### Android
```bash
flutter build apk --release
# or for app bundle
flutter build appbundle --release
```

#### iOS
```bash
flutter build ios --release
```

---

## 🏗️ Technical Architecture

### **Project Structure**
```
lib/
├── data/                    # Static data files
│   ├── juz_list.dart       # Juz (Part) definitions
│   ├── reciters.dart       # Available reciters
│   └── surah_list.dart     # Surah (Chapter) list
├── services/               # Business logic services
│   ├── audio_services.dart
│   ├── analytics_service.dart
│   ├── rating_service.dart
│   └── storage/            # Storage implementations
├── quran/                  # Quran-related functionality
├── surah/                  # Surah-related screens
├── juz/                    # Juz-related screens
├── widget/                 # Reusable UI components
└── util/                   # Utility classes
```

### **Key Dependencies**
- **Flutter**: Modern UI framework
- **just_audio**: Advanced audio playback
- **dio**: HTTP client for API calls
- **shared_preferences**: Local data storage
- **get_it**: Dependency injection
- **google_fonts**: Beautiful typography
- **showcaseview**: User onboarding

---

## 🧪 Testing & Quality

### **Comprehensive Test Coverage**
```bash
# Run all tests
flutter test

# Run tests with coverage
flutter test --coverage
```

### **Test Structure**
- **Unit Tests**: Service layer testing with mocked dependencies
- **Widget Tests**: UI component testing
- **Integration Tests**: End-to-end user flow testing

---

## 📊 Analytics & Privacy

### **Analytics Features**
- **Usage Tracking**: Understand how users interact with the app
- **Performance Monitoring**: Track app performance and stability
- **User Journey**: Analyze user behavior for continuous improvement

### **Privacy First**
- **No Personal Data Collection**: We don't collect personal information
- **Local Storage**: All user data stored locally on device
- **Transparent Analytics**: Open source analytics implementation

---

## 🤝 Contributing

We welcome contributions from the community! Here's how you can help:

### **Ways to Contribute**
1. **Bug Reports**: Report issues you encounter
2. **Feature Requests**: Suggest new features
3. **Code Contributions**: Submit pull requests
4. **Documentation**: Improve our documentation
5. **Translations**: Help translate the app

### **Development Guidelines**
- Follow Flutter/Dart style guidelines
- Write tests for new features
- Update documentation as needed
- Ensure all tests pass before submitting PR

### **Getting Started**
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📞 Support & Community

### **Getting Help**
- **GitHub Issues**: [Report bugs or request features](https://github.com/bynalab/hafiz_test/issues)
- **Discussions**: [Join community discussions](https://github.com/bynalab/hafiz_test/discussions)
- **Email**: Contact the development team

### **Community Guidelines**
- Be respectful and inclusive
- Help others learn and grow
- Share knowledge and experiences
- Follow Islamic principles in all interactions

---

## 🔄 Version History

### **Current Version: 25.10.08+13**
- ✅ Enhanced analytics and user tracking
- ✅ Improved audio playback experience
- ✅ Better user interface and navigation
- ✅ Comprehensive testing coverage
- ✅ Performance optimizations

### **Previous Versions**
- **v25.09.03+12**: Initial release with core features
- **v25.08.15+10**: Audio improvements and bug fixes
- **v25.07.20+8**: UI enhancements and new features

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

### **Special Thanks**
- **Quran API**: For providing Quran text and audio data
- **Reciters**: All the talented Quran reciters whose audio is used
- **Flutter Community**: For the excellent packages and support
- **Open Source Contributors**: For their valuable contributions
- **Beta Testers**: For their feedback and suggestions

### **Reciters Featured**
- Abdul Basit Abdul Samad
- Abdurrahmaan As-Sudais
- Maher Al Muaiqly
- Alafasy
- Abu Bakr Ash-Shaatree
- And many more renowned reciters

---

## 🌟 Why Choose Quran Hafiz?

### **For Students**
- **Structured Learning**: Organized by Surah and Juz for systematic memorization
- **Progress Tracking**: Monitor your memorization journey
- **Flexible Testing**: Multiple modes to suit your learning style

### **For Teachers**
- **Classroom Ready**: Perfect for Quran memorization classes
- **Progress Monitoring**: Track student progress and improvement
- **Customizable**: Adapt to different teaching methods

### **For Everyone**
- **Free & Open Source**: No hidden costs or subscriptions
- **Privacy Focused**: Your data stays on your device
- **Community Driven**: Built by and for the Muslim community
- **Continuously Updated**: Regular updates with new features

---

<div align="center">
  <h3>🌟 Start Your Quran Memorization Journey Today! 🌟</h3>
  
  [![Download Android](https://img.shields.io/badge/Download-Android-green.svg?style=for-the-badge&logo=android)](https://github.com/bynalab/hafiz_test/releases)
  [![Download iOS](https://img.shields.io/badge/Download-iOS-blue.svg?style=for-the-badge&logo=apple)](https://apps.apple.com/app/quran-hafiz)
  [![GitHub](https://img.shields.io/badge/GitHub-View%20Source-black.svg?style=for-the-badge&logo=github)](https://github.com/bynalab/hafiz_test)
</div>

---

<div align="center">
  <p><strong>May Allah bless this effort and make it beneficial for all Muslims seeking to memorize His words. Ameen.</strong> 🤲</p>
  
  <p><em>Built with ❤️ by the Muslim developer community</em></p>
</div>
