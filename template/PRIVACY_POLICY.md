# Privacy Policy — Earshot

**App:** Earshot — Voice to Text (offline speech-to-text with speaker ID)
**Bundle ID:** `com.earshot.transcription.app`
**Platforms:** iOS (App Store) only. Earshot does not ship on Android or Google Play.
**Effective date:** _[set to the App Store release date]_
**Last updated:** _[same as effective date]_
**Publisher / data controller:** _[legal entity or sole trader name]_
**Contact:** vincenttrandeveloper@gmail.com

---

## Summary — the short version

Earshot is built so that what you record stays yours.

- **Your recordings and transcripts never leave your device.** Speech-to-text,
  speaker identification, AI summaries, and search all run **on your iPhone**.
  There is no server that receives your audio, your transcripts, or anything
  derived from them (speaker labels, voice embeddings, summaries, search index).
- **There is no account.** No sign-up, no email required, no password, no
  social login. Nothing ties the app to your identity.
- **No ads, no ad SDKs, no tracking across other apps or websites.** Earshot
  does not use the advertising identifier (IDFA) and does not show the App
  Tracking Transparency prompt, because it has nothing to track you with.
- **We never sell your personal information.**
- **What does leave the device:** anonymous usage statistics and crash reports
  (to make the app work better), device-attestation tokens (to stop abuse of
  our servers), anonymous purchase/entitlement events (to unlock what you
  bought), and — only if you choose to use them — the content of a report you
  submit through the in-app feedback form, an optional AI model file you
  choose to download, or an optional iCloud backup you turn on yourself.

The rest of this policy explains each of those points precisely.

---

## 1. Scope

This policy applies to the Earshot app distributed on the Apple App Store, and
to any future updates, to the extent that the features described are actually
enabled on your device. Earshot is iOS-only; there is no Android or Google
Play version of this policy to reconcile.

It does not cover Apple's own processing of your data as the platform and
store operator — including iCloud, if you choose to use the optional backup
feature described in section 3.9 — which is governed by Apple's own privacy
policy.

## 2. Data that stays on your device

Earshot stores the following **locally on your phone only**. None of it is
transmitted to us, and none of it is transmitted to any third party as part
of normal use of the app.

| What | Details |
|---|---|
| **Audio recordings** | The `.m4a` audio file of each recording you make. |
| **Transcripts** | The text Earshot recognizes from your recording, word timestamps, and your own edits (with the original wording kept alongside your edit so you can compare or undo). |
| **Speaker data** | Which parts of a recording were spoken by which speaker, a voice embedding used to recognize the same speaker again in a later recording (Pro), and any name you give a speaker. |
| **Summaries, titles, and checklists** | AI-generated summaries, an AI-generated title, and a checklist of follow-ups Earshot extracts from a recording. |
| **Search index** | A numeric representation (embedding) of each transcript segment, used so you can search your library by meaning as well as by keyword (Pro). |
| **Tags and bookmarks** | Any tag you create and assign to a recording, and any moment in a transcript you bookmark (Pro). |
| **An optional AI model file** | If you choose to enable the improved on-device AI option (Pro), Earshot downloads one AI model file and stores it on your device so summaries and answers can be generated locally without a network connection. See section 3.6. |
| **Preferences** | Language, appearance, which AI engine you've chosen, whether Face ID lock is on, and other app settings. |
| **Purchase entitlement state** | A local record of whether a paid plan is active, so the app knows what to unlock while offline. |
| **An anonymous ID for the feedback form** | A randomly generated identifier (a UUID), created only if you open the feedback form. It is not derived from your device, phone number, email, or advertising identifier. It exists so that if you send several reports we can see they came from the same install. |
| **Your email, if you typed one into the feedback form** | Remembered locally so you do not have to retype it next time. |

**Deletion.** All of the above is removed when you delete a recording in the
app, delete the app, or clear the app's data in your device settings. Because
we never receive it, we cannot restore it for you — use the export or
iCloud backup features described below if you want a copy kept somewhere
else.

## 3. Data processed off the device

