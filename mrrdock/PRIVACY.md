# Privacy Policy — MRRDock

**Last updated: September 30, 2026**

## Overview

MRRDock ("the App") is a free, open-source MRR tracker for the macOS menu bar, developed by Simone Ruggiero. It is distributed from GitHub and Homebrew. This Privacy Policy explains how your information is handled when you use the App.

## Data Collection

**MRRDock does not collect, store, or share any personal data.** There is no account, no sign-in and no MRRDock server. We receive nothing from the App: nobody, including the developer, can see your revenue.

- **API keys** are stored in the **macOS Keychain** (service `com.simone.mrrdock`), never in the App's data file or in logs.
- **Settings and MRR history** are stored on your Mac in `~/Library/Application Support/MRRDock/`.

## Payment Platforms

The App calls the payment platforms you configure (Stripe, RevenueCat, Paddle, Lemon Squeezy, Polar, Dodo Payments, Gumroad) **directly from your Mac**, with the API keys you enter. Every key is used **read-only**: the App issues GET requests and nothing else. Each platform processes those requests under its own privacy policy.

## Exchange Rates

To convert revenue into your chosen currency, the App fetches exchange rates from **Yahoo Finance** (`query1.finance.yahoo.com`). Each request contains only the two currency codes and, as with any web request, your IP address: no amount and no identifier is sent. See the [Yahoo Privacy Policy](https://legal.yahoo.com/us/en/yahoo/privacy/index.html).

## Updates

The App checks for updates by downloading its public update feed from GitHub (`raw.githubusercontent.com`). GitHub sees the request like any other download; the App adds no identifier.

## Optional Discord / Slack Alerts

You can optionally enter a Discord or Slack webhook URL to receive revenue alerts in a channel of your choice. If you do, the App posts the alert text directly from your Mac to that URL, and only there (only `discord.com` and `hooks.slack.com` addresses are accepted). The webhook URL is stored on your Mac only; the feature is off unless you turn it on.

## What the App Does NOT Do

- No analytics, crash-reporting or usage-tracking SDKs
- No account and no cloud sync to our servers
- No write access to your payment platforms
- No in-app purchases or subscriptions
- No selling or sharing of data with third parties

## Deleting Your Data

Quit the App, delete it from `/Applications`, remove `~/Library/Application Support/MRRDock/` and delete the `com.simone.mrrdock` items in Keychain Access.

## Children's Privacy

The App does not knowingly collect data from children under 13.

## Changes

We may update this Privacy Policy from time to time. Changes will be reflected in the "Last updated" date above.

## Contact

**simone.ruggiero97@gmail.com**

Data controller: Simone Ruggiero, Naples, Italy.
