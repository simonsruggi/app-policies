# Privacy Policy — Scirocco

**Last updated: September 27, 2026**

## Overview

Scirocco ("the App") is developed by Simone Ruggiero and is available for iOS and Android. This Privacy Policy explains what the App does with your data.

## Data Collection

The App has **no account**, and **we do not store any personal data on our own servers**.

Everything you create in the App — waypoints, routes, tracks, vessels, documents, insurance records, personal documents, notes, attached photos and settings — is stored **on your device** (SwiftData on iOS, SQLite on Android). The name you may enter during onboarding or in "My data" is optional, stays on your device and is never synced or sent anywhere.

The only service of ours the App talks to is the **marine forecast service** described below (iOS only). It receives an approximate position, not your identity, and does not keep it.

## Location

The App uses your device location (GPS) to show your position on the chart, calculate distances and bearings to waypoints, and record GPS tracks.

- On iOS, background location ("Always") is requested **only** so that track recording keeps working while the App is not in the foreground.
- On Android, the App uses a foreground location service for the same purpose.

Your precise position is processed on the device, is stored only in your local tracks, and is **never** sent to us or used for advertising. You can use most of the App without granting location access.

## Marine Forecast (iOS)

To show the weather and sea forecast, the App sends our forecast service at `scirocco.app` an **approximate position**: the coordinates of where you are, or of the place you chose, **rounded to 0.1° (about 11 km)**. No identifier, name or account is sent with it.

- Our service forwards the rounded coordinates to **Open-Meteo**, the weather data provider, to obtain the forecast. Open-Meteo receives the request from our server, not from your device, so it does not see your IP address.
- Our service does not save coordinates in any database. It keeps only anonymous counters (for example, how many forecasts were requested), with no IP address or position.
- The service runs on **Cloudflare**, which processes your IP address to deliver the request and to limit abuse (a maximum number of requests per minute). Cloudflare's technical logs, kept for a few days, may include the request with the rounded coordinates.
- The last forecast is saved **on your device** so you can see it without a connection.

When you search for a place by name, the text you type is sent to **Apple** (MapKit search) to find matching places.

## Charts and Maps

- **iOS**: charts are rendered with **Apple MapKit**. As with any map, Apple receives the map area you are viewing in order to serve it. See the [Apple Privacy Policy](https://www.apple.com/legal/privacy/).
- **Android**: chart tiles are downloaded from **OpenStreetMap** and **OpenSeaMap**. As with any web request, those providers receive the map area you are viewing and your IP address. They are not given your identity.

Map data is requested only to draw the chart. Tiles already cached on the device keep working offline.

## iCloud Sync (iOS)

If you enable iCloud sync in Settings, the App synchronises your Scirocco data through **your own private iCloud database** (CloudKit) so it is available on your other Apple devices. The sync happens between your device and your iCloud account: **we have no access** to that data and cannot read it. If sync is off, or no iCloud account is configured, everything stays local.

## Photos, Documents and Text Recognition

- You can attach photos and documents (for example vessel papers, insurance certificates or your boating licence) to your records, or scan them with the document camera. They are picked with the system picker and stored inside the App on your device. On Android, camera and media access are requested only when you choose to take or pick a photo.
- The App can read coordinates from an image or a shared screenshot, and fill in the fields of a scanned document, using text recognition (OCR). Recognition runs **entirely on the device** — Apple's Vision framework on iOS, Google ML Kit's on-device text recognition on Android. The images are not uploaded anywhere.
- GPX files you import or export stay on your device unless you deliberately share them.

## Notifications and Live Activities

Reminders (document, insurance and maintenance deadlines) and navigation alerts are scheduled and shown **locally on your device**. On iOS, the Live Activity on the lock screen reads data already on your device. We do not send push notifications from any server.

## Diagnostics

On iOS the App receives crash and performance reports from Apple's MetricKit only if you have chosen to share analytics with developers in iOS Settings. The App keeps a technical log **on your device**; it leaves the device only if you decide to attach it to an email to support ("Contact me").

## Third-Party Services

- **RevenueCat** — manages subscriptions. It receives an anonymous, randomly generated identifier, purchase and subscription history, and the store country. The App also stores there a few **anonymous usage counters** linked to that identifier — how many times the subscription screen was shown and from which part of the App, and (iOS) how often the forecast is opened — to understand which features lead to a subscription. No name, email, position or navigation data is shared. See their [Privacy Policy](https://www.revenuecat.com/privacy). If you installed the App after tapping an Apple Ads advertisement, the App also passes RevenueCat the attribution token provided by Apple's AdServices framework: it only tells us which ad campaign led to the install, contains no personal data and does not require tracking permission.
- **Apple StoreKit / Google Play Billing** — process in-app purchases; all payment data is handled directly by Apple or Google under their respective privacy policies.
- **Apple MapKit** (iOS) and **OpenStreetMap / OpenSeaMap** (Android) — provide the chart and (iOS) the place search, as described above.
- **Open-Meteo** and **Cloudflare** (iOS) — provide and deliver the marine forecast, as described above.
- **Refund requests**: if you request a refund for an in-app purchase on the Apple App Store, Apple may ask us — via RevenueCat — to share data about your use of the App related to that purchase ("consumption data") to help Apple decide on the refund, in line with Apple's guidelines. This data is used only to process the refund request.

## What the App Does NOT Do

- No third-party analytics or crash-reporting SDKs: the only usage data are the anonymous counters sent to RevenueCat described above
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
