# Fenok Infinite Buying Releases

This public repository is the binary-only distribution channel for Fenok Infinite Buying.
The application source, build system, tests, operator data, and signing private key are not
published here.

## Authenticity

Stable update metadata is signed with Ed25519. A compiled application accepts a package
only after its packaged public key verifies the channel manifest and the downloaded ZIP
matches the signed size and SHA-256 digest.

## Current status

The stable update channel is active. This repository publishes update payloads only;
initial portable installers are delivered directly by the operator and are not hosted
here.

Published contents are intentionally limited to:

- immutable compiled application-update ZIP assets attached to stable releases;
- a canonical stable manifest and its detached signature;
- concise release notes.

An update payload is not a standalone installer. Installed clients download it through
the packaged updater, verify its signature and SHA-256 digest, and activate it as a new
immutable application version while keeping recipient configuration and operating data
outside the updated version slot.

Release asset download counts measure downloads of that update payload. They are not a
unique-user or fresh-install count.
