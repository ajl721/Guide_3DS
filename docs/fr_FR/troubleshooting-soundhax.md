---
head:
  [
    [ 'script', { src: '/assets/js/common.js' } ],
    [
        'script',
        { src: '/assets/js/soundhax-frankenfirm-link.js' }
      ],
    [ 'script', { src: '/assets/js/link-common.js' } ]
  ]
---

# Troubleshooting (Soundhax)

This page offers troubleshooting advice for commonly encountered issues with the "Installing boot9strap (Soundhax)" page, which is used on system versions between 1.0.0 and 11.3.0. If you are unable to solve your issue with the advice on this page, please join [Nintendo Homebrew on Discord](https://discord.gg/MWxPgEp) and describe your issue, including what you have already tried.

## Issues with Soundhax

:::details Red/purple/pink and white screen after running Soundhax

If your console is on system version 9.4.0, 9.5.0, or 9.6.0, you may be encountering a bug with an old version of universal-otherapp. Download the latest version from [here](https://github.com/TuxSH/universal-otherapp/releases/latest).

If your console is not on those firmwares, it likely indicates that you already have custom firmware. You should [check for CFW](checking-for-cfw).

:::

:::details "An error has occurred, forcing the software to close..." (white message box)

There is an issue with your `otherapp.bin` file (it is missing, misplaced, or corrupted). Download the latest release of [universal-otherapp](https://github.com/TuxSH/universal-otherapp/releases/latest) and place it on the root of your SD card.

You may also have the wrong Soundhax file for your console, region and version. Vérifiez que les détails de votre console sont corrects et retéléchargez votre fichier Soundhax à partir d'[ici](http://soundhax.com), puis placez-le à la racine de votre carte SD, en remplaçant celui existant.

If the above doesn't fix your issue, and you are using an Old 3DS / Old 3DS XL / Old 2DS, you may be encountering an issue involving cartridge updates. Take another look at the system version. Si le nombre avant la lettre est de 4 ou moins (par ex. 11.3.0-**4**U), remplacez le fichier Soundhax à la racine de votre carte SD par celui de [here](http://soundhax.686178.xyz/frankenfirm.html?crash).

If none of these fix your issue, join [Nintendo Homebrew on Discord](https://discord.gg/MWxPgEp) for assistance.

:::

:::details "Could not play"

You have the wrong Soundhax file for your console, region and version. Vérifiez que les détails de votre console sont corrects et retéléchargez votre fichier Soundhax à partir d'[ici](http://soundhax.com), puis placez-le à la racine de votre carte SD, en remplaçant celui existant.

If the above doesn't fix your issue, and you are using an Old 3DS / Old 3DS XL / Old 2DS, you may be encountering an issue involving cartridge updates. Take another look at the system version. Si le nombre avant la lettre est de 3 ou moins (par ex. 11.3.0-**0**U), remplacez le fichier Soundhax à la racine de votre carte SD par celui de [here](http://soundhax.686178.xyz/frankenfirm.html?unplayable).

If none of these fix your issue, join [Nintendo Homebrew on Discord](https://discord.gg/MWxPgEp) for assistance.

:::

:::details Failed to mount the SD card!

If this is unsuccessful, try using another SD card.

:::

## Issues with SafeB9SInstaller

<!--@include: ./_include/troubleshooting-sb9si-bin.md -->

<!--@include: ./_include/troubleshooting-sb9si-common.md -->

<!--@include: ./_include/troubleshooting-get-help-common.md -->

---

::: tip

Go back to [Installing boot9strap (Soundhax)](installing-boot9strap-\(soundhax\))

:::

<!--@include: ./_include/troubleshooting-return.md -->
