# uwuAOSP

1. Initialize


```bash
repo init -u https://github.com/uwuAOSP/platform_manifests.git -b uwu-17.0 --git-lfs
```

2. Sync

```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune
```

3. Build

```bash
source build/envsetup.sh
```

```bash
lunch custom_devicecode-cp2a-userdebug
```

```bash
m uwu
```
