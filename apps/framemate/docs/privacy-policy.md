---
sidebar_position: 2
title: Privacy Policy
---

# Privacy Policy

**App:** Framemate — Photo Coach (a camera that coaches the person holding the phone)  
**Platforms:** iOS (App Store) and Android (Google Play)  
**Effective date:** November 16, 2026  
**Last updated:** November 16, 2026  
**Publisher / data controller:** WBB  
**Contact:** [vincenttrandeveloper@gmail.com](mailto:vincenttrandeveloper@gmail.com)

---

## Summary — the short version

Framemate is a camera you hand to someone else: it coaches the person holding the phone, then helps you keep the best frames. It is built so that your photos stay on your phone.

- **There is no account and no sign-up.** No email, no password, no social login.
- **The camera picture is analysed on your phone, frame by frame.** It is never uploaded, and we never see it.
- **Photos you keep go to your own photo library.** Photos you look at in the app — to learn your style, or to turn one into a pose — stay on your phone.
- **Pose search (Framemate Pro)** sends the words you search for to Unsplash, the photo library it searches, in English, translated on your phone first. Nothing else in the app needs the internet to work.
- **No ads, no ad SDKs, no tracking across other apps or websites.** We never sell your personal information.
- **What does leave the device:** a small settings file the app reads at launch, anonymous usage statistics, crash reports, purchase/entitlement events — and, only if you choose to send one, the content of a feedback report. **Never** a photo, a camera frame, a pose, or the text of a search.

The rest of this policy explains each of those points precisely.

---

## 1. Scope

This policy applies to the Framemate app distributed on the Apple App Store and Google Play, and to any future updates, to the extent that the features described are actually enabled on your device.

It does not cover Apple's or Google's own processing of your data as the platform and store operator — including your phone's own device backup, described in [section 2.6](#26-backups) — or the processing done by Unsplash when you use pose search, which is governed by their own privacy policies.

## 2. Data that stays on your device

### 2.1 The camera

While you shoot, the app reads each camera frame **on your phone** — where the person is, their pose, their face, and the light — to choose the next instruction and the moment to shoot. This uses the phone's own image analysis: **Apple Vision** on iPhone, **Google ML Kit** on Android. Both run entirely on the device.

Frames are not stored, with one exception: the short burst taken at the moment of the shot. Those frames wait in the app's temporary storage until you finish reviewing them, and the ones you do not keep are then deleted.

### 2.2 Photos you keep

Photos you keep are saved to your photo library, in a "Framemate" album. On iPhone the app asks only for permission to **add** photos for this — it does not need access to your existing library.

The app also keeps a small thumbnail of each one on your phone, so **Your photos** can show you what it took without permission to read your whole library. The thumbnails never leave the phone, and **Settings → Delete all my data** removes them.

### 2.3 Photos you choose

When you turn a photo into a pose, or pick photos for the app to learn your style from, you choose them in the **system photo picker** — the app sees only the photos you select. On iPhone, **Learn my style** can instead read your Favorites album, if you allow access to your photos. In every case the photos are analysed on your phone.

### 2.4 What the app keeps

Stored in the app's private storage on your device, and never transmitted to us:

- **Your saved poses** — a cut-out of the person, its outline and body points, and a copy of the photo
- **Your style profile** — statistics only, for example how you are usually framed; never a photo
- **Your settings**
- **A history of your outings**, without any images

A photo shared to Framemate from another app is processed the same way, on your phone.

### 2.5 Voice cues

Spoken instructions use your phone's own text-to-speech. Nothing is sent to a server to be spoken.

### 2.6 Backups

Your phone's own backup — iCloud backup on iPhone, Google's Android backup — may include the app's data, under your account with Apple or Google and subject to their terms. Framemate has no cloud copy of its own.

## 3. Data processed off the device

### 3.1 Live view on a second phone — phone to phone, never through us

This runs **only when you turn it on**. The phone taking the photo sends a small, low-resolution picture of what its camera sees, about ten times a second, together with the coach's instructions and the pose outline, straight to the one other phone you paired with the four-digit code. In return, that phone sends the directions you tap and the shutter.

The two phones talk **directly** — over Wi-Fi, a hotspot, or between two iPhones with no network at all. The pictures never travel through the internet, through us, or through anyone else. The other phone shows the picture and keeps nothing. Each phone tells the other its device name. Turning live view off, or leaving the screen, ends it.

### 3.2 Pose search — Unsplash (Framemate Pro only)

When you search for a pose, the words — or the scene you tap, such as "beach" — are sent to the **Unsplash API** with the app's key, and Unsplash sends back matching photos.

