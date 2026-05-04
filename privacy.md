---
title: Privacy Policy
permalink: /privacy
---

# Privacy Policy

**Last updated: May 4, 2026**

168 ("the app") is a personal time-budget tool for iOS. This policy explains what data the app accesses, how it is stored, and what is shared with third parties.

The short version: **everything you log lives on your device, and a copy is synced to our servers so you can sign in across devices. We don't sell your data, we don't run ads, and we don't share your time entries with anyone.**

---

## 1. Data we access on your device

### Time entries you log
Manual entries you create — category, duration, optional note — are stored locally on your device.

### Apple Calendar
If you connect Apple Calendar, the app reads event start time, end time, and title to auto-classify events into your time budget. All-day and canceled events are skipped. Reading happens on-device; calendar events are not transmitted to our servers.

### Google Calendar
If you connect Google Calendar, the app reads event start time, end time, and title from your primary calendar. Authentication uses Google's OAuth 2.0 flow; the access token is stored on your device. Calendar events are read on-device and are not transmitted to our servers.

### Notifications
If you enable notifications, the app schedules **local** notifications on your device. The Apple Push Notification token is stored alongside your account so we can deliver cross-device reminders.

---

## 2. Cloud sync

168 requires you to sign in (see Section 3). Once signed in, the following are synced to our servers and tied to your account so the app works across your devices:

- Time entries (category, duration, timestamp, optional note)
- Categories and budgets you've created
- Goals and streaks
- Connection metadata (which sources are connected, last sync time — **not** the source data itself; calendar events are re-derived locally on each device)
- Apple Push Notification token (for cross-device reminders)

Data in transit is encrypted via TLS. Data at rest is encrypted on the server.

You can delete all of this at any time — see Section 11.

---

## 3. Account

168 uses **Sign in with Apple** or **Sign in with Google**. We do not store passwords. Authentication is handled via OAuth identity tokens; we receive only:

- **Email address** — for sign-in and account recovery (Apple users may share a private relay email; we accept that as-is)
- **Display name** — only if you choose to share it during Apple sign-in (Apple sends this on first sign-in only)
- **Sign-in metadata** — last sign-in timestamp (for account-recovery support)

You can delete your account at any time in Settings → Account → Delete account. Deletion is permanent and removes all your synced data within 30 days.

---

## 4. Subscriptions

168 v1.0 does not offer any in-app purchases or subscriptions. A future "168 Pro" tier is on a waitlist; if you opt in, we store only your email address and the date you joined, and we will email you when Pro launches.

---

## 5. Diagnostics and crash reports

To keep the app stable, we collect crash reports via **Sentry**:

- Stack traces (no personal data)
- Device model and OS version
- App version
- Approximate event timestamp

Crash reports do **not** include your time entries, calendar events, email, or any other personal information. Sentry's privacy policy: <https://sentry.io/privacy/>.

---

## 6. Data we do NOT collect

- We do not collect device advertising identifiers (IDFA).
- We do not collect location data.
- We do not collect HealthKit data (Apple Health is not integrated in this version).
- We do not run analytics or behavioral tracking.
- We do not share your time entries, calendar events, or any personal content with advertisers or data brokers.

---

## 7. Third-party services

The app integrates with the following services. Each is invoked only when you take an action that requires it.

| Service | When invoked | What is shared |
| --- | --- | --- |
| **Sign in with Apple** | You sign in with Apple | Apple ID identity token (verified by our backend) |
| **Sign in with Google** | You sign in with Google | Google OAuth identity token (verified by our backend) |
| **Apple Calendar (EventKit)** | You connect Apple Calendar | Read-only, on-device only |
| **Google Calendar API** | You connect Google Calendar | OAuth read-only access to your primary calendar; events stay on-device |
| **Apple Push Notification service (APNs)** | You enable cross-device reminders | Device push token |
| **Supabase (backend + auth)** | You sign in or sync data | Account credentials and the sync data described in Section 2 |
| **Sentry** | Always | Anonymous crash data described in Section 5 |

We choose providers that contractually agree not to use your data for advertising or to sell it.

---

## 8. Where data is stored

- **On your device**: time entries, calendar events, all settings.
- **Our backend (Supabase)**: the data described in Section 2, plus account credentials. Hosted in the United States.
- **Apple servers**: identity tokens, push tokens.
- **Sentry**: crash reports, retained no longer than 90 days.

Data may transit through other regions during sync.

---

## 9. Your rights

Regardless of where you live, you can:

- **Delete your account and data** — Settings → Account → Delete account. Permanent, completed within 30 days.
- **Disconnect any source** — Settings → Imports → tap a source → Disconnect. You can also remove imported entries on disconnect.
- **Revoke OS-level permissions** — iOS Settings → Privacy & Security → Calendars / Notifications.

### If you live in the EU/EEA/UK (GDPR)
You have the right to access, correct, port, or erase your personal data, and to lodge a complaint with your local data protection authority. Email **mockpyomotiv@gmail.com** to make a request.

### If you live in California (CCPA)
You have the right to know what personal information we collect, request deletion, and opt out of "sale" of personal information (we do not sell personal information). Email **mockpyomotiv@gmail.com** to make a request.

---

## 10. Children

The app is not directed at children under 13 (under 16 in the EU). We do not knowingly collect data from children. If you believe a child has provided us data, contact us and we will delete it.

---

## 11. Changes to this policy

If we materially change how data is handled, we will update this page and update the "Last updated" date above. For significant changes (e.g., a new category of data being collected), we will also notify you in the app the next time you open it. Continued use after a change means you accept the new policy.

---

## 12. Contact

Questions, requests, or concerns? Email **mockpyomotiv@gmail.com**.
