# Privacy Policy

**Last updated: May 21, 2026**

Holger Schueler ("we", "us") built wristrax as a personal music sync tool for Plex. This policy explains what data wristrax handles and how.

## The Short Version

wristrax does not collect or transmit your personal data automatically. The only information we receive is what you choose to send us by email (see "Voluntary correspondence" below). Everything else stays on your device.

## Data Handling

### Plex Authentication

When you sign in to Plex, wristrax receives an authentication token from Plex's servers. This token is stored locally on your device and is only used to communicate with your own Plex Media Server. We never see or have access to your token.

### Music Files

Music files are downloaded from your own Plex server and stored locally on your iPhone and/or Apple Watch. These files never pass through our servers.

### Diagnostic Logging

wristrax includes an optional diagnostic log for troubleshooting. It is:

- **Off by default** in release builds
- **In-memory only** -- logs are not written to disk
- **Never transmitted** -- logs are not sent anywhere automatically
- **User-controlled** -- you can enable, view, export, and clear logs manually from Settings

### In-App Purchases

Purchases are handled entirely by Apple's StoreKit framework. wristrax does not collect, process, or have access to any payment information.

### Network Connections

wristrax only connects to:

- **Your Plex Media Server** -- to browse your library and download music
- **Plex authentication servers** -- to sign in (plex.tv)
- **Apple's App Store servers** -- for in-app purchase validation

No other network connections are made.

### Voluntary correspondence

If you choose to contact us using one of the in-app email actions -- "Get Support", "Send Feedback", "Export Diagnostic Logs", or "Request Beta Access" -- your email app opens with a message prefilled. You decide whether to send it. When you do, we receive:

- Your email address and the message contents.
- For support and feedback emails: optionally a diagnostic log snapshot you can review and edit before sending.
- For beta access requests: an App Transaction ID that lets us verify your lifetime purchase in App Store Connect.

We store these emails in our regular inbox and use them only to reply to you, troubleshoot your issue, or process your beta enrollment. We do not share them with third parties. To request deletion of email correspondence from our records, write to us at the contact address below.

## Third-Party Services

wristrax uses one open-source library ([PlexKit](https://github.com/lcharlick/PlexKit)) for Plex API communication. It does not collect any data.

There are no analytics, crash reporting, advertising, or tracking frameworks in the app.

## Data Storage

All data (authentication tokens, music files, library metadata) is stored locally on your device using Apple's standard frameworks (SwiftData, file system). Nothing is stored on external servers controlled by us.

## Children's Privacy

wristrax does not knowingly collect any personal information from anyone, including children under 13.

## Changes to This Policy

If we update this policy, the changes will be posted here with an updated date. We do not maintain a contact list for proactive notifications -- please check back if you have concerns.

## Contact

If you have questions about this privacy policy, contact us at:

**wristrax@holgerschueler.com**
