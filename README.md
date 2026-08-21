# ČITTAM Capture Lab — releases

Signed Android APKs for **ČITTAM Capture Lab**, a small companion app for
[ČITTAM Linkbook](https://linkbook.cittam.com): share links from any Android
app into an inbox on your phone, then hand the batch to Linkbook in one tap.

This repository contains release artifacts only — no source code.

## Download

Latest release, permanent URL:

`https://github.com/cittam/cittam-capture-lab-releases/releases/latest/download/cittam-capture-lab.apk`

Requires Android 8.0 or newer (minSdk 26). Android will ask you to allow your
browser to install unknown apps — a one-time setting for any app installed
outside a store.

## What each release publishes

- `cittam-capture-lab.apk` — the signed APK; the asset name is stable across
  releases, so the latest-release URL above never changes
- The SHA-256 checksum of that APK
- The `aapt2 dump permissions` output of that exact signed APK — the app
  declares no Android permissions, not even INTERNET, and every release
  publishes this proof

## Verify a download

```
shasum -a 256 cittam-capture-lab.apk
```

Compare the value with the checksum in the release notes for the same version.
