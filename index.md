# Privacy Policy

**Effective Date: May 16, 2026**

This privacy policy applies to the **Noise Alert** app (hereby referred to as "Application") for Android mobile devices that was created by Noise Alert Team (hereby referred to as "Service Provider") as a Free service. This service is intended for use "AS IS".

## Information Collection and Use

The Application is designed with privacy in mind. It does not require registration and does not collect personal information.

### Microphone Access

The Application uses your device's microphone to measure ambient noise levels in real-time. **Important:** Audio data is processed locally on your device and is never recorded, stored, or transmitted to any server.

### Session Data

Noise monitoring sessions are stored locally on your device only. This data is never uploaded or shared. Session data includes:
- Session duration, start and end times
- Minimum, maximum, and average decibel levels
- Peak sound levels — unweighted (Lpeak), A-weighted (LApeak), and C-weighted (LCpeak)
- Noise dose calculations for occupational compliance
- Frequency weighting method used (A-weighting, C-weighting, or Z-weighting)
- Compliance mode settings (EU, OSHA, NIOSH, UK, Australia standards)
- Device model and audio source
- User-defined tags (free-text labels for session identification)
- Location data (if enabled) — latitude, longitude, and location name
- Hearing protection device settings (if enabled) — HPD active state and SNR attenuation value
- Location anonymization state (whether coordinates were stored at full or reduced precision)
- Alert trigger count and threshold snapshots at time of recording
- Audio clipping event count
- Sample count and audio sample rate
- Adaptive sampling tier transitions (internal quality metadata for measurement accuracy)
- Individual timestamped noise readings recorded at each measurement interval, including per-reading decibel levels, alert flags, and peak measurements

### Device and Calibration Data

To ensure measurement accuracy, the Application stores the following device-specific data locally:
- Device model and manufacturer
- Audio sample rate capabilities
- Microphone calibration offset (user-configured or from reference database)
- Calibration method (factory default, reference device, or manual)

This data is used solely for accurate noise level calculations and is never transmitted externally.

### Notifications

On Android 13 and above, the Application requests the notification permission (`POST_NOTIFICATIONS`) to display:
- **Foreground service notification:** Required by Android to keep the noise monitoring service running in the background
- **Threshold alert notifications:** Alerts when noise levels exceed your configured thresholds

You can revoke notification permission at any time in Android Settings. Without it, the app cannot run background monitoring.

### Camera (Flashlight)

The Application can optionally use your device's camera flash (LED) as a visual alert when noise exceeds your threshold. This feature:
- Uses only the camera flash LED — the camera itself is never activated
- No photos or videos are taken
- Must be enabled manually in Settings
- Uses Android's `CameraManager` API for torch control only

### Battery Optimization

To ensure reliable background monitoring, the Application may guide you to disable battery optimization in Android Settings. This prevents the system from stopping noise monitoring during active sessions. You can re-enable battery optimization at any time in **Android Settings → Battery → Battery Optimization**.

## Third-Party Services

The Application uses the following third-party services provided by Google:

### Firebase Crashlytics

To improve app stability, the Application uses Firebase Crashlytics to collect anonymous crash reports. This includes:
- Device type and OS version
- App version
- Crash stack traces

This data is **anonymous** and cannot be used to identify you personally.

### Firebase Analytics

The Application uses Firebase Analytics to collect anonymous usage statistics, including:
- App opens and session duration
- Screen views
- Basic device information (device model, OS version)