### 3.1 Usage analytics — Google Firebase Analytics

Earshot records anonymous, aggregated usage events so we can see which
features are used and where people get stuck. Examples of what is recorded:

- which screen you are viewing (Record, Library, Session Detail, Settings,
  Feedback, Paywall);
- that a recording started, finished, or failed, and roughly how long it ran
  — never its content;
- that speaker identification, a summary, or a search ran, and which engine
  produced it (the built-in free method, or the optional on-device AI model)
  — never the transcript, the summary text, the speaker names, or the search
  query itself;
- that the paywall was opened, a plan was selected, and whether a purchase
  started, completed, failed, or was cancelled — **and which plan tier**,
  never payment details;
- that "restore purchases" was tapped;
- that the app's rating prompt was shown;
- that a feedback report was submitted, and how many images were attached.

**What is never sent as analytics:** the audio itself, the text of your
transcripts, summaries, speaker names, tags, or search queries. Event values
are limited in length and stripped to plain identifiers before being sent.

Firebase assigns an **app-instance ID** to your installation and receives
basic technical context (platform, OS version, app version, device model,
coarse region/language, IP address at the time of the request). Earshot is
configured **without advertising-identifier support**, so no IDFA is
collected and this data is not used for advertising or cross-app tracking.
The app-instance ID is reset if you delete and reinstall the app, or clear
app data.

