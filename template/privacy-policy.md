# EveryHour Privacy Policy

**DRAFT — to be reviewed before publishing.** Fill in the bracketed items.
Publish at the URL in `store-content/common.json` (`privacy_url`) and in
`.env.production` (`PRIVACY_POLICY_URL`).

Effective date: [date]
Developer: [developer name], [contact email]

EveryHour is an hours tracker and pay stub checker for hourly workers in the
United States. It is built so that your work records stay on your phone.

## The short version

- There is no account and no sign-up.
- Your hours, breaks, pay rates, workplaces, pay stub photos, notes and
  reports are stored on your phone and are not sent to us.
- Pay stub photos are read on your phone. They are never uploaded.
- We use a few services to keep the app working and to sell EveryHour Pro.
  They receive the limited data listed below, never your hours or pay.

## What stays on your phone

Everything you enter or create in EveryHour: shifts and breaks, jobs and pay
rates, the state and city you choose, pay stub photos and the numbers read
from them, notes, letters you mark as sent, and the reports, spreadsheets
and backups you export. This data is kept in the app's private storage on
your device. We cannot see it and we do not have a copy.

**Text recognition.** When you photograph a pay stub, the text is read by
your phone's own text recognition (Apple Vision on iPhone, Google ML Kit
bundled in the app on Android). The photo and its text do not leave your
phone.

**Location.** If you tap "Use my location" while setting up a workplace, the
app reads your position once to suggest the state and city whose wage rules
apply. The coordinates are compared with maps built into the app; they are
not stored and not sent anywhere. You can choose the place by hand instead.

**Exports and backups.** A wage report (PDF), spreadsheets (CSV), a ZIP file
or an encrypted backup is created on your phone and only leaves it when you
send it somewhere yourself, using your phone's share sheet. Backups are
encrypted with a password you choose; we never see the password and cannot
recover it.

**App lock.** Face ID, fingerprint or passcode checks are done by your
phone's operating system. EveryHour only learns whether the check passed.

**Reminders.** Notifications (forgot to clock out, payday, backup, a coming
date for a pay period) are scheduled on your phone. No push service is used.

## What leaves your phone, and why

**Checking the time.** To make your records harder to dispute, the app asks
a web server for the current time (it reads the date of a response from
`firebasestorage.googleapis.com` or `www.google.com`). The request contains
nothing about you or your records. You can turn this off in Settings
("Check the time online").

**Crash reports and diagnostics** (Firebase Crashlytics, Google). When the
app crashes, a report with technical details (device model, OS version, app
version, the code that failed) is sent so we can fix the problem. Crash
reports do not contain your hours, pay, workplaces or pay stub text.

**Anonymous usage statistics** (Google Analytics for Firebase). The app
records which features are used — for example that a report was exported or
a paywall was shown — with a random identifier for the app installation.
These events never include hours, amounts of money, workplace or employer
names, or text from a pay stub. They are not linked to your identity.

**Purchases** (RevenueCat, Apple App Store, Google Play). If you buy
EveryHour Pro, the purchase is handled by Apple or Google. RevenueCat
receives the purchase details and a random app user identifier so the app
can tell whether Pro is active and restore it on a new phone. We do not
receive your payment details.

**Feedback you choose to send.** If you use "Send feedback", the message,
the type of feedback, any images you attach, the email address you type (if
any), the app version, your platform and a random identifier are sent to our
support database (Google Firebase) so we can read and answer it. Only send
what you are comfortable sharing; do not attach pay stubs or other personal
documents.

We do not sell your data, use it for advertising, or share it with data
brokers. There are no ads in EveryHour.

## Keeping and deleting your data

- Your records stay on your phone until you delete them. Settings → "Delete
  all data" erases every record, photo, note and export from the app on this
  phone. Deleting the app does the same.
- Backups and exports you saved elsewhere (Files, iCloud Drive, Google
  Drive, email) are under your control; delete them there.
- To have feedback you sent removed, write to [contact email] with the email
  address you used.
- Crash reports and usage statistics are kept by Google for the periods set
  in Firebase (currently up to 90 days for crash reports and up to 14 months
  for analytics events), then deleted.

## Children

EveryHour is meant for working adults and is not directed to children under
13. We do not knowingly collect information from children.

## Your rights

Depending on where you live (for example, California under the CCPA), you
may have rights to know about, access, correct or delete personal
information. Because your records are only on your phone, you can see,
change and delete them in the app at any time. For anything else, contact us
at [contact email].

## Changes

If this policy changes, the new version will be posted at this address with
a new effective date, and important changes will be noted in the app's
release notes.

## Contact

[developer name] — [contact email]
