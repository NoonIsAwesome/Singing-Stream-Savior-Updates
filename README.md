# Singing Stream Savior Updates

This public repository distributes compiled updates for **Singing Stream
Savior**. It does not contain the application's source code.

- `updates/stable.json` is the stable-channel update manifest read by the
  launcher.
- Compiled application and theme updates are published as GitHub Release
  assets.
- Full installation packages are distributed separately through the official
  download page.

## Publishing order

1. Build and validate the launcher, application, and changed themes.
2. Create a GitHub Release and upload all binary assets.
3. Verify every asset URL, byte size, and SHA-256 value.
4. Publish `updates/stable.json` last.

Publishing the manifest last prevents clients from discovering an update
before all referenced files are available.

Copyright © 2026 Noon. All rights reserved.
