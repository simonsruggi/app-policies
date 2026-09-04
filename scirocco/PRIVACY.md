# Privacy Policy — Scirocco

**Last updated: September 4, 2026**

## Overview

Scirocco ("the App") is developed by Simone Ruggiero and is available for iOS and Android. This Privacy Policy explains what the App does with your data.

## Data Collection

**We do not collect, receive or store any personal data on our own servers.** The App has no account and no backend of ours.

Everything you create in the App — waypoints, routes, tracks, vessels, documents, insurance records, notes, attached photos and settings — is stored **on your device** (SwiftData on iOS, SQLite on Android).

## Location

The App uses your device location (GPS) to show your position on the chart, calculate distances and bearings to waypoints, and record GPS tracks.

- On iOS, background location ("Always") is requested **only** so that track recording keeps working while the App is not in the foreground.
- On Android, the App uses a foreground location service for the same purpose.

Your position is processed on the device, is stored only in your local tracks, and is **never** sent to us or used for advertising. You can use most of the App without granting location access.

## Charts and Maps

- **iOS**: charts are rendered with **Apple MapKit**. As with any map, Apple receives the map area you are viewing in order to serve it. See the [Apple Privacy Policy](https://www.apple.com/legal/privacy/).
- **Android**: chart tiles are downloaded from **OpenStreetMap** and **OpenSeaMap**. As with any web request, those providers receive the map area you are viewing and your IP address. They are not given your identity.

Map data is requested only to draw the chart. Tiles already cached on the device keep working offline.

## iCloud Sync (iOS)

If you enable iCloud sync in Settings, the App synchronises your Scirocco data through **your own private iCloud database** (CloudKit) so it is available on your other Apple devices. The sync happens between your device and your iCloud account: **we have no access** to that data and cannot read it. If sync is off, or no iCloud account is configured, everything stays local.

## Photos, Documents and Text Recognition

- You can attach photos and documents (for example vessel papers or insurance certificates) to your records. They are picked with the system picker and stored inside the App on your device. On Android, camera and media access are requested only when you choose to take or pick a photo.
- The App can read coordinates from an image or a shared screenshot using text recognition (OCR). Recognition runs **entirely on the device** — Apple's Vision framework on iOS, Google ML Kit's on-device text recognition on Android. The images are not uploaded anywhere.
- GPX files you import or export stay on your device unless you deliberately share them.

## Notifications, Widgets and Live Activities

Anchor-watch and other alerts are scheduled and shown **locally on your device**. Widgets and Live Activities read data already stored on your device. We do not send push notifications from any server.

## Third-Party Services

- **RevenueCat** — manages subscriptions. It receives an anonymous, randomly generated identifier, purchase and subscription history, and the store country. No name, email or navigation data is shared. See their [Privacy Policy](https://www.revenuecat.com/privacy).
- **Apple StoreKit / Google Play Billing** — process in-app purchases; all payment data is handled directly by Apple or Google under their respective privacy policies.
- **Apple MapKit** (iOS) and **OpenStreetMap / OpenSeaMap** (Android) — provide the chart, as described above.
- **Refund requests**: if you request a refund for an in-app purchase on the Apple App Store, Apple may ask us — via RevenueCat — to share data about your use of the App related to that purchase ("consumption data") to help Apple decide on the refund, in line with Apple's guidelines. This data is used only to process the refund request.

## What the App Does NOT Do

- No analytics, crash-reporting or usage-tracking SDKs
- No advertising identifiers (no IDFA, no Android Advertising ID) and no cross-app tracking
- No selling or sharing of your data with third parties

## Safety Notice

Scirocco is a navigation aid, not a certified nautical chart system. It does not replace official charts and instruments required on board.

## Children's Privacy

The App does not knowingly collect data from children under 13.

## Changes

We may update this Privacy Policy from time to time. Changes will be reflected in the "Last updated" date above.

## Contact

**simone.ruggiero97@gmail.com**