This data helps us understand how the app is used and improve user experience. **No personally identifiable information is collected.** Data is processed in accordance with [Google's Privacy Policy](https://policies.google.com/privacy).

### Google AdMob (Free Version Only)

The free version of the Application displays banner and rewarded video advertisements via Google AdMob. AdMob may collect:
- Advertising ID (resettable device identifier)
- Device information (model, OS version)
- Ad interaction data (impressions, clicks)

You can control personalized advertising in your Android device settings:
- **Settings → Google → Ads → Opt out of Ads Personalization**
- You can also reset your Advertising ID at any time

**Note:** The Premium version of the Application contains no advertising and does not use AdMob.

### Ad and Analytics Consent (EU/EEA, UK, Switzerland)

For users located in the European Economic Area, the United Kingdom, and Switzerland, the Application uses **Google's User Messaging Platform (UMP)** — a Google-certified IAB TCF v2.2 Consent Management Platform — to obtain GDPR/DMA-compliant consent **before** any analytics events are sent or any advertising is loaded.

**On first launch in a regulated region**, a Google-rendered consent form appears. The form lets you:
- Grant or deny consent for personalized advertising
- Grant or deny consent for analytics measurement
- Review the list of advertising vendors (currently: Google AdMob)

**The Application's behaviour reflects your choice exactly:**
- **If you grant consent:** Firebase Analytics begins collecting anonymous usage data; AdMob may serve personalized ads
- **If you deny consent:** No analytics events are sent; the banner ad area collapses to zero height; the rewarded-ad option is disabled with an explanation. We **do not** fall back to non-personalized ads — denying means no ads at all (per the Application's "transparency over revenue" principle)
- **If you are outside the regulated region:** The form is not shown; analytics and ads operate as described above
- **If the consent backend is unreachable** (offline launch): The Application proceeds with analytics and ads disabled until consent can be resolved on a later launch (fail-closed behaviour)

**You can change your choice at any time** via the **Privacy options** entry in the navigation drawer's Legal section. This entry is visible only to users in regulated regions.

This Application uses Google's Consent Mode v2 — analytics and ads SDKs receive your consent decision and adjust their behaviour accordingly. See [Google's User Messaging Platform documentation](https://developers.google.com/admob/android/privacy) and [Google's certified CMP overview](https://support.google.com/admanager/answer/13554116) for technical details.

### Google Play Billing

The Application uses Google Play Billing for in-app purchases (one-time lifetime Premium upgrade). When you make a purchase:
- Google processes your payment information directly
- The Application receives only purchase tokens and order IDs to verify your purchase status
- No payment details (credit card numbers, billing address) are ever seen or stored by the Application

Purchase history is managed by Google Play. See [Google Play's Terms of Service](https://play.google.com/about/play-terms/) for details.

### Google Play In-App Review

The Application may prompt you to rate it via Google Play's In-App Review API.
When the review dialog is shown, the Google Play SDK communicates with Google servers
to check review eligibility (e.g., whether you have recently been prompted).
No personal data from the Application is transmitted to Google in this process —
only standard app and device identifiers used by Google Play.
See [Google Play's Terms of Service](https://play.google.com/about/play-terms/) for details.

## Cloud Backup (Optional)

The Application supports Android Auto Backup, which can automatically back up your app data to your personal Google Drive account. This is an **optional** Android system feature.

### What may be backed up:
- App settings and preferences
- Calibration data

**Note:** Session history is stored in an encrypted database (SQLCipher) and is NOT included in cloud backups. Encryption keys are device-specific and cannot be transferred between devices.

### How to control:
- **Disable in app:** Settings → Cloud Backup → Off
- **Disable system-wide:** Android Settings → Google → Backup

When enabled, backup data is encrypted and stored in your personal Google Drive, not on our servers. See [Google's Backup documentation](https://support.google.com/android/answer/2819582) for details.

### Device-to-Device Transfer

When setting up a new Android device, the system may transfer app data from your old device.
The same inclusion/exclusion rules as Cloud Backup apply: app settings and preferences may be transferred,
but the encrypted session database and encryption keys are excluded.

## Data Export

The Application allows you to export your monitoring sessions as PDF reports or CSV data files.

- **Local generation:** All exports are generated entirely on your device — no data is uploaded to any server
- **Sharing:** Exports are shared via Android's standard share sheet (email, messaging apps, cloud storage). Once shared, the data is subject to the recipient's privacy practices
- **Location in exports:** A separate setting ("Include location in exports") controls whether location data appears in exported files. When enabled, both PDF and CSV exports include coordinates as stored at session time — full precision if anonymization was disabled, or approximately 111-meter accuracy if anonymization was enabled during recording
- **Export format:** CSV files use RFC 4180 format with UTF-8 encoding for compatibility with spreadsheet applications
- **Free tier limits:** 3 exports per week. Premium tier: unlimited exports

## Free and Premium Tiers

The Application offers both Free and Premium tiers with different data policies:

### Free Tier
- **Session history retention:** 7 days (older sessions are automatically deleted)
- **Export limits:** 3 exports per week (PDF/CSV)
- **Session duration:** Maximum 2 hours per session

### Premium Tier
- **Session history retention:** Unlimited (data kept until you delete it)
- **Export limits:** Unlimited exports
- **Session duration:** Unlimited

**Note:** Upgrading to Premium restores access to any sessions within the 7-day window that haven't been deleted yet.

## Location Information

The Application offers an **optional** location tagging feature that captures your location when starting a noise monitoring session. This feature requires your **explicit consent** before any location data is collected. A consent dialog is shown the first time you start monitoring with location tagging enabled.

### Three location modes — you choose which Android permission is requested

In line with [Google Play's Location Permissions policy](https://support.google.com/googleplay/android-developer/answer/9799150) (effective April 15, 2026), the Application requests **only the minimum location scope** that matches your in-app choice. The consent dialog and the Settings screen offer three modes, each mapped to a specific Android runtime permission:

| Your choice in the dialog / Settings | Android permission requested | Captured precision |
|--------------------------------------|------------------------------|--------------------|
| **Approximate** (recommended) | `ACCESS_COARSE_LOCATION` | Network/cell-based, approximately 1–3 km |
| **Precise** | `ACCESS_FINE_LOCATION` | GPS, approximately 5 m |
| **Don't share** | None — no permission requested | No coordinates captured |

Both `ACCESS_COARSE_LOCATION` and `ACCESS_FINE_LOCATION` are declared in the Android manifest, but the Application **never requests `ACCESS_FINE_LOCATION` unless you explicitly chose "Precise"**. You can change your choice at any time in **Settings → Save location → Location precision**, and you can revoke the permission entirely from the Android system settings.

### App-level toggle vs Android system permission

Turning **Save location** off in Settings stops the Application from collecting, processing, or storing location immediately and persistently — no future session will record location while the toggle is off. This satisfies the data-minimization (GDPR Art. 5) and right-to-withdraw (GDPR Art. 7(3)) principles by halting *processing*.

Following the Android industry baseline (used by Google Photos, Strava, Komoot, and other location-aware apps), the **system-level permission grant remains in place** until you revoke it through Android Settings. The in-app toggle controls whether the Application *uses* the permission; the OS controls whether the grant *exists*. To make this distinction visible, the Settings screen shows a transparency hint with an "Open Settings" shortcut whenever the toggle is off but Android still has the location permission granted.

To fully revoke the OS-level grant, navigate to **Android Settings → Apps → Noise Alert → Permissions → Location → Don't allow**, or tap the in-app shortcut. The Application does not auto-revoke its own permission via `Context.revokeSelfPermissionsOnKill` because that API requires the app process to be killed (which looks like a crash to the user) and is unavailable on Android 12 and below; stopping processing is a non-disruptive, equally-protective alternative.

### How location data works:
- **Opt-in only:** Location tagging is disabled by default. You must enable it in Settings and grant the matching Android permission. An additional in-app consent dialog is shown before any location data is collected
- **Per-session capture:** Location is recorded **once** at session start using the device's last known location — there is no continuous or background tracking
- **Additional anonymization for Precise mode:** When you choose Precise, the captured GPS coordinates are stored as received from the system. When you choose Approximate, the system itself returns a coarse fix; the Application also rounds the result to approximately 111-meter accuracy as a defense-in-depth measure
- **On-device processing:** Reverse geocoding (converting coordinates to a human-readable location name) uses Android's built-in Geocoder API. On most devices with Google Play Services, this may involve a request to Google's geocoding service. Only the session-start coordinates are sent — no audio, noise measurements, or other app data is transmitted in this process
- **Local storage only:** Location data is stored exclusively on your device in an encrypted database — it is never transmitted to any server
- **Export control:** A separate setting controls whether location data is included in PDF/CSV exports. Exports include coordinates at the precision they were captured. A "Location Privacy" label in each export indicates the precision level
- **No background tracking:** The Application never accesses your location in the background or between sessions

You can disable location tagging at any time in Settings. Previously captured location data is deleted when the associated session is deleted.

## Third-Party Data Sharing

The Application does not collect or share personal information. Anonymous data collected by third-party services (Firebase Crashlytics, Firebase Analytics, AdMob, Google Play Billing, Google Play In-App Review, Google User Messaging Platform) is processed by Google in accordance with [Google's Privacy Policy](https://policies.google.com/privacy). For users in the EU/EEA, UK, and Switzerland, data flow to Firebase Analytics and AdMob is gated by your consent choice as described in **Ad and Analytics Consent** above.

## Data Retention

### Local Data
- **Session data (Free tier):** Automatically deleted after 7 days
- **Session data (Premium tier):** Stored until you delete it or uninstall the app
- **Deleted sessions:** Kept as "soft delete" tombstones for 30 days to support undo functionality, then permanently removed
- **App settings and calibration:** Stored until you uninstall the app or clear app data

### Third-Party Services
- **Crash reports (Firebase Crashlytics):** Retained for 90 days
- **Analytics data (Firebase Analytics):** 2 months (default retention period)
- **Advertising data (AdMob):** Subject to Google Ads data retention policies
- **Purchase records (Google Play Billing):** Managed by Google Play

## Opt-Out Rights

You can stop all data collection by the Application by uninstalling it using the standard uninstall process on your Android device.

## Children's Privacy

The Application is not directed to children under the age of 13. We do not knowingly collect personally identifiable information from children. If you are a parent or guardian and believe your child has provided personal information, please contact us at noisealert.dev@gmail.com so we can take appropriate action.

## Security

The Service Provider is committed to protecting your information through multiple layers of security:

- **Local-first design:** All noise measurement data is processed and stored exclusively on your device
- **Database encryption:** Session data is encrypted at rest using SQLCipher (AES-256-CBC with HMAC-SHA512 page-level verification)
- **Hardware-backed key storage:** Encryption keys are protected by the Android Keystore system, utilizing hardware security modules (TEE or StrongBox) when available on your device
- **Settings integrity:** Safety-critical settings (noise thresholds, calibration values) are protected by HMAC-SHA256 integrity verification to detect unauthorized modifications
- **No cleartext traffic:** The Application does not permit unencrypted network connections
- **Code protection:** Release builds use R8 code obfuscation and resource shrinking

Since the Application processes audio locally and does not transmit personal data to our servers, there is minimal risk of unauthorized access to your noise monitoring information.

## Health & Medical Disclaimer

The Application is a noise-awareness and occupational-safety tool. **It is not a medical device.** It does not diagnose, treat, cure, prevent, or monitor any disease or health condition, including hearing loss or other hearing impairments.

Noise measurements, noise-dose calculations, and compliance estimates (EU, OSHA, NIOSH, UK, Australia standards) are provided **for general awareness only**. Consumer smartphone microphones are not calibrated reference instruments, and readings are not a substitute for a professionally calibrated sound level meter or a formal occupational-hygiene assessment. Do not rely on the Application for legal compliance determinations, workplace safety certification, or medical decisions.

If you have concerns about noise exposure or your hearing, consult a qualified healthcare professional (such as an audiologist) or a certified occupational-safety professional.

Noise-exposure and dose data is stored only on your device. It is **never sold, never shared, and never used to make decisions about employment, insurance, or credit.**

## Hearing Safety Disclaimer

The Application provides alert sounds to notify you of high noise levels. By default, alert volume is set to **50%** with a normal maximum of **100%**.

### Override Alert Volume Limiter

The Application includes an optional "Override Alert Volume Limiter" setting that allows alert volumes up to **150%** of normal output. This feature is provided for use cases where default volume is insufficient (e.g., industrial environments with hearing protection).

**⚠️ WARNING:** Enabling this setting can produce alert sounds loud enough to cause **permanent hearing damage**, especially when using headphones or earbuds. By enabling this setting, you acknowledge that:

1. You understand the risk of hearing damage from high-volume audio
2. You will not use high-volume alerts with headphones/earbuds in quiet environments
3. The Service Provider is not liable for any hearing damage resulting from use of this feature
4. Per NIOSH guidelines, exposure to sounds above 85 dB(A) for extended periods can cause hearing loss

Use this feature responsibly and at your own risk.

## Changes to This Privacy Policy

This Privacy Policy may be updated from time to time. We will notify you of any changes by posting the new Privacy Policy on this page and updating the "Effective Date" above. You are advised to review this Privacy Policy periodically for any changes.

## Your Consent

By using the Application, you consent to the processing of your information as described in this Privacy Policy.

## Contact Us

If you have any questions about this Privacy Policy or the Application's privacy practices, please contact us:

**Email:** noisealert.dev@gmail.com

---

*This privacy policy was created with the help of [App Privacy Policy Generator](https://app-privacy-policy-generator.nisrulz.com/)*
