# Framemate Privacy Policy

**DRAFT — to be reviewed before publishing.** Fill in the bracketed items.
Publish at the URL in `store-content/common.json` (`privacy_url`) and in
`.env.production` (`PRIVACY_POLICY_URL`). Keep it identical in substance to
the App Privacy and Data safety answers in `docs/store-listing/app-privacy.md`.

Effective date: [date]
Developer: [developer name], [contact email]

Framemate is a camera you hand to someone else: it coaches the person holding
the phone, then helps you keep the best frames. It is built so that your
photos stay on your phone.

## The short version

- There is no account and no sign-up.
- The camera picture is analyzed on your phone, frame by frame. It is never
  uploaded, and we never see it.
- Photos you keep go to your own photo library. Photos you look at in the app
  — to learn your style or to turn one into a pose — stay on your phone.
- Pose search (Framemate Pro) sends the words you search for to Unsplash,
  the photo library it searches — in English, translated on your phone first.
  Nothing else in the app needs the internet to work.
- We use a few services to keep the app working and to sell Framemate Pro.
  They receive the limited data listed below — never a photo, a camera frame,
  a pose or the text of a search.

## What stays on your phone

**The camera.** While you shoot, the app reads each camera frame on your
phone — where the person is, their pose, their face and the light — to choose
the next instruction and the moment to shoot. This uses the phone's own image
analysis (Apple Vision on iPhone, Google ML Kit on Android). Frames are not
stored, except the short burst taken when the photo is taken: those frames
wait in the app's temporary storage until you finish reviewing them, and the
ones you do not keep are then deleted.

**Photos you keep** are saved to your photo library, in a "Framemate" album.
On iPhone the app asks only for permission to add photos for this. The app
also keeps a small thumbnail of each one on your phone, so *Your photos* can
show you what it took without permission to read your whole library. The
thumbnails never leave the phone, and Settings → *Delete all my data*
removes them.

**Photos you choose.** When you turn a photo into a pose, or pick photos for
the app to learn your style from, you choose them in the system photo picker
— the app sees only the photos you select. On iPhone, *Learn my style* can
instead read your Favorites album, if you allow access to your photos. The
photos are analyzed on your phone.

**What the app keeps.** Your saved poses (a cut-out of the person, its
outline and body points, and a copy of the photo), your style profile
(statistics only — for example how you are usually framed — never a photo),
your settings, and a history of outings without any images. A photo shared to
Framemate from another app is processed the same way, on your phone.

**Voice cues** are spoken by your phone's own text-to-speech.

**Backups.** Your phone's own backup (iCloud backup on iPhone, Google's
Android backup) may include the app's data, under your account with Apple or
Google. Framemate has no cloud copy of its own.

## What leaves your phone, and why

**Live view on a second phone** — only when you turn it on. The phone taking
the photo sends a small, low-resolution picture of what its camera sees,
about ten times a second, together with the coach's instructions and the
pose outline, straight to the one other phone you paired with the four-digit
code. In return that phone sends the directions you tap and the shutter. The
two phones talk directly — over Wi-Fi, a hotspot, or between two iPhones with
no network at all — never through the internet, never through us or anyone
else. The other phone shows the picture and keeps nothing. Each phone tells
the other its device name. Turning live view off, or leaving the screen,
ends it.

**Pose search** (Unsplash, Framemate Pro only). When you search for a pose,
the words — or the scene you tap, such as "beach" — are sent to the Unsplash
API with the app's key, and Unsplash sends back matching photos. Words you
type in another language are translated into English **on your phone**
first (Apple's Translation on iPhone, Google's ML Kit on Android, both
running on the device), and only the English is sent; the screen shows what
was searched. On Android the app downloads the translation model for your
language once, over Wi-Fi. When you choose a photo, the app downloads it
from Unsplash and tells Unsplash that the photo was downloaded, as its API
terms require — that message names the photo, not you. Unsplash receives
your device's network address and the search, as any website would. The
search text is sent nowhere else. See the Unsplash privacy policy at
<https://unsplash.com/privacy>.

**App settings from our server** (Google Firebase). Once per launch the app
reads a small settings file — for example the limits of the free version —
from Google Cloud Firestore. To keep that file to the genuine app, the phone
proves it is running the real app with Firebase App Check (Apple App Attest on
iPhone, Google Play Integrity on Android). Neither request contains anything
about you or your photos.

**Crash reports and diagnostics** (Firebase Crashlytics, Google). When the
app crashes, a report with technical details (device model, OS version, app
version, the code that failed) is sent so we can fix the problem. Crash
reports contain no photo, frame, pose or search.

**Anonymous usage statistics** (Google Analytics for Firebase). The app
records which features are used — for example that a burst was taken, a pose
was saved or a paywall was shown — with a random identifier for the app
installation. These events never include a photo, a camera frame, body points
or a pose, or the text of a search. They are not linked to your identity, and
no advertising identifier is used.

**Purchases** (RevenueCat, Apple App Store, Google Play). If you buy
Framemate Pro, the purchase is handled by Apple or Google. RevenueCat receives
the purchase details and a random app user identifier so the app can tell
whether Pro is active and restore it on a new phone. We do not receive your
payment details.

**Feedback you choose to send.** If you use "Send feedback", the message, the
type of feedback, any images you attach, the email address you type (if any),
the app version, your platform and a random identifier are sent to our
support database (Google Firebase) so we can read and answer it. Only send
what you are comfortable sharing.

We do not sell your data, use it for advertising, or share it with data
brokers. There are no ads in Framemate, and the app does not track you across
other companies' apps or websites.

## Keeping and deleting your data

- Your saved poses, style profile, history and the thumbnails of the photos
  you kept stay on your phone until you delete them. Settings → *Delete all
  my data* erases them, along with any frames waiting for review and any
  photos shared to the app that are still waiting. Deleting the app does the same. Photos you kept stay in your photo
  library; delete them there.
- Framemate Pro is not affected: it belongs to your Apple or Google account,
  and *Restore purchases* brings it back.
- To have feedback you sent removed, write to [contact email] with the email
  address you used.
- Crash reports and usage statistics are kept by Google for the periods set in
  Firebase (currently up to 90 days for crash reports and up to 14 months for
  analytics events), then deleted.

## Other people in your photos

Framemate helps someone else take your photo, and you may photograph other
people. Their pictures are handled exactly like yours: analyzed on the phone,
never uploaded, and kept only if you keep the photo. Please respect the people
you photograph and the rules of the places you shoot in.

## Children

Framemate is not directed to children under 13. We do not knowingly collect
information from children.

## Your rights

Depending on where you live (for example, in the European Union under the
GDPR, or in California under the CCPA), you may have rights to know about,
access, correct or delete personal information. Because your photos and poses
are only on your phone, you can see and delete them in the app at any time.
For anything else, contact us at [contact email].

## Changes

If this policy changes, the new version will be posted at this address with a
new effective date, and important changes will be noted in the app's release
notes.

## Contact

[developer name] — [contact email]
