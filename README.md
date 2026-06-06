# uwuAOSP

## Downloading:

1. Initialize:

```bash
repo init -u https://github.com/uwuAOSP/platform_manifests.git -b uwu-16.2 --git-lfs
```

2. Sync:

```bash
repo sync
```

## Building

1. Setup environment:

```bash
source build/envsetup.sh
```

2. lunch device:
```bash
lunch custom_devicecode-bp4a-user
```

3. Build the package:

```bash
m uwu
```
