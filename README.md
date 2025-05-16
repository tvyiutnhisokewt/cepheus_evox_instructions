![](https://raw.githubusercontent.com/Evolution-X/manifest/vic/Banner.png)

# Installing Evolution X on Xiaomi Mi 9 (cepheus)

This build uses retrofit dynamic partitioning, and a custom (OrangeFox) recovery image is required for flashing and future updates.

If you're already on the recommended OrangeFox recovery or other recoveries with retrofit metadata support, you can skip this instruction.

tl;dr: [Recovery image](https://raw.githubusercontent.com/tvyiutnhisokewt/cepheus_evox_instructions/refs/heads/main/recovery_ofox_cepheus.img), [Recovery zip](https://sourceforge.net/projects/cepheus/files/recovery/OrangeFox-cepheus-A14RetrofitMetadata-28012024.zip/download)

* [Clean flashing](#clean-flashing)
* [Updating from an older Official Evolution X build](#updating-from-an-older-official-evolution-x-build)
* [Updating from an older Unofficial Evolution X build]()

## Clean flashing

_Users coming from MIUI or other ROMs **MUST** do this to install Evolution X._

1. Hold Power button + Volume down until device reboots. You should see the fastboot logo.

2. Flash the recovery from fastboot:

    `fastboot flash recovery recovery_ofox_cepheus.img`

3. Reboot to recovery: type:

    `fastboot reboot`

    then hold the Volume up button until you see the OrangeFox logo.

4. Go to Wipe, tick on all boxes **EXCEPT** "USB-Storage", then swipe to wipe.

5. Go to Menu > ADB & Sideload > Swipe to Start Sideload. Then sideload the ROM using adb sideload:

    `adb sideload EvolutionX-...-cepheus-...-Official.zip`

6. Reboot System and #KeepEvolving

## Updating from an older Official Evolution X build

1. Hold Power button > Reboot > Recovery

2. While in Recovery, go to Apply update > sideload the OrangeFox recovery zip:

    `adb sideload OrangeFox-cepheus-A14RetrofitMetadata-28012024.zip`

    The device will reboot to recovery itself.

3. Go to Menu > Reboot > System

4. Check for updates, download and apply from the Updater app in Settings.

## Updating from an older Unofficial Evolution X build

1. Hold Power button > Reboot > Recovery

2. While in Recovery, go to Apply update > sideload the OrangeFox recovery zip:

    `adb sideload OrangeFox-cepheus-A14RetrofitMetadata-28012024.zip`

    The device will reboot to recovery itself.

3. Go to Menu > ADB & Sideload > Swipe to Start Sideload. Then sideload the ROM using adb sideload:

    `adb sideload EvolutionX-...-cepheus-...-Official.zip`

4. Reboot System and #KeepEvolving