Processor: **Google LLC / Firebase** — see the
[Firebase privacy documentation](https://firebase.google.com/support/privacy).

### 3.2 Crash reports — Google Firebase Crashlytics

If the app crashes or hits a fatal error, a crash report is sent so we can
fix it. A report contains the stack trace, the app version, the device
model, the OS version, and technical state at the moment of the crash. It
does **not** contain your recordings, transcripts, or any of their content,
and it is not used to identify you.

Processor: **Google LLC / Firebase**.

### 3.3 Abuse prevention — Google Firebase App Check

Before Earshot talks to our Firebase services, it asks the operating system
to prove the app is a genuine, untampered install (**App Attest /
DeviceCheck**). The result is a short-lived attestation token. This protects
our backend from spam and abuse. The token attests the *app*, not you — it
carries no personal data and cannot be used to identify you.

Processor: **Apple Inc.** (App Attest / DeviceCheck) and **Google LLC**
(Firebase App Check).

### 3.4 Remote configuration

Earshot reads a small, public, read-only configuration document from Cloud
Firestore at startup, gated by App Check with no sign-in of any kind. It
tells the app things like whether the feedback form is currently accepting
submissions, and which on-device AI model options are currently offered.
This is a read only — nothing about you is sent. As with any network
request, Google receives your IP address and basic technical data to serve
the response.

### 3.5 The in-app feedback form (bug report / feedback / feature suggestion)

This is the only place in normal use where you deliberately send us content.
It is entirely optional — the app is fully usable without ever opening it.

When you submit a report, the following is stored in **Cloud Firestore** and
**Firebase Storage**:

- the **email address** you enter (so we can reply — you choose whether to
  give a real one);
- the **report type** (bug report, feedback, or feature suggestion);
- your **message** (up to 2,000 characters);
- up to **3 images** you attach (max 5 MB each);
- the **anonymous ID** described in section 2, the **app version**, and a
  **server timestamp**.

**Your recordings and transcripts are never attached automatically.** If you
choose to describe a problem by attaching a screenshot, only the image you
explicitly pick is uploaded — the photo picker never gives Earshot access to
your photo library as a whole, and Earshot does not read location or other
metadata from the images you attach.

**Retention.** Reports are kept while we work through them and for a
reasonable period afterwards as a record of what was fixed and why. You can
ask us to delete your report and its attachments at any time — see
section 9.

### 3.6 Optional on-device AI model download (Pro)

If you turn on the improved on-device AI option in Settings, Earshot
downloads one AI model file over HTTPS from a third-party file-hosting
service, **Hugging Face**, and stores it on your device. This is a plain
file download: your device's IP address and standard request metadata reach
Hugging Face's servers, exactly as with any file download from any website,
but **no recording, transcript, or other content of yours is sent as part of
this download** — the traffic only pulls a generic, publicly published model
file, it never uploads anything. Once downloaded, the model runs entirely on
your device; nothing about how you use it is sent anywhere.

Processor: **Hugging Face, Inc.** — file delivery only, no personal data
exchanged.

### 3.7 Purchases and subscriptions — RevenueCat and Apple

Earshot offers optional paid plans (monthly, yearly, and a one-time lifetime
purchase). Payment itself is processed **entirely by Apple** through the App
Store on your device.

- We never see or receive your card number, bank details, or billing
  address.
- Earshot uses **RevenueCat** to determine which plan is active and unlock
  the right features. RevenueCat receives an **anonymous, RevenueCat-generated
  identifier** for your install (Earshot does not log this identifier in with
  any account, because there is no account), which App Store product you
  purchased, whether it is active, and basic device/platform information.
  This entitlement state is also cached locally so the app knows what to
  unlock while offline.
- "Restore purchases" asks Apple and RevenueCat to re-report purchases
  already tied to your Apple Account.
- Managing or cancelling a subscription opens Apple's own subscription
  management screen.

Processors: **RevenueCat, Inc.** (entitlement management) and **Apple Inc.**
(App Store billing). Apple's handling of your purchase data is governed by
Apple's privacy policy, not this one; RevenueCat's is governed by
[RevenueCat's privacy policy](https://www.revenuecat.com/privacy/).

### 3.8 Optional iCloud backup (Pro)

If you turn on iCloud backup in Settings, Earshot writes a copy of your
session library — transcripts, speaker data, and the audio files — into a
private container inside **your own iCloud account**, so a lost or new phone
does not mean a lost library. This is:

- **off by default** — nothing is backed up unless you turn it on;
- **one-way**, restore-on-demand — Earshot writes files there and can read
  them back to restore a library, but this is not a live, continuous,
  multi-device sync;
- **stored under your Apple ID's iCloud storage**, not on a server we
  operate. We never receive a copy of it. Apple's handling of the data in
  your iCloud account is governed by Apple's own privacy policy, and it
  counts against your iCloud storage quota.

### 3.9 Notifications and Live Activity

Earshot does not send push notifications and has no push infrastructure — it
registers no push token and cannot message you from our side. While
recording, the app can show a **Live Activity** (Lock Screen / Dynamic
Island) with the current recording duration (Pro); this is drawn locally by
the app on your device and involves no server or notification service.

### 3.10 Rating prompt

Earshot may ask the operating system to display the **native App Store
rating dialog**. The dialog, and any review you write in it, are handled by
Apple. We only record internally that the prompt was shown (see
section 3.1); we never see whether or how you rated the app.

## 4. Permissions Earshot asks for — and the ones it does not

| Permission | Why | Required? |
|---|---|---|
| **Microphone** | To record the audio you choose to capture. Recordings never leave your device. | Required to record |
| **Speech Recognition** | To transcribe your recordings to text entirely on your device. Nothing is sent to a server as part of this. | Required to transcribe |
| **Face ID** | To lock the app, or a single recording (Pro), so only you can open it. Face ID matching happens entirely within the operating system; Earshot never sees or stores your biometric data. | Optional |
| **Photo library (selected photos only)** | To attach an image to a feedback report you are sending us. The system photo picker is used, so Earshot never gets access to your photo library as a whole. | Optional |

Earshot deliberately does **not** request or use: camera, contacts, location,
calendar, reminders, health data, motion sensors, or the advertising
identifier / App Tracking Transparency prompt.

## 5. How we use the data

We process the limited data described above to:

- provide recording, transcription, speaker identification, summaries,
  search, and export;
- keep the app stable — diagnosing crashes and errors;
- understand which features are used, so we know what to improve;
- unlock paid features you bought, via Apple and RevenueCat;
- reply to a feedback report you sent us, and fix what it describes;
- protect our services from abuse and comply with legal obligations.

We do **not** use your data for advertising, profiling, automated
decision-making, or cross-app or cross-site tracking. **We do not sell
personal information**, and we do not "share" it for cross-context
behavioural advertising as those terms are used in California law.

## 6. Legal bases (EEA / UK)

Where the GDPR or UK GDPR applies to you:

| Purpose | Legal basis |
|---|---|
| Providing the app's features | Performance of a contract (Art. 6(1)(b)) |
| Crash reporting, abuse prevention, security | Legitimate interests (Art. 6(1)(f)) — keeping the app working and our services safe |
| Usage analytics | Legitimate interests (Art. 6(1)(f)), or your consent where local law requires it |
| Handling a feedback report you send us | Performance of a contract / your consent (Art. 6(1)(a)) — you choose to send it |
| Purchases and entitlement | Performance of a contract (Art. 6(1)(b)) |
| Optional AI model download / iCloud backup | Your consent — you turn each on yourself (Art. 6(1)(a)) |
| Legal and record-keeping obligations | Legal obligation (Art. 6(1)(c)) |

You may object to processing based on legitimate interests, and withdraw
consent at any time — for the optional features above, by turning them off
in Settings.

## 7. Recipients, sub-processors, and international transfers

| Recipient | Role | Data involved |
|---|---|---|
| **Google LLC / Firebase** | Analytics, Crashlytics, App Check, Firestore, Storage, Remote Config | Usage events, crash reports, attestation tokens, feedback content, IP address |
| **RevenueCat, Inc.** | Purchase/entitlement management | Anonymous purchaser ID, product ID, purchase status, device/platform info |
| **Apple Inc.** | App Store distribution, in-app purchases, App Attest, optional iCloud backup, Face ID, rating prompt | Purchase and entitlement data, attestation, iCloud-stored backup (under your own Apple ID) |
| **Hugging Face, Inc.** | Delivery of an optional, publicly published AI model file | IP address and standard request metadata only — no personal content |

These providers process data on servers in the United States and other
countries, which may be outside your country of residence. Where required,
such transfers rely on the safeguards those providers offer — including the
European Commission's Standard Contractual Clauses and, where applicable,
the EU–US Data Privacy Framework. Each provider processes data under its own
privacy policy.

We use no advertising networks, no attribution or MMP SDKs, and no analytics
providers beyond the ones named above.

## 8. Retention

| Data | Kept for |
|---|---|
| Everything in section 2 (on your device) | Until you delete it in the app, clear app data, or uninstall Earshot |
| Analytics events | For the retention period configured in Firebase Analytics (by default up to 14 months for event-level data), then deleted or aggregated |
| Crash reports | Typically up to 90 days, per Crashlytics' retention |
| Feedback reports and attached images | While being handled, and for a reasonable period afterwards as a record; deleted earlier on request |
| Purchase/entitlement data at RevenueCat | For as long as needed to provide entitlement service, per RevenueCat's own retention policy |
| iCloud backup (if enabled) | Until you turn the feature off, delete the backup, or delete your iCloud data — controlled entirely by you |
| App Check tokens | Short-lived; refreshed automatically and not retained as records |

## 9. Your rights

Depending on where you live — including under the GDPR/UK GDPR, the
CCPA/CPRA in California, and comparable laws elsewhere — you may have the
right to access, correct, delete, restrict, or object to the processing of
your personal information, to receive a copy of it in a portable format, to
withdraw consent, and not to be discriminated against for exercising these
rights.

**In practice, for Earshot:**

- **Data on your device** — you control it directly. Delete individual
  recordings in the app, clear the app's data in system settings, or
  uninstall the app. We hold no copy, so there is nothing for us to delete.
- **Analytics and crash data** — reinstalling the app, or clearing app data,
  resets the app-instance ID and disconnects future data from past data. To
  have data associated with your current installation deleted, email us; we
  will need the approximate dates so we can locate it.
- **Purchase/entitlement data at RevenueCat** — email us and we will submit
  a deletion request on your behalf, or contact RevenueCat directly.
- **A feedback report you sent us** — email us from the address you used, or
  quote the report, and we will delete the report and its attachments.
- **iCloud backup** — delete it yourself from Settings, or from your
  iCloud storage settings; we never hold a copy.

Write to **vincenttrandeveloper@gmail.com**. We aim to respond within 30
days. You may also lodge a complaint with your local data protection
authority; in the EEA, that is the authority for your country of residence.

## 10. Children

Earshot is a general-audience utility app. It is not directed at children
under 13 (or the higher minimum age set by your local law, such as 16 in
parts of the EEA), and we do not knowingly collect personal information from
children. The app contains no ads, no social features, no user-to-user
content, and no external links other than to the App Store.

If you are a parent or guardian and believe a child has sent us personal
information through the feedback form, contact us and we will delete it.

## 11. Recording other people

Earshot lets you record audio you capture with your device's microphone,
including conversations with other people. **You are responsible for
complying with the law that applies to you** — including any requirement to
obtain the other participants' consent before recording a conversation,
which varies by country, and in the United States, by state. We do not
monitor, moderate, or have access to what you record, and we cannot advise
you on the recording-consent law in your specific situation.

## 12. Security

Data on your device is protected by the operating system's app sandbox and
device encryption. Data in transit is sent over HTTPS/TLS. Access to our
Firebase project is restricted to the publisher, requests are attested with
App Check, and Firestore security rules limit what the app can read and
write.

No method of transmission or storage is completely secure, and we cannot
guarantee absolute security.

## 13. Changes to this policy

We may update this policy as the app changes. The "Last updated" date at the
top will change, and for material changes — for example a genuinely new
category of data collection — we will give notice in the app or on the store
listing before the change takes effect. Continuing to use the app after a
change takes effect means the updated policy applies.

## 14. Contact

- **Email:** vincenttrandeveloper@gmail.com
- **Publisher:** _[legal entity or sole trader name]_
- **Postal address:** _[postal address]_

---

## Appendix — App Store privacy label mapping (internal reference)

Not part of the published policy. Kept here so the App Store Connect "App
Privacy" questionnaire stays consistent with this document. Earshot does not
ship on Android/Google Play, so there is no Play Data Safety table to keep in
sync — add one if that ever changes.

| Category | Collected | Linked to identity | Tracking | Purpose |
|---|---|---|---|---|
| Identifiers → Device ID (Firebase app-instance ID) | Yes | No | No | Analytics, App Functionality |
| Identifiers → User ID (RevenueCat anonymous ID) | Yes | No | No | App Functionality (entitlement) |
| Usage Data → Product Interaction | Yes | No | No | Analytics |
| Diagnostics → Crash Data, Performance Data | Yes | No | No | App Functionality |
| Contact Info → Email Address | Yes (feedback form only) | No | No | Developer Communications, Support |
| User Content → Photos | Yes (feedback form only) | No | No | Developer Communications, Support |
| **Audio Data** (recordings) | **No** — recorded, transcribed, and stored on-device only; never collected by us | — | — | — |
| User Content → Other User Content (transcripts, summaries, speaker data, tags) | **No** — processed and stored on-device only, never collected by us | — | — | — |
| Purchases → Purchase History | Yes — via RevenueCat, to determine entitlement | No | No | App Functionality |
| Location, Contacts, Health, Financial Info, Browsing History, Search History, Sensitive Info | No | — | — | — |

**Tracking:** No. No ad identifier, no third-party ad or attribution SDK, no
ATT prompt.

### Publishing checklist

- [ ] Fill in the publisher legal name, postal address, and effective date
      above.
- [ ] Publish this document at a stable public HTTPS URL (plain HTML is
      fine), and update `PRIVACY_POLICY_URL` in every `.env.<environment>`
      file and `store-content/common.json` to point at it — they must match.
- [ ] Set that URL as the privacy policy URL in **App Store Connect**.
- [ ] Link it from the app's Settings screen alongside the Terms of Use.
- [ ] Re-check the Appendix declarations whenever a new SDK, permission, or
      network call is added — most importantly, if the on-device AI model or
      diarization pipeline is ever changed to call out to a network service
      instead of running locally.
