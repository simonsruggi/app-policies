# Privacy Policy — FarmaStock

**Last updated:** June 4, 2026

## Overview

FarmaStock ("the App") is developed by Simone Ruggiero. The App is also accompanied by a website at [https://farmastock.app](https://farmastock.app) ("the Website"). This Privacy Policy explains how your information is handled when you use the App and/or the Website.

## Data Collection

### The App
FarmaStock does **not** require a user account and does **not** collect your personal data. Your scanned products, inventory, and expiry dates are stored **locally on your device** (using SwiftData on iOS and SQLite on Android) and are never uploaded to us.

### The Website
The Website does not require user accounts or collect personal data. Anonymous analytics may be collected through [EasyAnalytics](https://easyanalytics.app) to understand usage patterns (page views, referrers). No cookies are used for tracking purposes.

## Camera Usage

The App uses your device's camera exclusively to:
- Scan product barcodes (EAN/UPC codes)
- Read expiry dates via OCR (optical character recognition)

Camera data is processed entirely on-device and is never recorded, stored, or transmitted.

## Third-Party Services

The App uses the following third-party services:

### Product Lookup Service
When you scan a barcode (or search by product name) that is not in the local database, the App sends **only the barcode number or search term** to our lookup service (hosted on Supabase) to retrieve product information (name, brand, category). To identify the product, our service may in turn query third-party sources: **UPCitemdb**, **Open Food Facts**, and an **AI web-search assistant (Anthropic)**. Your IP address is processed transiently for rate-limiting and is not stored. No personal, account, or health data is transmitted.

### RevenueCat
Used to manage premium subscriptions. RevenueCat may collect:
- Anonymous device identifier
- Purchase and subscription history
- Country/region (derived from the app store)

No personal information (name, email, health data) is shared with RevenueCat. For more details, see the [RevenueCat Privacy Policy](https://www.revenuecat.com/privacy).

### In-App Purchases
Subscriptions are processed by **Apple StoreKit** (iOS) or **Google Play Billing** (Android). All payment data is handled directly by Apple or Google and is governed by their respective privacy policies.

If you request a refund for an in-app purchase on the Apple App Store, Apple may ask us — via RevenueCat — to share data about your use of the App related to that purchase ("consumption data") to help Apple decide on the refund, in line with Apple's guidelines. This data is used only to process the refund request.

## Notifications

The App may send local notifications to remind you of upcoming product expiry dates. These notifications are generated entirely on-device and are not sent through any external server.

## Data Sharing

We do **not** share, sell, or transfer any personal or health-related user data to third parties. The only data transmitted externally is:
- **Barcode numbers / product search terms** → to our lookup service and the product databases above (UPCitemdb, Open Food Facts, Anthropic), to identify scanned products
- **Anonymous purchase data** → to RevenueCat (for subscription management)

## Children's Privacy

The App does not knowingly collect data from children under 13.

## Changes

We may update this Privacy Policy from time to time. Changes will be reflected in the "Last updated" date above.

## Contact

For questions or concerns about this Privacy Policy, contact:

**Simone Ruggiero**
Email: simone.ruggiero97@gmail.com
