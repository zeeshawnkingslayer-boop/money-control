# Money Control — APK conversion package

This folder contains the complete mobile-first web app prepared for Android packaging.

Files:
- index.html — application
- manifest.webmanifest — install/app metadata
- sw.js — offline cache/service worker
- icon-192.png — app icon
- icon-512.png — app icon

Android-only conversion:
1. Put these files on a web host (for example, any static hosting service).
2. Open the hosted app in Chrome on Android.
3. Chrome can install it as a PWA if the host serves HTTPS.
4. If you specifically need an APK, use an Android packaging service/tool that accepts a hosted PWA URL (such as a Trusted Web Activity wrapper).

Important:
- The app stores budget/expense data in the browser's localStorage.
- Export a backup before clearing browser data or uninstalling a wrapper.
