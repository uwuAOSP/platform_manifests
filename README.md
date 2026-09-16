# uwuAOSP

1. Initialize


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

4. Build an OTA package:

```bash
uni -j＄(nproc) otapackage
```
