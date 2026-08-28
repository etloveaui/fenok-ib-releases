# Fenok Infinite Buying Releases

This public repository is the binary-only distribution channel for Fenok Infinite Buying.
The application source, build system, tests, operator data, and signing private key are not
published here.

## Authenticity

Stable update metadata is signed with Ed25519. A compiled application accepts a package
only after its packaged public key verifies the channel manifest and the downloaded ZIP
matches the signed size and SHA-256 digest.

## Current status

The channel is being prepared. There is no stable manifest, release tag, or downloadable
application yet. The first release will appear only after the native Windows build,
privacy validation, self-check, signing, upload, and remote read-back gates pass.

Published contents are intentionally limited to:

- immutable compiled ZIP assets attached to versioned releases;
- a canonical stable manifest and its detached signature;
- concise recipient-facing release notes.
