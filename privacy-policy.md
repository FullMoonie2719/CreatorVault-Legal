# CreatorVault Privacy Policy

Last updated: 8 October 2026

## Who operates CreatorVault

CreatorVault is operated by **Scott Hall**. Privacy and data-protection
questions can be sent to **Tracksuitchav@proton.me**.

## What CreatorVault does

CreatorVault is a private creator-media workflow. It lets signed-in users select and
upload media to a private Vault, organise and tag it, review draft metadata, run
creator-triggered AI analysis, prepare content against configured platform guidance,
export selected content, and delete stored content or the account.

CreatorVault does not automatically publish media.

## Information we process

### Account information

We process the email address and internal account identifier needed to create,
authenticate, secure, recover, export, and delete a CreatorVault account.

### Media selected by the user

CreatorVault processes photos and videos only when the user explicitly chooses them
through a file picker, selected folder, or supported Android cloud-media picker.

Uploaded media is stored privately for the signed-in account. CreatorVault records
technical metadata needed to operate the Vault, such as file name, MIME type, file
size, image dimensions where available, video duration where available, SHA-256
checksum, private storage path, processing status, and thumbnail path.

For videos, CreatorVault generates a private thumbnail for preview and AI analysis.
Under the current architecture, raw video is not sent to the AI provider.

### Creator workflow data

We process creator-entered titles, descriptions, captions, tags, favourites,
collections, review decisions, preparation/rule-check results, export metadata,
processing status, draft AI suggestions, and security-relevant audit/activity
records.

## How we use information

We process this information to:

- authenticate and secure accounts;
- provide private media storage and previews;
- detect exact duplicate uploads;
- organise media, tags, collections, and favourites;
- provide review and preparation workflows;
- provide creator-triggered AI draft suggestions;
- export creator-selected content and metadata;
- operate account/media deletion and data export;
- diagnose failures, prevent abuse, and maintain security.

CreatorVault does not sell creator media or personal information and does not use
creator media for advertising.

## Service providers

CreatorVault currently uses:

- **Supabase** for authentication, PostgreSQL database services, private object
  storage, signed URLs, and server-side Edge Functions.
- **Cloudflare Workers AI** for creator-triggered AI inference.

These providers process information as part of delivering CreatorVault's services.
Provider/admin credentials are kept server-side and are not embedded in the mobile
application.

## AI processing

AI analysis happens only after the creator explicitly requests it.

For an image, CreatorVault may create a short-lived private signed preview and pass
that through the server-side analysis flow to Cloudflare Workers AI.

For a video, CreatorVault sends the generated private thumbnail rather than the raw
video under the current architecture.

AI results are draft suggestions. They do not automatically replace creator data or
publish content. The creator remains responsible for reviewing and approving the
result.

## Private storage and security

Creator media is stored in private, user-isolated storage. Database access uses Row
Level Security and creator-owned records. Private previews use time-limited signed
URLs.

CreatorVault uses HTTPS/TLS for network traffic. The Android application explicitly
disables cleartext traffic and excludes app-private files, databases, shared
preferences, and device-protected data from Android cloud backup/device transfer.

No Supabase service-role key, Cloudflare AI credential, or other administrator
secret is included in the mobile app.

## Android photo and video access

CreatorVault does not request broad Android photo/video library permissions. It uses
user-driven file/folder selection and the Android system Photo Picker where
supported. This gives CreatorVault access only to media the user explicitly chooses
for the relevant workflow.

## Retention

Account and private workflow data are retained while the account is active unless
the creator deletes individual content sooner.

Short-lived signed preview URLs expire automatically. Temporary local staging/export
files are cleaned as part of their workflows.

If a narrow category of information must be retained for security, fraud prevention,
legal compliance, or another lawful requirement, that retained information should be
described and limited to the purpose and duration required.

## Export and deletion

Users can export account metadata from **Settings > Your data**.

Users can permanently delete their CreatorVault account from **Settings > Your
data > Permanently delete account**. Deletion requires confirmation and
reauthentication.

When an account-deletion request is completed, CreatorVault is designed to remove
the login, associated private media, and associated account records, except for any
information that must lawfully be retained for a clearly disclosed reason.

Users who no longer have the app can [request account deletion](account-deletion.md).

## Adult-only use and content rights

CreatorVault is intended for users aged 18 or older. Users must have the rights and
legally required consent for content they upload. Content involving minors,
uncertain age, coercion, exploitation, or non-consensual activity is prohibited.

## Changes to this policy

This policy may be updated when CreatorVault's features, providers, legal
requirements, or data practices change. The published version should show the date
of the latest revision.

## Contact

Privacy, security, support, and account-deletion questions:
**Tracksuitchav@proton.me**
