# CalyxOS

CalyxOS is an AOSP based OS, built upon many free software projects. Check out the [website](https://calyxos.org/) to learn more about the project.

## Development

The [Building CalyxOS](https://calyxos.org/docs/development/build/) page on our documentation covers in detail about how you can setup the environment and build your own copy of CalyxOS for a supported device.

Contributions to the project are always welcome. Please check out the documentation on [Gerrit Code Review](https://calyxos.org/docs/development/gerrit/) which covers the general setup and workflow.

## Sync
```bash
repo init -u https://github.com/dopaemon/CalyxOS.git -b android14
```

```bash
repo sync -c --force-sync --no-clone-bundle --no-tags -j8
```

## Build
```bash
source build/envsetup.sh
```
```bash
lunch calyx_bluejay-ap1a-userdebug
```
```bash
m -j$(nproc --all) | tee log.txt
```

## Translations

Missing your language?

Help us by translating [CalyxOS on Weblate](https://hosted.weblate.org/projects/calyxos/). We also use translations from LineageOS, for contributing to them check [LineageOS wiki](https://wiki.lineageos.org/how-to/translate).
