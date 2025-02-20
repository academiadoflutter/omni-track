# Omni Track Crashlytics

**Omni Track Crashlytics** is a log driver for **Omni Track**, providing seamless integration with **Firebase Crashlytics** for real-time error tracking and diagnostics.

## 📦 Installation

Add to your `pubspec.yaml`:

```yaml
dependencies:
  omni_track_crashlytics: latest_version
```

Then, run:

```sh
flutter pub get
```

## 🚀 Usage

### 1️⃣ Initialize Omni Track with Crashlytics

```dart
import 'package:omni_track/omni_track.dart';
import 'package:omni_track_crashlytics/omni_track_crashlytics.dart';

void main() {
  OmniTrack.addDriver(CrashlyticsDriver());
}
```

### 2️⃣ Logging Errors

```dart
try {
  throw Exception('Test error');
} catch (e, stacktrace) {
  OmniTrack.logError(e, stacktrace);
}
```

## 🤝 Contributing
Contributions are welcome! Feel free to submit issues and pull requests.

## 📜 License
Licensed under the [MIT License](LICENSE).

---

💙 Developed by [Rodrigo Rahman](https://github.com/rodrigorahman) - **Academia do Flutter** 🚀

