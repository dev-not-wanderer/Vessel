# Vessel
Vessel is a quiet, local-first space for personal reflection and emotional record-keeping. Unlike modern apps that prioritize cloud syncing and social engagement, Vessel is designed to be a private sanctuary. It runs entirely on-device; your data never leaves your hardware.

Features
Offline-First Privacy: No accounts, no cloud, and no tracking. Data is stored locally via IndexedDB and never sent to a server.

Three Modes of Expression:

Diary: Freeform notes (lined or blank) for limitless writing.

Things I Love / Things I Hate: Structured lists for capturing emotional snapshots.

The Graveyard: A safety net for deleted entries, allowing for recovery of thoughts you weren't quite ready to lose.

Robust Autosave: Triple-redundant saving (25-second intervals, app backgrounding, and hardware back-button triggers).

Security: Private notes can be locked behind a secondary vault password, hashed on-device using SHA-256.

Poetic Awareness: A thoughtful notification system including daily prompts, inactivity nudges, and random gentle check-ins.

Technical Architecture
Vessel is built with a "no-framework" philosophy to ensure longevity and simplicity.

Core: Vanilla HTML5, CSS3, and ES6+ JavaScript.

Storage: Persistent local storage via IndexedDB.

Security: WebCrypto API for on-device hashing.

Mobile Wrapper: Capacitor for native Android deployment.

Notifications: Capacitor LocalNotifications plugin.

The entire application is contained within a single HTML file, making it exceptionally portable and easy to audit.

Getting Started
Development
The core experience can be run by opening the index.html file in any modern web browser.

Android Deployment
Install dependencies: npm install @capacitor/core @capacitor/cli @capacitor/local-notifications

Initialize Capacitor: npx cap init

Add Android platform: npx cap add android

Sync and open: npx cap sync && npx cap open android

License
This project is licensed under the MIT License.
