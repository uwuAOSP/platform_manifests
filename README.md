# uwuAOSP

1. Initialize

We recommend initializing with the release manifests:

```bash
repo init -u https://github.com/uwuAOSP/platform_vendor_uwu-versions.git -b main --git-lfs
```

Or track our development repositories:

> [!NOTE]
> The development branch may be unstable.

```bash
repo init -u https://github.com/uwuAOSP/platform_manifests.git -b uwu-17.0 --git-lfs
```

2. Sync

```bash
repo sync -c -j$(nproc --all) --force-sync --force-checkout --no-clone-bundle --no-tags --optimized-fetch --prune
```

3. Setup environment

```bash
source build/envsetup.sh
```

```bash
lunch uwu_devicecode-cp2a-userdebug
```

> [!TIP]
> For new device bringup, see the [instructions on our website](https://uwuaosp.uwuniverse.org/docs/bringup-17/).

4. Build an OTA package:

```bash
uni -j＄(nproc) otapackage
```
