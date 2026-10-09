---
sidebar_position: 2
title: Privacy Policy
---

# Privacy Policy

**App:** EveryHour — Hours Tracker (hours tracking and pay stub checking for hourly workers in the United States)  
**Platforms:** iOS (App Store) and Android (Google Play)  
**Effective date:** October 9, 2026  
**Last updated:** October 9, 2026  
**Publisher / data controller:** WBB  
**Contact:** [vincenttrandeveloper@gmail.com](mailto:vincenttrandeveloper@gmail.com)

---

## Summary — the short version

EveryHour is built so that your work records stay on your phone.

- **There is no account and no sign-up.** No email, no password, no social login.
- **Your hours, breaks, pay rates, workplaces, pay stub photos, notes, and reports stay on your phone** and are not sent to us.
- **Pay stub photos are read on your phone.** They are never uploaded.
- **No ads, no ad SDKs, no tracking across other apps or websites.** We never sell your personal information.
- **What does leave the device:** a request to a web server to check the current time, anonymous usage statistics, crash reports, purchase/entitlement events — and, only if you choose to send one, the content of a feedback report. None of these contain your hours or your pay.

The rest of this policy explains each of those points precisely.

---

## 1. Scope

This policy applies to the EveryHour app distributed on the Apple App Store and Google Play, and to any future updates, to the extent that the features described are actually enabled on your device.

It does not cover Apple's or Google's own processing of your data as the platform and store operator, or the processing done by any service you choose to send an exported file to (email, Files, iCloud Drive, Google Drive), which is governed by their own privacy policies.

## 2. Data that stays on your device

Everything you enter or create in EveryHour is stored in the app's private storage on your device. None of it is transmitted to us, and none of it is transmitted to any third party as part of normal use of the app:

- Shifts, clock-in and clock-out times, and breaks
- Jobs, employers, pay rates, and the state and city you choose for wage rules
- Pay stub photos and the numbers read from them
- Notes, letters you mark as sent, and the edit history of each record
- Reports (PDF), spreadsheets (CSV), ZIP files, and encrypted backups you export

We cannot see any of it and we do not have a copy.

**Text recognition.** When you photograph a pay stub, the text is read by your phone's own text recognition — Apple Vision on iPhone, Google ML Kit bundled inside the app on Android. The photo and the text read from it do not leave your phone.

**Location.** If you tap "Use my location" while setting up a workplace, the app reads your position once to suggest the state and city whose wage rules apply. The coordinates are compared with maps built into the app; they are not stored and not sent anywhere. You can choose the place by hand instead, and the app works fully without ever granting location access.

**Exports and backups.** A wage report, spreadsheet, ZIP file, or encrypted backup is created on your phone and only leaves it when you send it somewhere yourself, using your phone's share sheet. Backups are encrypted with a password you choose; we never see the password and cannot recover it.

**App lock.** Face ID, Touch ID, fingerprint, or passcode checks are performed by your phone's operating system. EveryHour only learns whether the check passed — it never receives your biometric data.

**Reminders.** Notifications (forgot to clock out, payday, backup, an approaching pay period date) are scheduled locally on your phone. No push service is used and no notification content is sent through a server.

## 3. Data processed off the device

### 3.1 Checking the time

To make your records harder to dispute, the app asks a web server for the current time — it reads the date header of a response from `firebasestorage.googleapis.com` or `www.google.com`. The request contains nothing about you or your records; the server sees only the standard request metadata, including your IP address. You can turn this off in **Settings → "Check the time online"**.

### 3.2 Anonymous usage statistics — Google Analytics for Firebase

The app records which features are used — for example that a report was exported or a paywall was shown — together with a random identifier for the app installation and standard technical context (device model, OS version, app version, coarse region derived from IP).

These events **never** include hours, amounts of money, workplace or employer names, pay rates, or any text from a pay stub. They are not linked to your identity, and the identifier is reset if you reinstall the app or clear its data.

### 3.3 Crash reports — Google Firebase Crashlytics

When the app crashes, a report with technical details (device model, OS version, app version, the code path that failed, and a random installation identifier) is sent so we can fix the problem. Crash reports do not contain your hours, pay, workplaces, or pay stub text.

### 3.4 Purchases and subscriptions — RevenueCat, Apple, and Google

If you buy EveryHour Pro, the transaction itself is handled by Apple or Google; we never receive your payment details. RevenueCat receives the purchase details (product identifier, purchase and renewal status, platform and device information) and a random app user identifier, so the app can tell whether Pro is active and restore it on a new phone. This identifier is not tied to your name or email.

### 3.5 The in-app feedback form

If you use **Settings → Send feedback**, the following is sent to our support database (Google Firebase) so that we can read and answer it: your message, the type of feedback, any images you attach, the email address you type (if any), the app version, your platform, and a random identifier.

Only send what you are comfortable sharing — **do not attach pay stubs or other personal documents**. Sending feedback is entirely voluntary.

## 4. Permissions EveryHour asks for — and the ones it does not

| Permission | Why | Required? |
| --- | --- | --- |
| **Camera** | To photograph a pay stub so its text can be read on your device | No — you can type the figures in by hand |
| **Photo library** | Only if you pick an existing photo of a stub, or save an export | No |
| **Location** | One reading, on request, to suggest the state and city for wage rules | No — you can choose the place manually |
| **Notifications** | Local reminders (clock-out, payday, backup, pay period) | No |
| **Face ID / biometrics** | App lock, checked by the operating system | No |

