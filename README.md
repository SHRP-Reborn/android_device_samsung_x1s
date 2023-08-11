# SHRP device tree for Samsung S20 aka x1s

## Kernel source 
Available at https://github.com/corsicanu/android_kernel_samsung_universal9830

## How to build
This was tested and it's fully compatible with the [SHRP Manifest](https://github.com/SHRP-Reborn/manifest.git) on the shrp-12.1 branch.
1. Set up the build environment following instructions from [here](https://shrp-reborn.github.io/docs/#/guide)
2. In the root folder of cloned repo you need to clone the device tree:
```bash
git clone -b shrp-12.1 https://github.com/SHRP-Reborn/android_device_samsung_x1s.git device/samsung/x1s
```
3. To build:
```bash
export ALLOW_MISSING_DEPENDENCIES=true && . build/envsetup.sh && lunch twrp_x1s-eng && mka recoveryimage -j$(nproc --all)
```

