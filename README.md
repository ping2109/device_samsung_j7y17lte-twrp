# OrangeFox Recovery Project for the Samsung Galaxy J7 2017

### How to build ###

```bash
# Create dirs
$ mkdir ofox ; cd ofox

# Init repo
$ repo init --depth=1 -u https://gitlab.com/OrangeFox/Manifest.git -b fox_9.0

# Clone j7y17lte repo
$ https://github.com/ping2109/device_samsung_j7y17lte-twrp/ -b fox_9.0 device/samsung/j7y17lte

# Sync
$ repo sync --no-repo-verify -c --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j`nproc`

# Build
$ source build/envsetup.sh ; lunch omni_j7y17lte-eng ; mka recoveryimage
```
## Credits
2020 @Astrako

## Contact
Telegram support group: https://t.me/joinchat/D1Jk_VbieGBXOWZt2y8O7A
