# Omni Track Core


**Omni Track Core** is the foundation of **Omni Track**, providing the necessary interfaces and abstractions to create custom logging solutions. This package allows developers to build custom log drivers or use existing ones like `omni_track_crashlytics` and `omni_track_sentry`.

## 📌 Features
- ✅ **Core Logging Abstractions**: Provides interfaces for building custom log drivers.
- 🔌 **Plugin-Based Architecture**: Easily extend with specific log integrations.
- 🚀 **Lightweight and Flexible**: Designed to fit any logging requirement.
- 📡 **Seamless Integration**: Works with multiple logging backends.

## 📦 Installation

Add **Omni Track Core** to your `pubspec.yaml`:

```yaml
dependencies:
  omni_track_core: latest_version
```

Then, run:

```sh
flutter pub get
```

## 🚀 Getting Started

### 1️⃣ Implement a Custom Log Driver

```dart
import 'package:omni_track_core/omni_track_core.dart';

class MyCustomDriver extends LogDriver {
  @override
  void log(LogEntry entry) {
    print('[${entry.level}] ${entry.message}');
  }
}
```

### 2️⃣ Register the Custom Driver

```dart
void main() {
  OmniTrackCore.addDriver(MyCustomDriver());
}
```

## 📌 Available Plugins
- [Omni Track Crashlytics](https://github.com/your-repo/omni_track_crashlytics)
- [Omni Track Sentry](https://github.com/your-repo/omni_track_sentry)

## 🤝 Contributing
Contributions are welcome! Feel free to submit issues and pull requests to improve **Omni Track Core**.

## 📜 License
This project is licensed under the [MIT License](LICENSE).

---

💙 Developed by [Rodrigo Rahman](https://github.com/rodrigorahman) - **Academia do Flutter** 🚀

