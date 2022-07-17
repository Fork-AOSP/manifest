The RadonOS is a simple, clean, beautiful Android based custom ROM that strives to provide a stable and fluid experience, with minimal enhancements and features to bring out the most out of your Android device.

### Build Environment.
**Initializing the manifest.**
```
repo init -u https://github.com/RadonOS/manifest -b twelve
```

**Syncing the source.**

```
repo sync -j$(nproc --all) --force-sync --no-tags --no-clone-bundle --prune --optimized-fetch
```

**Compiling**
```
source build/envsetup.sh
lunch radon_<device>-userdebug
make bacon
```
You need to clone hals separately according to your device.

