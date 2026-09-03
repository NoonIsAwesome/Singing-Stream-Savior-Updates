# Singing Stream Savior Updates

This public repository distributes compiled updates for **Singing Stream
Savior**. It does not contain the application's source code.

Current stable release: **[2.1.0.3](https://github.com/NoonIsAwesome/Singing-Stream-Savior-Updates/releases/tag/v2.1.0.3)**

Official guide and download page: **[Singing Stream Savior Manual](https://noonisawesome.github.io/Singing-Stream-Savior-Manual/)**

- The 2.1.0.3 full installation ZIP includes launcher **1.2.0.1**.
- Existing launchers update the inner application; the application can then
  verify and replace the outer launcher in the background when needed.
- `updates/stable.json` is the stable-channel update manifest read by the
  launcher through `raw.githubusercontent.com`.
- Full installation ZIP files, compiled application updates, and changed theme
  packages are published as GitHub Release assets.
- The official download page links to the appropriate release asset.

## Publishing order

1. Build and validate the launcher, application, and changed themes.
2. Create a GitHub Release and upload all binary assets.
3. Verify every asset URL, byte size, and SHA-256 value.
4. Publish `updates/stable.json` last.

Publishing the manifest last prevents clients from discovering an update
before all referenced files are available.

Copyright © 2026 Noon. All rights reserved.
