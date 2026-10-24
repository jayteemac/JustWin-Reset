JUST WIN v2.2 — OneSignal push connection (test phase)

IMPORTANT BEFORE UPLOADING:
1. Export a private JSON backup from JUST WIN. Never upload the JSON to public GitHub.
2. In OneSignal > Web Configuration > Advanced > Service workers set:
   Service worker path: /JustWin-Reset/
   Main filename: OneSignalSDKWorker.js
   Updater filename: OneSignalSDKUpdaterWorker.js
   Service worker registration scope: /JustWin-Reset/onesignal/
   (The narrower scope prevents collision with JUST WIN's offline sw.js.)
3. Upload ALL files in this ZIP to the ROOT of the jayteemac/JustWin-Reset repository.
4. After GitHub Pages deployment, open JUST WIN on your Galaxy, go to Settings > Enable notifications and grant permission.
5. In OneSignal dashboard, send a manual test push to your subscribed device. Set click URL to:
   https://jayteemac.github.io/JustWin-Reset/#emotion
   Or #today / #mental.

IMPORTANT: Recurring 3-times-daily reminders are NOT scheduled by this update. This is the connection/test phase only. We must verify push delivery and then configure a free recurring sender.

Your existing localStorage key reset90-v1 is unchanged.