Words you type in another language are translated into English **on your phone** first (Apple's Translation on iPhone, Google's ML Kit on Android, both running on the device), and only the English is sent; the screen shows what was searched. On Android the app downloads the translation model for your language once, over Wi-Fi.

When you choose a photo, the app downloads it from Unsplash and tells Unsplash that the photo was downloaded, as its API terms require — that message names the photo, not you. Unsplash receives your device's network address and the search, as any website would. The search text is sent nowhere else. See the [Unsplash privacy policy](https://unsplash.com/privacy).

### 3.3 App settings from our server — Google Firebase

Once per launch the app reads a small settings file — for example the limits of the free version — from **Google Cloud Firestore**. To keep that file to the genuine app, the phone proves it is running the real app with **Firebase App Check** (Apple App Attest on iPhone, Google Play Integrity on Android). Neither request contains anything about you or your photos.

### 3.4 Crash reports — Google Firebase Crashlytics

When the app crashes, a report with technical details (device model, OS version, app version, the code path that failed, and a random installation identifier) is sent so we can fix the problem. Crash reports contain **no photo, frame, pose, or search**.

### 3.5 Anonymous usage statistics — Google Analytics for Firebase

The app records which features are used — for example that a burst was taken, a pose was saved, or a paywall was shown — together with a random identifier for the app installation and standard technical context (device model, OS version, app version, coarse region derived from IP).

These events **never** include a photo, a camera frame, body points, a pose, or the text of a search. They are not linked to your identity, no advertising identifier is used, and the identifier is reset if you reinstall the app or clear its data.

### 3.6 Purchases and subscriptions — RevenueCat, Apple, and Google

If you buy Framemate Pro, the transaction itself is handled by Apple or Google; we never receive your payment details. **RevenueCat** receives the purchase details (product identifier, purchase and renewal status, platform and device information) and a random app user identifier, so the app can tell whether Pro is active and restore it on a new phone. This identifier is not tied to your name or email.

### 3.7 The in-app feedback form

If you use **Settings → Send feedback**, the following is sent to our support database (Google Firebase) so that we can read and answer it: your message, the type of feedback, any images you attach, the email address you type (if any), the app version, your platform, and a random identifier.

Only send what you are comfortable sharing. Sending feedback is entirely voluntary.

## 4. Permissions Framemate asks for — and the ones it does not

| Permission | Why | Required? |
| --- | --- | --- |
| **Camera** | To coach the shot and take the photo, analysed on your device | Yes — the app is a camera |
| **Add to photo library** | To save the photos you keep into the "Framemate" album | No — you can review without keeping |
| **Read photo library** | Only for *Learn my style* reading your Favorites on iPhone; otherwise you pick photos in the system picker instead | No |
| **Local network / nearby devices** | Live view between the two paired phones | No — only if you use live view |

Framemate does **not** request the advertising identifier (IDFA / AAID), does not show the App Tracking Transparency prompt, does not read your contacts, calendar, location, or microphone, and contains no advertising SDK.

## 5. How we use the data

- To make the app work — unlock what you purchased, and read the settings file that configures the free version's limits.
- To fix problems — crash reports and, where it matters, the diagnostic details in a feedback report you sent.
- To improve the app — aggregated, anonymous usage statistics telling us which features are used and where people get stuck.
- To answer you — only when you contact us.

We do not sell your data, use it for advertising, profile you, or share it with data brokers. There are no ads in Framemate, and the app does not track you across other companies' apps or websites.

## 6. Legal bases (EEA / UK)

Where the GDPR or UK GDPR applies, we rely on: **legitimate interests** for crash reporting, abuse-free operation of our settings endpoint, and anonymous product analytics (Art. 6(1)(f)); **performance of a contract** for delivering and restoring purchases and for running a pose search you ask for (Art. 6(1)(b)); and **consent** for optional features you turn on yourself, such as sending a feedback report, granting photo access, or starting live view (Art. 6(1)(a)), which you can withdraw at any time by stopping use of that feature or revoking the permission in system settings.

## 7. Recipients, sub-processors, and international transfers

| Recipient | Role | Data involved |
| --- | --- | --- |
| **Google LLC / Firebase** | Settings file and App Check, Analytics, Crashlytics, feedback database and storage | Attestation token, usage events, crash reports, feedback content and attachments, IP address |
| **Unsplash Inc.** | Pose search and photo download (Pro) | The English search text, the downloaded photo's identifier, IP address |
| **RevenueCat, Inc.** | Purchase / entitlement management | Anonymous purchaser ID, product ID, purchase status, device and platform info |
| **Apple Inc.** | App Store distribution, in-app purchases, App Attest, on-device Vision and Translation | Purchase and entitlement data, attestation |
| **Google LLC (Play)** | Google Play distribution, in-app purchases, Play Integrity, on-device ML Kit | Purchase and entitlement data, attestation |

