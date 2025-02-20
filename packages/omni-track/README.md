# Omni Track

**Omni Track** is a flexible and scalable logging solution for Flutter and Dart applications. It serves as a central hub for collecting, processing, and dispatching logs to various services, allowing seamless integration with multiple logging providers.

## 📌 Features
- ✅ **Modular Log Drivers**: Easily extend functionality with plugins like `omni_track_crashlytics`, `omni_track_sentry`, and more.
- 🔧 **Customizable Log Handling**: Define your own logging strategy or use predefined drivers.
- 🚀 **Scalable Architecture**: Works in any Flutter/Dart project, from small apps to large-scale applications.
- 📡 **Multi-Destination Logging**: Send logs to different services simultaneously.

## 📦 Installation

Add **Omni Track** to your `pubspec.yaml`:

```yaml
dependencies:
  omni_track: latest_version
```

Then, run:

```sh
flutter pub get
```

## 🚀 Getting Started

### 1️⃣ Initialize Omni Track

```dart
import 'package:omni_track/omni_track.dart';

void main() {
  OmniTrack.init();
}
```

### 2️⃣ Logging Messages

```dart
OmniTrack.log('This is an info log');
OmniTrack.log('This is an error log', level: LogLevel.error);
```

### 3️⃣ Using Log Drivers

```dart
import 'package:omni_track_crashlytics/omni_track_crashlytics.dart';

void main() {
  OmniTrack.addDriver(CrashlyticsDriver());
}
```

## 📌 Available Plugins
- [Omni Track Crashlytics](https://github.com/your-repo/omni_track_crashlytics)
- [Omni Track Sentry](https://github.com/your-repo/omni_track_sentry)

## 🤝 Contributing
Contributions are welcome! Feel free to submit issues and pull requests to improve **Omni Track**.

## 📜 License
This project is licensed under the [MIT License](LICENSE).

---

💙 Developed by [Rodrigo Rahman](https://github.com/rodrigorahman) - **Academia do Flutter** 🚀

