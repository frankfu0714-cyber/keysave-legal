# Key Save Privacy Policy

**Last updated:** 2026-05-16
**Operator:** Martin Fu (Key Save)
**Contact:** keysave-privacy@fufamily.com

This Privacy Policy explains how Key Save ("the app", "we", "us") handles
information when you use it on your iOS device. Plain English version: we
do not collect, transmit, sell, share, or otherwise touch your data. The
app runs entirely on your device.

## What Key Save stores

Key Save is a personal password manager. When you add a credential, the
app stores the following information you enter:

- The service or website name
- The account or username
- The password
- An optional URL
- Optional notes
- The category you select
- The date the entry was created and last updated

This data is held in a single file inside the app's private Documents
directory on your device. The file is encrypted with AES-256-GCM using a
256-bit key that is generated the first time you launch the app. The key
is stored in the iOS Keychain with accessibility
`kSecAttrAccessibleWhenUnlockedThisDeviceOnly`, which means the key
cannot be read while your device is locked and is not synced to other
devices via iCloud Keychain.

The app does not record analytics events, crash reports, telemetry,
diagnostic logs, advertising identifiers, or anything else that could
identify you or describe how you use the app.

## What Key Save does not do

- **No network requests.** Key Save does not contain any networking
  code. It does not connect to our servers (we do not run any), to
  third-party servers, or to any analytics, advertising, or
  crash-reporting service. Your passwords never leave your device by
  way of the app.
- **No third-party SDKs.** Key Save does not bundle Firebase, Mixpanel,
  Amplitude, Sentry, Crashlytics, TelemetryDeck, PostHog, or any similar
  library.
- **No accounts.** You do not register, sign in, or create a user
  profile. The app has no concept of an account.

## Device features the app uses

- **Local Authentication (Face ID / Touch ID).** If you turn on
  biometric unlock in Settings, Key Save asks iOS to verify your
  identity using `LAContext`. The biometric data itself is handled by
  iOS inside the Secure Enclave; the app only receives a yes/no answer
  and never sees your face or fingerprint data.
- **iOS Keychain.** Used to store the encryption key described above.
- **Clipboard.** When you tap the copy button on a credential, the
  value is placed on the system clipboard so you can paste it into
  another app. The app does not read your clipboard except when you
  press the "Paste" button on the Import screen.

## Backups

If you have iCloud Backup or local iTunes/Finder backup enabled, iOS
may include the encrypted vault file in your device backup as part of
the standard Documents-directory backup. Apple controls how those
backups are stored and encrypted; we do not have access to them. The
file in the backup is the same AES-256-GCM ciphertext that lives on
your device — without the matching Keychain key, the contents cannot
be decrypted.

## Sharing and selling data

We do not share, sell, rent, or transfer your data to anyone. We are
not in a position to do so, because the data never leaves your device
and we never see it.

## Your choices

- To remove every credential, use **Settings → Delete All Credentials**
  inside the app. This empties the vault and saves an empty encrypted
  file.
- To remove the app and all of its data, delete Key Save from your
  device the same way you delete any other app. The encrypted vault
  file and the Keychain entry are removed when iOS removes the app.
- To stop biometric unlock, toggle off **Face ID / Touch ID** in
  Settings inside the app.

## Children

Key Save is not designed for or directed at children under 13. We do
not knowingly collect information from any user, including children,
because we do not collect information at all.

## Changes to this policy

If we ever change how Key Save handles your data, we will update this
document and change the "Last updated" date at the top. Because
Key Save has no servers, changes to data handling can only ship as a
new version of the app released through the App Store.

## Contact

If you have questions about this policy or about how Key Save works,
write to **keysave-privacy@fufamily.com**.