The other phone in a live view session is **not** a recipient in this sense: nothing passes through a server, and the picture is sent only to the phone you paired with yourself.

These providers process data on servers in the United States and other countries, which may be outside your country of residence. Where required, such transfers rely on the safeguards those providers offer — including the European Commission's Standard Contractual Clauses and, where applicable, the EU–US Data Privacy Framework. Each provider processes data under its own privacy policy.

We use no advertising networks, no attribution or MMP SDKs, and no analytics providers beyond the ones named above.

## 8. Retention

| Data | Kept for |
| --- | --- |
| Everything in [section 2](#2-data-that-stays-on-your-device) — poses, style profile, outing history, thumbnails, settings | Until you delete it in the app, use **Settings → Delete all my data**, clear app data, or uninstall Framemate |
| Burst frames waiting for review, and photos shared to the app | Until you finish reviewing; frames you do not keep are then deleted. **Delete all my data** erases any still waiting |
| Photos you kept | In your own photo library, until you delete them there |
| Analytics events | The retention period configured in Firebase Analytics — currently up to 14 months — then deleted or aggregated |
| Crash reports | Up to 90 days, per Crashlytics' retention |
| Feedback reports and attached images | While being handled, and for a reasonable period afterwards as a record; deleted earlier on request |
| Purchase / entitlement data at RevenueCat | For as long as needed to provide entitlement service, per RevenueCat's own retention policy |

Framemate Pro is not affected by deleting your data: it belongs to your Apple or Google account, and **Restore purchases** brings it back.

## 9. Your rights

Depending on where you live — including under the GDPR/UK GDPR, the CCPA/CPRA in California, and comparable laws elsewhere — you may have the right to access, correct, delete, restrict, or object to the processing of your personal information, to receive a copy of it in a portable format, to withdraw consent, and not to be discriminated against for exercising these rights.

**In practice, for Framemate:**

- **Data on your device** — you control it directly. Because your photos and poses are only on your phone, you can see and delete them in the app at any time, or use **Settings → Delete all my data** to erase everything at once. We hold no copy, so there is nothing for us to delete.
- **Analytics and crash data** — reinstalling the app, or clearing app data, resets the installation identifier and disconnects future data from past data. To have data associated with your current installation deleted, email us; we will need the approximate dates so we can locate it.
- **Purchase / entitlement data at RevenueCat** — email us and we will submit a deletion request on your behalf, or contact RevenueCat directly.
- **A feedback report you sent us** — email us from the address you used, or quote the report, and we will delete the report and its attachments.

Write to **[vincenttrandeveloper@gmail.com](mailto:vincenttrandeveloper@gmail.com)**. We aim to respond within 30 days. You may also lodge a complaint with your local data protection authority; in the EEA, that is the authority for your country of residence.

## 10. Other people in your photos

Framemate helps someone else take your photo, and you may photograph other people. Their pictures are handled exactly like yours: analysed on the phone, never uploaded, and kept only if you keep the photo. Please respect the people you photograph and the rules of the places you shoot in.

## 11. Children

Framemate is not directed to children under 13 (or the higher minimum age set by your local law, such as 16 in parts of the EEA). We do not knowingly collect personal information from children. The app contains no ads, no social features, and no user-to-user content beyond the live view you start yourself between two phones you hold.

If you are a parent or guardian and believe a child has sent us personal information through the feedback form, contact us and we will delete it.

## 12. Security

Data on your device is protected by the operating system's app sandbox and device encryption. Requests for the settings file are gated by Firebase App Check, so only the genuine app can read it. Data in transit is sent over HTTPS/TLS, and access to our Firebase project is restricted to the publisher. Live view is a direct link between the two phones you paired and does not pass through any server of ours.

No method of transmission or storage is completely secure, and we cannot guarantee absolute security.

## 13. Changes to this policy

We may update this policy as the app changes. The "Last updated" date at the top will change, and for material changes — for example a genuinely new category of data collection — we will give notice in the app or in the release notes before the change takes effect. Continuing to use the app after a change takes effect means the updated policy applies.

## 14. Contact

**Email:** [vincenttrandeveloper@gmail.com](mailto:vincenttrandeveloper@gmail.com)  
**Publisher:** WBB
