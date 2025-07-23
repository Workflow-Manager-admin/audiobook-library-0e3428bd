# mobile_frontend_app

A Flutter mobile app for browsing, buying, and playing audiobooks with library and playback tracking, built using modern, clean UI and local storage. 

## Features
- Store tab: Browse a marketplace of audiobooks with details and buy actions.
- Library tab: View and select your purchased audiobooks.
- Player tab: Cover art, title/author, playback controls (play/pause, skip 15s), progress bar, and playback position display.
- Audiobook library and playback progress are stored *locally* (offline-ready).
- Modern, light, user-friendly UI. Accent color `#50B99A`, Primary `#3C4F76`, Secondary `#F7C873`.

## How It Works

- Purchases and library are stored offline in local SQLite (sqflite).
- Playback progress (for every book) is saved and persisted automatically.
- All navigation via bottom tabs.

## How to Run

1. Ensure you have Flutter SDK installed.
2. From the `mobile_frontend_app` directory, run:
   ```
   flutter pub get
   flutter run
   ```
3. No API backend required – demo catalog and local-only functionality.

## Dependencies

- [sqflite](https://pub.dev/packages/sqflite)
- [provider](https://pub.dev/packages/provider)
- [shared_preferences](https://pub.dev/packages/shared_preferences)
- [intl](https://pub.dev/packages/intl)

## Customization

- To customize the catalog, see the `demoStoreBooks` list in `lib/main.dart`.
- For your own backend, replace the store/book logic accordingly.

---
