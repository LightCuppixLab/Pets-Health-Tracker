# Pet Health Logbook Privacy Policy

_Last updated: June 16, 2026_

Pet Health Logbook ("the app") is a pet-health record-keeping tool developed by Light Cup Pix Lab, based in Padova, Italy. The app lets you record and review health information about your own pets. This policy explains what data we collect, why, and how we handle it, in compliance with the EU General Data Protection Regulation (GDPR).

Pet Health Logbook is available as two native apps that share the same data logic: an Android app and an iOS app. This single policy covers both. The only differences between platforms are the sign-in provider and the subscription provider, and these are explained where relevant. Everything else is identical.

Pet Health Logbook is a record-keeping tool, not a medical one: it shows your pet's data and trends, but it does not provide veterinary diagnoses and does not replace professional veterinary advice.

You can also read our Terms of Service at https://pethealthtracker.app/terms.

## Data Controller

Light Cup Pix Lab, Padova, Italy. Contact: lightcuppixlab.dev@gmail.com.

## Data we collect

### Identity (from your sign-in provider)

You sign in with a social login only. There is no password to create, and we never see or store one.

- On Android you sign in with Google (Google Sign-In).
- On iOS you sign in with Apple (Sign in with Apple).

From the sign-in provider we receive:

- your email address;
- a unique account identifier; and
- a display name.

Two specifics apply to Sign in with Apple on iOS:

- If you choose "Hide My Email", the email we receive is an Apple private relay address (in the form xxx@privaterelay.appleid.com) rather than your real address. Apple forwards mail from that relay to you. This is fully supported, and we treat the relay address exactly as we would any email.
- Apple provides your name only on the first sign-in. We store it then; if it is missing, your account simply has no display name. Apple also supplies a stable user identifier that durably identifies your account to us across sign-ins, even if your private relay email changes; we map it to the internal user identifier (UUID) used in our database.

We do not receive or use a profile photo from either provider.

Your email and name are held in our managed authentication store (Supabase Auth). In the application database tables, your records are linked only by a user identifier (UUID), so your email and name do not appear there.

### Pet data (stored on our backend)

When you use the app, the following is stored server-side so it is available to you and survives reinstalling the app:

- Pet profile: name, species, breed, sex, birth date.
- Weight history.
- Body measurements: height, abdomen.
- Vaccination records: name, date given, expiry.
- Reminders / to-dos: free-text title, due date, repeat setting, done state.
- Personal events: type, title, date, repeat, colour.
- Subscription entitlement flag: whether your account is "Pro" and its expiry. This contains no payment data (see Payments below).

### Device-only data (never uploaded to us)

The following stays on your device and is never sent to our servers:

- Pet photos.
- The pet-sitter care sheet: diet, to-do list, do-not list, medications, free-text notes, and vet & owner names and phone numbers.
- Your pet's nickname.
- App preferences: theme, language, units, notification settings, quiet hours.

You may choose to export the pet-sitter care sheet (for example to share it with your sitter or vet). Once you share such a copy yourself, it is outside our control and outside your device-backup settings.

Because this data lives on your device, it may be included in your device's system backup if you have that enabled: Google Drive on Android or iCloud on iOS. That backup is operated by your OS provider under your own account settings; we do not access it and it is outside our control. You can manage or disable it in your device settings.

## What we do NOT collect

We have verified that the app does not collect or use any of the following:

- Location data.
- Contacts.
- Advertising identifier.
- Analytics SDKs, advertising SDKs, or crash-reporting SDKs.
- Payment card data (see Payments).
- Camera access: photos are chosen through the operating system's photo picker, so the app does not access your camera or your full photo library.

## Legal basis for processing (GDPR Art. 6)

- **Performance of a contract (Art. 6(1)(b)):** to create and operate your account, store your pet records, and provide the service you asked for, including verifying a subscription purchase. We retain your subscription-entitlement record (the "Pro" flag and its expiry) on this basis for as long as your account exists, so that purchased access is honoured; it is erased when your authentication account is erased. We do not store any payment or invoice data, which are held by the app store.
- **Legitimate interests (Art. 6(1)(f)):** to keep the service secure, prevent abuse, and maintain its technical integrity. Our interest is balanced against your rights.
- **Consent (Art. 6(1)(a)):** where the platform requires you to grant a specific permission (for example, to pick a photo through the OS picker). You can withdraw such consent at any time in your device settings.

## Your rights (GDPR Art. 15–22)

