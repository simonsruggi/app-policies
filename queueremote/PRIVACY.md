# Privacy Policy — QueueRemote

**Last updated: September 4, 2026**

## Overview

QueueRemote ("the App") is developed by Simone Ruggiero. The App is a remote control for a queue assistant that runs on **your own Mac**: it lets you watch its status from your iPhone and receive the queue session it produces.

## Data Collection

**We do not collect analytics, profiles or personal data.** There is no sign-up: the App has no name, email or account of yours. It works only after you pair it with your own Mac.

Everything the App keeps — the pairing token, the encryption key and your preferences — is stored **on your device**, with the token and key held in the iOS **Keychain**.

## The Relay

Your Mac and your iPhone exchange data through a small relay service we operate on Cloudflare Workers (`queue-relay.simone-ruggiero97.workers.dev`).

- **End-to-end encryption**: the queue session payload (the browser cookies of the session and its URL) is encrypted on your Mac with AES-GCM, using a key derived from an X25519 key exchange performed during pairing. **Neither we nor Cloudflare can read it** — the key never leaves your two devices.
- **What the relay does see**: the pairing bearer token, the session identifiers, the event name and page URL used to label a session in the list, timestamps, the status of the assistant, and — as with any web request — the IP addresses of the devices connecting. These are used only to route data between your Mac and your iPhone.
- Data is kept only as long as needed to deliver a pending session; unpairing from the App deletes the token and key from your device.

Cloudflare acts as our hosting provider; see the [Cloudflare Privacy Policy](https://www.cloudflare.com/privacypolicy/).

## Notifications

The App shows **local notifications** on your device (for example when a session becomes available or the assistant's status changes), generated from data it has already fetched from the relay.

## What the App Does NOT Do

- No analytics, crash-reporting or usage-tracking SDKs
- No advertising identifiers (no IDFA) and no cross-app tracking
- No access to your location, photos, contacts or health data
- No in-app purchases
- No selling or sharing of data with third parties

## Children's Privacy

The App does not knowingly collect data from children under 13.

## Changes

We may update this Privacy Policy from time to time. Changes will be reflected in the "Last updated" date above.

## Contact

**simone.ruggiero97@gmail.com**
