# Privacy Policy

**Effective Date: February 11, 2026**

This privacy policy applies to the **Noise Alert** app (hereby referred to as "Application") for Android mobile devices that was created by Noise Alert Team (hereby referred to as "Service Provider") as a Free service. This service is intended for use "AS IS".

## Information Collection and Use

The Application is designed with privacy in mind. It does not require registration and does not collect personal information.

### Microphone Access

The Application uses your device's microphone to measure ambient noise levels in real-time. **Important:** Audio data is processed locally on your device and is never recorded, stored, or transmitted to any server.

### Session Data

Noise monitoring sessions are stored locally on your device only. This data is never uploaded or shared. Session data includes:
- Session duration, start and end times
- Minimum, maximum, and average decibel levels
- Peak sound levels (LCpeak measurements)
- Noise dose calculations for occupational compliance
- Frequency weighting method used (A-weighting, C-weighting, or Z-weighting)
- Compliance mode settings (EU, OSHA, NIOSH, UK, Australia standards)

### Device and Calibration Data

To ensure measurement accuracy, the Application stores the following device-specific data locally:
- Device model and manufacturer
- Audio sample rate capabilities
- Microphone calibration offset (user-configured or from reference database)
- Calibration method (factory default, reference device, or manual)

This data is used solely for accurate noise level calculations and is never transmitted externally.

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

The free version of the Application displays rewarded advertisements via Google AdMob. AdMob may collect:
- Advertising ID (resettable device identifier)
- Device information (model, OS version)
- Ad interaction data (impressions, clicks)

You can control personalized advertising in your Android device settings:
- **Settings → Google → Ads → Opt out of Ads Personalization**
- You can also reset your Advertising ID at any time

**Note:** The Premium version of the Application contains no advertising and does not use AdMob.

### Google Play Billing

The Application uses Google Play Billing for in-app purchases (Premium subscription). When you make a purchase:
- Google processes your payment information directly
- The Application receives only purchase tokens and order IDs to verify your subscription status
- No payment details (credit card numbers, billing address) are ever seen or stored by the Application

Purchase history is managed by Google Play. See [Google Play's Terms of Service](https://play.google.com/about/play-terms/) for details.

## Cloud Backup (Optional)

The Application supports Android Auto Backup, which can automatically back up your app data to your personal Google Drive account. This is an **optional** Android system feature.

### What may be backed up:
- Session history and statistics
- App settings and preferences
- Calibration data

### How to control:
- **Disable in app:** Settings → Cloud Backup → Off
- **Disable system-wide:** Android Settings → Google → Backup

When enabled, backup data is encrypted and stored in your personal Google Drive, not on our servers. See [Google's Backup documentation](https://support.google.com/android/answer/2819582) for details.

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

This Application does not collect any location information.

## Third-Party Data Sharing

The Application does not collect or share personal information. Anonymous data collected by third-party services (Firebase Crashlytics, Firebase Analytics, AdMob, Google Play Billing) is processed by Google in accordance with [Google's Privacy Policy](https://policies.google.com/privacy).

## Data Retention

### Local Data
- **Session data (Free tier):** Automatically deleted after 7 days
- **Session data (Premium tier):** Stored until you delete it or uninstall the app
- **Deleted sessions:** Kept as "soft delete" tombstones for 30 days to support undo functionality, then permanently removed
- **App settings and calibration:** Stored until you uninstall the app or clear app data

### Third-Party Services
- **Crash reports (Firebase Crashlytics):** Retained for 90 days
- **Advertising data (AdMob):** Subject to Google Ads data retention policies
- **Purchase records (Google Play Billing):** Managed by Google Play

## Opt-Out Rights

You can stop all data collection by the Application by uninstalling it using the standard uninstall process on your Android device.

## Children's Privacy

The Application is not directed to children under the age of 13. We do not knowingly collect personally identifiable information from children. If you are a parent or guardian and believe your child has provided personal information, please contact us at noisealert.dev@gmail.com so we can take appropriate action.

## Security

The Service Provider is committed to protecting your information. Since the Application processes audio locally and does not transmit personal data, there is minimal risk of unauthorized access to your information.

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
