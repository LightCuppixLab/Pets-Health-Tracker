# Privacy Policy — Pets Health Tracker

Last updated: June 16, 2026

Pets Health Tracker ("the app") is a pet-health tracker developed by
**Light Cup Pix Lab**, based in Padova, Italy. The app lets you record and
review health information about your own pets. This policy explains what data
we collect, why, and how we handle it, in compliance with the EU General Data
Protection Regulation (GDPR). It describes the app as it is currently built
and deployed.

Pets Health Tracker is a record-keeping tool, not a medical one: it shows your
pet's data and trends, but it does not provide veterinary diagnoses and does
not replace professional veterinary advice.

## Data Controller

The data controller is **Light Cup Pix Lab, Padova, Italy**.
For any privacy request, contact us at **lightcuppixlab.dev@gmail.com**.

## Data we collect

The app is built around data about *your pets*, with only the minimum personal
data about you needed to run an account.

**Information about you (your identity).** You sign in with Google. Through our
authentication provider (Supabase Auth) we receive from your Google account your
email address, a unique account identifier, and your profile display name. We use
these to create and secure your account and to show who is signed in. We do
**not** collect a password (there is no email/password login) and we do **not**
use your Google profile photo. In the app's own database tables we store only
your account identifier (a UUID) to link your records to you; your email and
name remain in the managed authentication store.

**Information about your pets (stored on our backend).** For each pet you add,
we store on our Supabase backend:

- Profile: name, species, breed, sex, and birth date (used to calculate age).
- Weight history (weight over time).
- Body measurements (height and abdomen circumference over time).
- Vaccination records (vaccine name, date given, expiry date), which drive
  expiry reminders.
- Reminders / to-dos (a title you write, due date, repeat, completion status),
  optionally linked to a pet.
- Personal events (type, title, date, repeat, colour), such as birthdays or
  grooming.
- Your subscription status (whether Pro is active, and its expiry) — see
  *Payments*.

**Information that stays only on your device.** Some data is intentionally kept
on your phone and is **never uploaded** to our backend:

- Your pets' photos.
- Your "pet-sitter" care sheet for each pet: diet, to-do and do-not lists,
  medications, free-text notes, and the vet's and owner's names and phone numbers.
- Your nickname and app preferences (theme, language, units, notification
  settings, quiet hours).

Because this on-device data lives in the app's storage, it may be included in
Android's own system backup to your personal Google Drive and in device-to-device
transfers, under Android's default backup behaviour. This is data on your own
device under your own Google account; we do not access it.

**What we do NOT collect.** We do not collect your location, your contacts, an
advertising identifier, or any analytics or tracking data. The app contains no
advertising SDK, no analytics SDK, and no crash-reporting SDK, and does not track
you across other apps or websites. We do not collect your payment card details
(see *Payments*). We do not access your camera or your broader photo gallery —
pet photos are chosen through the Android system photo picker.

## Legal basis for processing (GDPR Art. 6)

- **Performance of a contract (Art. 6(1)(b)):** We process your account identity
  and your pet records to provide the service you asked for — storing and
  displaying your pets' health information.
- **Legitimate interests (Art. 6(1)(f)):** We process the minimum technical data
  needed to keep the service secure and functioning (e.g. per-user data
  isolation and purchase verification).
- **Consent (Art. 6(1)(a)):** Local reminders are shown only after you grant the
  notification permission, and can be turned off at any time. A pet-sitter PDF is
  shared only when you actively choose to share it.

## Your rights (GDPR Art. 15–22)

You have the right to **access**, **rectify**, **erase**, **restrict**, and
**object** to the processing of your personal data, and the right to **data
portability**. In practice:

- **Access / rectification:** Most of your data is visible and editable directly
  in the app.
- **Erasure ("right to be forgotten"):** The in-app **Delete all my data** action
  removes your pets and all their records (weights, measurements, vaccines,
  events), your reminders, and your on-device photos and pet-sitter sheets. To
  also erase your underlying sign-in account — the email and display name held by
  our authentication provider — contact us at **lightcuppixlab.dev@gmail.com** and
  we will delete it without undue delay.
- **Portability / export:** To receive a copy of your stored data in a
  machine-readable format, contact us at **lightcuppixlab.dev@gmail.com**.
- **Complaint:** You may lodge a complaint with your local data protection
  authority.

You can exercise any of these rights by contacting
**lightcuppixlab.dev@gmail.com**.

## Cookies and tracking technologies

Pets Health Tracker is a native mobile app. It does **not** use cookies, web
beacons, advertising identifiers, analytics SDKs, or any third-party tracking
technology, and does not track your activity across other apps or websites.

## Data retention and deletion

We retain your pet records and account data for as long as your account exists.
When you use **Delete all my data**, the pet and reminder records and local files
listed above are removed promptly (server records are deleted, and their linked
child records are removed automatically). Your sign-in account data is removed
when you request account deletion as described under *Your rights*. On-device data
is removed when you delete it in the app or uninstall the app (subject to any
backup you have made through Android).

## Sub-processors

We rely on the following providers that process data on our behalf:

- **Supabase** — backend hosting: authentication, PostgreSQL database, and file
  storage. Stores your account identity (email, display name, account id) and
  your server-side pet records.
  Privacy policy: https://supabase.com/privacy
- **Google** (Google Sign-In / Identity, Google Play Billing, and the Google Play
  Developer API) — authentication and subscription management / purchase
  verification.
  Privacy policy: https://policies.google.com/privacy

Access to your stored records is isolated per user: our database enforces
row-level security so you can read and write only your own data, over encrypted
(HTTPS) connections.

## International data transfers

Our providers (Supabase and Google) may process data on servers located inside
or, depending on the configured region, outside the European Economic Area. Where
data is transferred outside the EEA, it is protected by appropriate safeguards
such as the European Commission's Standard Contractual Clauses (SCCs).

## Reminders / notifications

All reminders — vaccine expiries and personal events — are generated **locally on
your device**. The app runs a daily on-device check that reads your pet data and
shows local notifications according to your settings (lead time, quiet hours, and
on/off toggles). There is **no** push-notification service and no server that
decides when to notify you. Notifications require the Android notification
permission, which you can revoke at any time.

## Payments

The optional **Pro** subscription is sold and processed entirely by **Google Play
Billing**, which acts as the merchant of record. All payment collection and card
handling happen inside Google Play. The app and our backend **never** receive or
store your card number, billing address, or any payment instrument. After a
purchase, the app sends only an opaque Google Play purchase token (transiently) to
our backend, which verifies it with Google's Play Developer API and then stores
only an entitlement flag (whether Pro is active, and its expiry) linked to your
account identifier. You can manage or cancel your subscription at any time from
your Google Play account settings.

## Security

Data is transmitted over encrypted HTTPS connections and protected at the database
level by row-level security policies, so each account can access only its own
data. Pet photos and pet-sitter information (including vet and owner contact
details) are kept on your device and are not uploaded to our servers.

## Minors

Pets Health Tracker is intended for adult pet owners and is not directed to
children. We do not knowingly collect personal data from users under the age of
**16**. If you believe a minor has provided personal data, contact us at
**lightcuppixlab.dev@gmail.com** and we will delete it.

## Changes

We may update this policy from time to time. The "Last updated" date above
reflects the latest version. Material changes will be communicated through the
app where appropriate.

## Contact

- Privacy questions and data-subject requests: **lightcuppixlab.dev@gmail.com**
- Data Controller: **Light Cup Pix Lab, Padova, Italy**
