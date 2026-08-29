# Privacy Policy for Sucar!

_Last updated: 2026-08-21_

Sucar! ("the app") is a glucose monitoring app that displays Continuous Glucose Monitor (CGM) data from a service you already use, in the car (via Android Auto or, for the experimental Android Automotive OS variant, directly on the vehicle's built-in screen).

## Summary

Sucar! has no backend server of its own. It reads glucose data either from the cloud CGM service you configure (LibreView/LibreLinkUp, Dexcom Share, or Nightscout) or directly from another app already on your phone (xDrip+ or Juggluco, via their local, on-device broadcast APIs). Data goes from that source straight to your device — never through a server operated by us. The app contains no analytics, advertising, or crash-reporting SDKs, and does not sell or share your data with any third party.

## What data the app accesses

- **Glucose readings and trend**, from whichever single data source you select in Settings:
  - **LibreView/LibreLinkUp, Dexcom Share, or Nightscout**: the app connects directly to that service's own servers, using the account
    credentials or server address you provide, to fetch your glucose data.
  - **xDrip+ or Juggluco**: if you use one of these apps on the same phone, Sucar! receives glucose updates via that app's local broadcast API — this data never leaves your device.
  - **Demo mode**: generates fake data locally for trying out the app; no real data or network access involved.
- **Account credentials** (for LibreView, Dexcom, or a Nightscout URL/token, if you use one of those sources) are stored locally on your device, in the app's private settings storage, and are sent only directly to the corresponding official service you configured — never to any server operated by Sucar!.

## Where data is stored

- The app keeps a short local history of your recent glucose readings (up to about 12 hours) on your device, purely to draw the graph. This history is not uploaded anywhere by the app.
- Your settings (selected data source, credentials/URL, unit preference, display preferences) are stored locally on your device using Android's standard app-private storage (DataStore).
- Like most Android apps, Sucar! allows Android's built-in device backup (tied to your own Google account) to include this locally stored data, so it can be restored if you set up a new device signed into the same Google account. This is controlled by your device's own backup settings, not by Sucar!.

## Data sharing

Sucar! does not sell, rent, or share your glucose data or credentials with any third party. The only network destinations the app talks to are the CGM service you explicitly configured (LibreView, Dexcom, or your own Nightscout server) — no analytics platform, advertising network, or crash-reporting service is included in the app.

## Android Auto / Android Automotive

When connected to Android Auto, or when running the Android Automotive OS variant, the app displays the same glucose data described above on the vehicle's screen and, on the mobile variant, in an ongoing notification while a car session is active. No additional data is collected for this purpose, and nothing is transmitted to the vehicle manufacturer or to Google beyond what Android Auto's platform itself requires to operate.

## Permissions

The app requests only the Android permissions needed for its core functionality: network access to reach your chosen CGM service, notification and foreground-service permissions to keep glucose polling running while connected to Android Auto, exact-alarm scheduling to keep glucose data timely, and boot-completed access to resume monitoring after a device restart if a car session was recently active. No location, contacts, camera, microphone, or similar sensitive permissions are requested.

## Your choices

You can change or remove your configured data source and credentials at any time from the app's Settings. Uninstalling the app removes its locally stored data from your device (subject to any device backup you may have enabled, as described above).

## Contact

If you have questions about this privacy policy, contact: sucar@gmx.eu
