---
title: Privacy Policy
permalink: /privacy
---

# Privacy Policy

**Last updated: April 27, 2026**

168 ("the app") is a personal time-budget tool for iOS. This policy explains what data the app accesses, how it is stored, and what is shared with third parties.

The short version: **everything we collect is either stored locally on your device or, if you opt in to cloud sync, on our servers tied to your account. We do not sell your data, and we do not use HealthKit data for advertising — ever.**

---

## 1. Data we access on your device

### Time entries you log
Manual entries you create — category, duration, optional note — are stored locally on your device.

### Apple Calendar
If you connect Apple Calendar, the app reads event start time, end time, title, and decline status to auto-classify events into your time budget.

### Apple Health (HealthKit)
If you connect Apple Health, the app reads workout sessions and mindful sessions (start time, end time, type) to auto-classify them. The app does not write any data to Apple Health.

### Google Calendar
If you connect Google Calendar, the app reads event start time, end time, title, and decline status from your primary calendar. Authentication uses Google's OAuth 2.0 flow; the access token is stored on your device.

### Notifications
If you enable notifications, the app schedules **local** notifications on your device. No notification token is transmitted unless you opt in to cloud sync (see Section 2).

---

## 2. Cloud sync (optional, opt-in)

If you enable cloud sync, the following are uploaded to our servers and tied to your account:

- Time entries (category, duration, timestamp, optional note)
- Categories and budgets you've created
- Goals and streaks
- Connection metadata (which sources are connected, last sync time — **not** the source data itself; calendar events and HealthKit samples are re-derived locally on each device)
- Push notification token (so we can deliver notifications across your devices)

**Cloud sync is off by default.** You can turn it off at any time in Settings → Sync; doing so removes your data from our servers within 30 days.

Data in transit is encrypted via TLS. Data at rest is encrypted on the server.

---

## 3. Account

If you create a 168 account (required for cloud sync, Pro, or signing in across devices), we collect:

- **Email address** — for sign-in and account recovery
- **Hashed password** — we never store your password in plain text; we use industry-standard hashing (bcrypt or Argon2)
- **Sign-in metadata** — last sign-in timestamp, the device type that signed in (for security alerts)

You can delete your account at any time in Settings → Account → Delete Account. Deletion is permanent and removes all your synced data within 30 days.

---

## 4. Pro subscription

168 Pro is a paid auto-renewing subscription managed entirely by Apple through the App Store.

**What Apple handles** (we never see this):
- Your payment method
- Your Apple ID
- Your billing address

**What we receive** from Apple:
- A subscription status flag (active / expired / refunded)
- A receipt that proves your purchase

We use this information only to unlock Pro features for your account. Subscription terms (price, renewal, cancellation) are governed by Apple's standard subscription terms; you can manage your subscription in iOS Settings → Apple ID → Subscriptions.

---

## 5. Diagnostics and crash reports

To keep the app stable, we collect **anonymous** crash reports and error logs:

- Stack traces (no personal data)
- Device model and OS version
- App version
- Approximate event timestamp

Crash reports do **not** include your time entries, calendar events, HealthKit data, email, or any other personal information.

You can turn diagnostics off in Settings → Privacy → Send Crash Reports. They are on by default but easy to disable.

---

## 6. Analytics

We collect **anonymous** usage statistics to understand which features matter:

- Which screens are opened
- Which features are used (e.g., "started timer", "logged entry")
- Aggregate counts (e.g., "average entries per week")

We do **not** collect:
- The contents of your entries (titles, notes, categories)
- HealthKit data of any kind
- Calendar event titles or attendees
- Your email address or any identifier that links events to you personally

You can turn analytics off in Settings → Privacy → Share Anonymous Usage Data. They are on by default but easy to disable.

---

## 7. Data we do NOT collect

- We do not collect device advertising identifiers (IDFA).
- We do not collect location data.
- We do not sell, share, or use HealthKit data for advertising, marketing, data mining, or any purpose other than display within the app.
- We do not share your time entries, calendar events, or any personal content with advertisers or data brokers.

---

## 8. Third-party services

The app integrates with the following services. Each is invoked only when you take an action that requires it.

| Service | When invoked | What is shared |
| --- | --- | --- |
| **Apple HealthKit** | You connect Apple Health | Read-only, on-device only |
| **Apple Calendar (EventKit)** | You connect Apple Calendar | Read-only, on-device only |
| **Apple App Store / StoreKit** | You purchase Pro | Apple handles payment; we receive a subscription receipt |
| **Apple Push Notification service (APNs)** | You enable cross-device notifications via cloud sync | Device push token |
| **Google Calendar API** | You connect Google Calendar | OAuth read-only access to your primary calendar |
| **Our backend (cloud sync)** | You enable cloud sync or create an account | Sync data described in Section 2 |
| **Crash reporting provider** | Always, unless you opt out | Anonymous crash data described in Section 5 |
| **Analytics provider** | Always, unless you opt out | Anonymous events described in Section 6 |

We choose providers that contractually agree not to use your data for advertising or to sell it.

---

## 9. HealthKit-specific terms

In compliance with Apple's HealthKit guidelines:

- HealthKit data is read on-device only.
- HealthKit data is **never** transmitted to our servers, even if you enable cloud sync.
- HealthKit data is **never** shared with third parties.
- HealthKit data is **never** used for advertising, marketing, or data mining.
- You can revoke HealthKit access at any time via iOS Settings → Privacy & Security → Health.

---

## 10. Where data is stored

- **On your device**: time entries, calendar events, HealthKit samples (always), all settings.
- **Our servers** (only if cloud sync is enabled): the data described in Section 2, plus account credentials.
- **Apple servers**: subscription receipts, push tokens.
- **Crash / analytics provider**: anonymous events, retained no longer than 90 days.

Our servers are hosted in the United States. Data may transit through other regions during sync.

---

## 11. Your rights

Regardless of where you live, you can:

- **Export your data** — Settings → Account → Export. We deliver a JSON file containing all your synced data.
- **Delete your account and data** — Settings → Account → Delete Account. Permanent, completed within 30 days.
- **Disconnect any source** — Settings → Imports → tap a source → Disconnect. You can also remove imported entries on disconnect.
- **Opt out of diagnostics or analytics** — Settings → Privacy.
- **Revoke OS-level permissions** — iOS Settings → Privacy & Security → Health / Calendars / Notifications.

### If you live in the EU/EEA/UK (GDPR)
You have the right to access, correct, port, or erase your personal data, and to lodge a complaint with your local data protection authority. Email **mockpyomotiv@gmail.com** to make a request.

### If you live in California (CCPA)
You have the right to know what personal information we collect, request deletion, and opt out of "sale" of personal information (we do not sell personal information). Email **mockpyomotiv@gmail.com** to make a request.

---

## 12. Children

The app is not directed at children under 13 (under 16 in the EU). We do not knowingly collect data from children. If you believe a child has provided us data, contact us and we will delete it.

---

## 13. Changes to this policy

If we materially change how data is handled, we will update this page and update the "Last updated" date above. For significant changes (e.g., a new category of data being collected), we will also notify you in the app the next time you open it. Continued use after a change means you accept the new policy.

---

## 14. Contact

Questions, requests, or concerns? Email **mockpyomotiv@gmail.com**.
