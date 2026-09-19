# YouTube Queue Pro 2.0

A personal Android companion for the official YouTube app.

### Features
- Android Share Sheet: YouTube -> Share -> YouTube Queue Pro
- Paste links
- Persistent queue
- Duplicate prevention
- Reorder with up/down controls
- Open any queued item
- Delete/clear queue
- Accessibility service with conservative end-state detection
- Attempts to open the next queued item directly in the YouTube app

### Important limitation
The official YouTube Android app does not expose a public third-party API for another app to read its playback position or command its player. The automatic feature therefore uses Android Accessibility to observe visible UI text. It is deliberately conservative and can vary with YouTube UI changes.

### Build
Open the project in Android Studio, let Gradle sync, then Build > Build APK(s). Install the debug APK on an Android phone. In Android Settings > Accessibility > Installed apps, enable YouTube Queue Pro.

### Privacy
The queue is stored locally in SharedPreferences. No network service or account login is included.
