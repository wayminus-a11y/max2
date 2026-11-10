# MAX Security Scope

- No INTERNET permission in the starter manifest.
- No third-party runtime SDK dependencies.
- Android Keystore AES-GCM helper supplied; integration and tests pending.
- Backup disabled by default to avoid accidental cloud/device backup.
- No Accessibility, microphone, contacts, SMS, location, or broad file permissions.
- No claim of complete security: device compromise, malicious OS, rooted-device attacks, physical access, insecure future components, and user-exported files remain risks.
- Before release: dependency/SBOM review, static analysis, exported-component review, APK permission audit, offline network test, encryption tamper test, backup/restore test, and signed release build.
