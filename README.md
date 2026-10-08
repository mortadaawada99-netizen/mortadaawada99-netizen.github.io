# Sub-Zero Owner PWA — Push Notification Version

OneSignal App ID:
56c420e3-f7ec-4010-81be-b0f5e7bc87e8

## GitHub files to upload

Upload/replace these files in the ROOT of your `mortadaawada99-netizen.github.io` repository:

- index.html
- manifest.webmanifest
- sw.js
- icon-192.png
- icon-512.png

Also create/upload this nested path exactly:

- push/onesignal/OneSignalSDKWorker.js

The final public worker URL must be:

https://mortadaawada99-netizen.github.io/push/onesignal/OneSignalSDKWorker.js

Opening that URL should show:

importScripts("https://cdn.onesignal.com/sdks/web/v16/OneSignalSDK.sw.js");

## OneSignal dashboard

Use Custom Code integration.

Site URL:
https://mortadaawada99-netizen.github.io

The code already contains:
- App ID
- serviceWorkerPath: push/onesignal/OneSignalSDKWorker.js
- service worker scope: /push/onesignal/
- autoResubscribe enabled

Do not add another automatic OneSignal prompt in the dashboard. The PWA has its own "Enable Notifications" button.

## iPhone

1. Open https://mortadaawada99-netizen.github.io in Safari.
2. Share > Add to Home Screen.
3. Open Sub-Zero Owner FROM THE HOME SCREEN.
4. Connect to Supabase if needed.
5. Tap Enable Notifications.
6. Tap Allow on the iOS notification permission dialog.
7. In OneSignal, check Audience > Users & subscriptions.

This package only registers the iPhone for OneSignal notifications.
Automatic "new sale" and "low stock" sending is the next server-side step.
