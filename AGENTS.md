# Neon District updater channel

- Publish only an APK produced by a fully successful `Sigma` Android workflow.
- Require the clean runtime boot and all visual/interaction checkpoints to pass, then manually inspect the CI screenshots before publication.
- Verify the extracted APK SHA-256 locally before changing `latest.json`.
- Update `NeonDistrict.apk` and `latest.json` together in one normal Git commit.
- Keep `version_code`, `version_name`, the cache-busted APK URL, checksum, and release notes synchronized.
- Never publish an APK from a failed, cancelled, or unverified workflow run.
