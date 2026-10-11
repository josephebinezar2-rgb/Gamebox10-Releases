# Public release checklist

The app is not publicly downloadable yet. The existing GitHub Actions artifact is a **debug APK**, not a production release.

## Before publishing an APK

- [ ] Generate a dedicated **release signing keystore** and back it up securely. Never commit the keystore or passwords to GitHub.
- [ ] Build a release APK signed with the same key intended for future updates.
- [ ] Confirm the production AdMob configuration and compliance with AdMob's app readiness and ad-serving policies. Do not represent unapproved ad serving as guaranteed revenue.
- [ ] Verify app name, package ID `com.gamebox.ten`, version, and device compatibility.
- [ ] Test the **signed release build** on a real Android phone (games, photo saving, credits, ad availability).
- [ ] Review privacy policy, add a private contact method, and implement consent controls where legally required.
- [ ] Attach the signed APK to a GitHub Release with checksum, version number, and release notes.
- [ ] Add a verified voluntary support/donation URL only after confirming the payment provider's eligibility and terms.

## Donation and monetization

GitHub Releases allows free distribution but **does not make GitHub an AdMob-supported app store**. Donations are voluntary; no payment should be required to play the free app.

## Versioning

Use a stable version name and increment Android `versionCode` for every update. Keep the signing key unchanged for compatible upgrades.