You have the right to:

- Access the data we hold about you.
- Rectify inaccurate data. You can edit your pet records directly in the app at any time.
- Erase your data ("right to be forgotten"). See Data retention and deletion below.
- Restrict or object to processing.
- Data portability: receive your data in a portable form. The app does not currently offer an in-app export, so please request a copy by email and we will provide one.
- Lodge a complaint with a supervisory authority. In Italy this is the Garante per la protezione dei dati personali; you may also contact the authority in your country of residence.

To exercise any right, email lightcuppixlab.dev@gmail.com.

## Cookies and tracking technologies

The app uses no cookies and no tracking technologies. There is no analytics, no advertising, and no third-party tracker.

## Data retention and deletion

We keep your data for as long as your account exists.

- **In-app deletion:** the "Delete all my data" function removes your pets and their associated records (profiles, weight history, measurements, vaccinations, reminders, and events) from our backend, and removes the on-device photos and pet-sitter files from your device. This account-data deletion is available in the app on both platforms. (If your device's system backup is enabled, copies of the on-device data may still exist in your own Google Drive or iCloud backup, which is under your control and which we cannot access or delete.)
- **What in-app deletion does not do:** it does not by itself delete your sign-in (authentication) account. Your email and display name remain in our authentication store, and your subscription-entitlement record (the "Pro" flag and its expiry, linked to your user identifier) is retained, until the account itself is erased.
- **Full account erasure:** to delete your authentication account as well, so that no email, name, or entitlement record remains, email lightcuppixlab.dev@gmail.com and we will erase it. This is also how the right to erasure (Art. 17) is fulfilled in full.

## Sub-processors

We rely on the following providers to deliver the service:

- **Supabase:** backend hosting for authentication, the PostgreSQL database, and storage. Privacy policy: https://supabase.com/privacy
- **Google:** Google Sign-In (Android login), Google Play (Android subscriptions), and the Google Play Developer API (server-side purchase verification on Android). Privacy policy: https://policies.google.com/privacy
- **Apple:** Sign in with Apple (iOS login), the App Store (iOS subscriptions), and the App Store Server API (server-side purchase verification on iOS). Privacy policy: https://www.apple.com/legal/privacy/en-ww/

Which of Google or Apple is involved depends on the platform you use.

## International data transfers

Where a sub-processor processes data outside the European Economic Area, that transfer is protected by appropriate safeguards, in particular the European Commission's Standard Contractual Clauses (SCCs), together with any supplementary measures required.

## Reminders / notifications

Reminders are 100% local on your device. The app schedules local reminders on your device and runs an on-device check that reads your pet data and posts those reminders, honouring your notification settings and quiet hours (subject to your operating system's background-activity settings). There is no push notification service: no Firebase Cloud Messaging (FCM) and no Apple Push Notification service (APNs) server push. No notification content is sent to or through our servers.

## Payments

Subscriptions are sold by your platform's app store, which acts as the merchant of record:

- On Android, Google Play (Google Play Billing).
- On iOS, the Apple App Store (StoreKit).

The app store handles all payment and card data. No card number and no billing address ever reaches the app or our backend. The app receives only an opaque purchase token or receipt, which is transient. We verify that token server-side with the store's developer/server API (the Google Play Developer API or the App Store Server API) and store only the resulting entitlement flag (the "Pro" flag and its expiry).

You manage, renew, or cancel your subscription from your store account (your Google or Apple account), not inside the app.

## Security

- All communication between the app and our backend uses HTTPS.
- Data is isolated per user with row-level security (RLS) in the database, so one user cannot read another user's records.
- The most sensitive content, pet photos and the pet-sitter care sheet (including vet and owner phone numbers), is held device-only and is never transmitted to us.
- No password is ever created or stored, because sign-in is delegated to your trusted provider (Google or Apple).
- No method of transmission or storage is perfectly secure, but we take reasonable measures appropriate to the data involved.

## Minors

The app is intended for users aged 16 and over. It is not directed at children under 16, and we do not knowingly collect data from them. We do not ask for your age and have no means to verify it; the limit is a usage condition. If you believe a minor has provided us data, contact us and we will delete it.

## Changes

We may update this policy as the app evolves. When we do, we will revise the "Last updated" date above and publish the new version at https://pethealthtracker.app/privacy. Material changes will be brought to your attention where appropriate.

## Contact

For any privacy question or to exercise your rights, email lightcuppixlab.dev@gmail.com.
