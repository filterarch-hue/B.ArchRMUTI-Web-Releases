# RMUTI B.Arch Studio Portal Releases

Signed OTA packages for the RMUTI B.Arch Studio Portal hosted at `https://www.faca.rmuti.ac.th/arch/th/`.

This public repository contains deployable release artifacts only. Application source code, institutional configuration, Google IDs, OAuth tokens, and API keys are not published here.

## OTA channels

- `stable.json` — production channel
- `beta.json` — preview channel when available

Every versioned GitHub Release contains:

- `rmuti-portal-frontend-<version>.zip` — OTA frontend payload
- `rmuti-portal-frontend-<version>.zip.sig` — detached RSA/SHA-256 signature
- `rmuti-portal-installer-<version>.zip` — File Manager installer and updater

The updater verifies the package SHA-256 and detached signature before staging or changing the live website. The verification key is published as `ota-signing-public.pem`. The private signing key is kept outside GitHub.

## Stable manifest

```text
https://raw.githubusercontent.com/filterarch-hue/B.ArchRMUTI-Web-Releases/main/stable.json
```

Do not add credentials, installation configuration, Google Sheet IDs, Drive folder IDs, or user data to this repository.
