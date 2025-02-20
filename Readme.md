# Omni Track Monorepo

Welcome to the **Omni Track Monorepo**, the centralized repository for the **Omni Track** logging ecosystem. This repository contains the core package, drivers, and integrations designed to provide a flexible and scalable logging solution for Flutter and Dart applications.

## 📂 Repository Structure

```
/packages/omni_track            # Main package for logging
/packages/omni_track_core       # Core package with interfaces and abstractions
/packages/omni_track_crashlytics # Firebase Crashlytics log driver
/packages/omni_track_sentry     # Sentry log driver
/packages                      # Additional future integrations
```

## 📦 Installation
Each package in this monorepo can be installed individually. Refer to the specific package directory for installation instructions.

Example for **Omni Track**:

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

### 2️⃣ Add a Log Driver (e.g., Crashlytics)

```dart
import 'package:omni_track_crashlytics/omni_track_crashlytics.dart';

void main() {
  OmniTrack.addDriver(CrashlyticsDriver());
}
```

## 🤝 Contributing
Contributions are welcome! Feel free to submit issues, feature requests, or pull requests to improve **Omni Track**.

## 📜 License
Licensed under the [MIT License](LICENSE).

---

💙 Developed by [Rodrigo Rahman](https://github.com/rodrigorahman) - **Academia do Flutter** 🚀