EveryHour does **not** request the advertising identifier (IDFA / AAID), does not show the App Tracking Transparency prompt, does not read your contacts, calendar, or microphone, and contains no advertising SDK.

## 5. How we use the data

- To make the app work — unlock what you purchased, schedule the reminders you set, and timestamp records reliably.
- To fix problems — crash reports and, where it matters, the diagnostic details in a feedback report you sent.
- To improve the app — aggregated, anonymous usage statistics telling us which features are used and where people get stuck.
- To answer you — only when you contact us.

We do not sell your data, use it for advertising, profile you, or share it with data brokers. There are no ads in EveryHour.

## 6. Legal bases (EEA / UK)

Where the GDPR or UK GDPR applies, we rely on: **legitimate interests** for crash reporting, abuse-free operation, and anonymous product analytics (Art. 6(1)(f)); **performance of a contract** for delivering and restoring purchases (Art. 6(1)(b)); and **consent** for optional features you turn on yourself, such as sending a feedback report or granting location access (Art. 6(1)(a)), which you can withdraw at any time by stopping use of that feature or revoking the permission in system settings.

## 7. Recipients, sub-processors, and international transfers

| Recipient | Role | Data involved |
| --- | --- | --- |
| **Google LLC / Firebase** | Analytics, Crashlytics, feedback database and storage, time check | Usage events, crash reports, feedback content and attachments, IP address |
| **RevenueCat, Inc.** | Purchase / entitlement management | Anonymous purchaser ID, product ID, purchase status, device and platform info |
| **Apple Inc.** | App Store distribution, in-app purchases, Face ID, local notifications | Purchase and entitlement data |
| **Google LLC (Play)** | Google Play distribution and in-app purchases | Purchase and entitlement data |

These providers process data on servers in the United States and other countries, which may be outside your country of residence. Where required, such transfers rely on the safeguards those providers offer — including the European Commission's Standard Contractual Clauses and, where applicable, the EU–US Data Privacy Framework. Each provider processes data under its own privacy policy.

We use no advertising networks, no attribution or MMP SDKs, and no analytics providers beyond the ones named above.

## 8. Retention

| Data | Kept for |
| --- | --- |
| Everything in [section 2](#2-data-that-stays-on-your-device) (on your device) | Until you delete it in the app, use **Settings → Delete all data**, clear app data, or uninstall EveryHour |
| Analytics events | The retention period configured in Firebase Analytics — currently up to 14 months — then deleted or aggregated |
| Crash reports | Up to 90 days, per Crashlytics' retention |
| Feedback reports and attached images | While being handled, and for a reasonable period afterwards as a record; deleted earlier on request |
| Purchase / entitlement data at RevenueCat | For as long as needed to provide entitlement service, per RevenueCat's own retention policy |
| Backups and exports you saved elsewhere | Entirely under your control — delete them wherever you put them |

## 9. Your rights

Depending on where you live — including under the GDPR/UK GDPR, the CCPA/CPRA in California, and comparable laws elsewhere — you may have the right to access, correct, delete, restrict, or object to the processing of your personal information, to receive a copy of it in a portable format, to withdraw consent, and not to be discriminated against for exercising these rights.

**In practice, for EveryHour:**

- **Data on your device** — you control it directly. Edit or delete individual records in the app, use **Settings → Delete all data** to erase every record, photo, note, and export at once, or uninstall the app. We hold no copy, so there is nothing for us to delete.
- **Analytics and crash data** — reinstalling the app, or clearing app data, resets the installation identifier and disconnects future data from past data. To have data associated with your current installation deleted, email us; we will need the approximate dates so we can locate it.
- **Purchase / entitlement data at RevenueCat** — email us and we will submit a deletion request on your behalf, or contact RevenueCat directly.
- **A feedback report you sent us** — email us from the address you used, or quote the report, and we will delete the report and its attachments.

Write to **[vincenttrandeveloper@gmail.com](mailto:vincenttrandeveloper@gmail.com)**. We aim to respond within 30 days. You may also lodge a complaint with your local data protection authority; in the EEA, that is the authority for your country of residence.

## 10. Children

EveryHour is meant for working adults and is not directed at children under 13 (or the higher minimum age set by your local law, such as 16 in parts of the EEA). We do not knowingly collect personal information from children. The app contains no ads, no social features, and no user-to-user content.

If you are a parent or guardian and believe a child has sent us personal information through the feedback form, contact us and we will delete it.

## 11. Security

Data on your device is protected by the operating system's app sandbox and device encryption, and can be locked behind Face ID, a fingerprint, or a passcode. Backups are encrypted with a password only you hold. Data in transit is sent over HTTPS/TLS, and access to our Firebase project is restricted to the publisher.

No method of transmission or storage is completely secure, and we cannot guarantee absolute security.

## 12. Changes to this policy

We may update this policy as the app changes. The "Last updated" date at the top will change, and for material changes — for example a genuinely new category of data collection — we will give notice in the app or in the release notes before the change takes effect. Continuing to use the app after a change takes effect means the updated policy applies.

## 13. Contact

**Email:** [vincenttrandeveloper@gmail.com](mailto:vincenttrandeveloper@gmail.com)  
**Publisher:** WBB
