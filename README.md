# AgenticManager

Local-first macOS app for reviewing AI coding-tool Skills and Agents, running
bundled offline static checks, and explicitly managing project assignments.

## Download

Download the DMG and SHA256SUMS.txt from [Releases](https://github.com/haiderhamad/AgenticManager/releases).

The initial release is an **experimental, unnotarized Apple Silicon preview**.
It has no Developer ID signature. macOS can warn about an unverified developer
or block opening it. It is not an Apple-verified production release.

## Install

1. Verify the downloaded DMG against SHA256SUMS.txt.
2. Open the DMG and drag AgenticManager.app to Applications.
3. Eject the disk image. Open the installed app only if you trust this source.

The image does not launch or install the app automatically. No global macOS
security setting needs to be disabled by an installer.

## Current scope

- Apple Silicon / arm64 only.
- Current OS qualification: macOS 27.0.1. Intel Macs and other macOS versions
  are not qualified, regardless of the static deployment target.
- The optimized build has static bundle and DMG integrity checks. It has not
  been functionally accepted as a notarized or production-data build.
- Project/library data is stored locally in unencrypted SQLite. Native
  resource changes require explicit review and confirmation in the app.
- Static scanning is not a guarantee that imported resources are safe.

This repository initially hosts distribution metadata and release assets.
Its tags identify those releases, not an attested source-code build commit.
The application was built from a separately verified source-input snapshot;
its source fingerprint and test boundaries are recorded in the release notes.
Only the reviewed app image and checksum are release assets. The source checkout,
project databases and QA logs are not uploaded.

Project license: MIT; the DMG includes LICENSE.txt. Third-party scanner/license
notices are retained inside the application resources.
