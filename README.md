# winecalcpro-privacy
Privacy Policy for WineCalc Pro  Effective date: May 7, 2026  WineCalc Pro is developed by Manuchar Meskhidze.
Privacy Policy for WineCalc Pro
Last updated: September 27, 2026
Applies to WineCalc Pro for Android, package com.manuchar.winecalcpro.

WineCalc Pro is developed by Manuchar Meskhidze. This policy explains how the Android app handles information when you use its calculators, cellar records, label scanner, optional online recognition, and optional AI features. For privacy questions, contact monkeyskm@gmail.com.

1. Information stored on your device
The app processes ordinary wine calculations on your device. It stores your saved calculation history, favorites, cellar tasks, wine batch records, logbook entries, saved scan text, and preferences in the app’s private Android storage. Records may contain names, notes, measurements, dates, and other information you choose to enter. The app does not require a WineCalc user account or provide an automatic WineCalc account synchronization service.

Your records are not automatically sent to the developer as part of ordinary calculator and logbook use. Online recognition, AI requests, sharing, Android backups, and SDK diagnostics are described separately below.

2. Camera and label scanning
The scanner requests Android camera permission and uses the camera while you use the scanning feature. You can decline or revoke camera permission in Android settings; the other calculators do not require it.

Offline mode: label text is recognized on your device using Tesseract. The fallback ML Kit text recognizer also processes images and recognized text on the device.
Online mode: when you supply a Google Cloud Vision API key and start a scan, the captured image is sent to Google Cloud Vision over HTTPS to recognize its text. Images can include any personal information visible in the photograph.
Auto mode: the scanner attempts online recognition first when a usable API key is supplied and falls back to on-device recognition if the online attempt fails. Without a key, it falls back to local processing.
Captured images are temporarily written to the app’s private cache. The app attempts to delete each temporary image when recognition finishes, including when recognition returns an error. An interrupted operation can leave a cache file until the cache is cleared. Recognized text becomes a persistent logbook entry only when you choose to save it.

For the synchronous Cloud Vision recognition used by this app, Google states that images are processed in memory rather than persisted to disk, while some request metadata is logged temporarily. See Google Cloud Vision data usage.

3. Optional AI requests
The AI Wine Expert feature requires you to enter an endpoint address. When you press Generate Tasks, the app sends your entered cellar situation, selected language, and task instructions to that endpoint. If you enter a bearer token, it is sent to the same endpoint to authenticate the request. There is no preconfigured AI endpoint in this Android version.

The companion backend supplied with WineCalc Pro forwards the submitted text to the OpenAI API to generate a response. A different endpoint may use a different provider. Use only an endpoint you trust, use HTTPS, and review its operator’s privacy information before submitting personal or confidential information. The endpoint operator and its AI and hosting providers may process request content and connection metadata, such as your IP address.

The app keeps the endpoint, token, request input, and displayed response in the current screen’s memory rather than saving them as a persistent AI conversation history. Server-side retention, logs, and deletion depend on the endpoint operator and provider configuration; clearing the app does not delete copies already processed by an external service. For OpenAI’s practices, see OpenAI’s privacy policy. Contact the endpoint operator for the applicable retention period and deletion options.

4. SDK diagnostics and third parties
The app includes Google ML Kit for an on-device text recognition fallback. ML Kit may send Google device and application information, installation identifiers, and API usage and performance metrics for diagnostics, maintenance, and usage analytics. Its on-device image and text inputs and recognition results are not sent to Google as part of ML Kit recognition. Google documents HTTPS encryption for these diagnostic transmissions. See ML Kit privacy information, ML Kit’s Android data disclosures, and Google’s privacy policy.

The app does not include advertising functionality or sell user data. External providers process information as described in this policy and their applicable terms. Optional online services may process information outside your country.

5. Sharing and backups
If you use Share on a logbook entry, the selected text is passed to the app or recipient you choose in Android’s share menu. The recipient’s handling of that copy is outside WineCalc Pro’s control.

Android backup is enabled for the app. Depending on your device and backup settings, Android may include eligible app data in a cloud backup or device transfer. Backup storage, protection, retention, and removal are controlled by Android and your backup provider. Restoring a backup can restore previously saved records. Manage backups through your device and provider settings.

6. Secure data handling
Local records and temporary scan files are stored in Android’s app-specific private storage, protected by the operating system’s application sandbox. The app does not implement a separate encrypted database, so device security and any operating-system encryption remain important. Protect your device with a screen lock and current security updates.

Cloud Vision requests use HTTPS. The Android app does not opt in to cleartext network traffic; use HTTPS for optional AI endpoints. The companion backend connects to OpenAI over HTTPS and reads the provider API key from server-side environment configuration rather than embedding it in the Android app. Camera access is subject to Android permission controls. User-entered Cloud Vision keys and AI bearer tokens are not saved in the app’s preferences. No storage or transmission method provides an absolute security guarantee.

7. Retention and deletion
Saved logbook entries, tasks, batch records, and preferences remain on your device until removed or the app’s data is cleared. Calculation history retains up to the latest 50 entries and can be cleared in the app.
You can delete individual logbook entries and batch records using their in-app deletion controls. To remove all local app data, use Android Settings → Apps → WineCalc Pro → Storage → Clear storage/data, or uninstall the app. Device menus may use different labels.
Clear the app’s cache to remove any remaining temporary scan files. Copies in backups, shared messages, or external services must be managed separately with the corresponding provider or recipient.
The developer cannot remotely read or erase records that exist only in your device’s private app storage. Contact the developer for help with privacy requests concerning information held by the developer; contact your selected AI endpoint operator for requests concerning that service.
8. Changes and contact
Updates to this policy will be published on this page with a revised date. Questions about this policy or the app’s data handling can be sent to Manuchar Meskhidze at monkeyskm@gmail.com.

WineCalc Pro for Android · Manuchar Meskhidze
