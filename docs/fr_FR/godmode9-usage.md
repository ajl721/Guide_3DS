# GodMode9 Usage

::: info

For information on dumping cartridge or SD card content, see [Dumping Titles and Game Cartridges](dumping-titles-and-game-cartridges).

:::

::: info

Pour de l'aide (en anglais) sur GodMode9 ainsi que sur le scripting, et pour être tenu à jour et informé, rejoignez [le Discord de GodMode9](https://discord.gg/BRcbvtFxX4).

:::

## Lecture requise

GodMode9 is a full access file browser for the Nintendo 3DS console, giving you access to your SD card, the FAT partitions inside your SysNAND and EmuNAND, and basically anything else. Among other functionality, you can copy, delete, rename files, and create folders.

Note that if you have any payload files other than `GodMode9.firm` in the `/luma/payloads/` folder on your SD card, holding (Start) on boot will display a "chainloader menu" where you will have to use the D-Pad and the (A) button to select "GodMode9" for these instructions.

GodMode9 is powerful software that has the capability to modify essentially anything on your console. Though many of these modifications are locked behind a permissions system, and it is impossible to accidentally perform dangerous actions without deliberately unlocking permissions, you should still follow instructions carefully and keep backups just in case.

## Mise à jour de GodMode9

::: info

Some of the instructions below are only applicable to the latest version of GodMode9, and as such you should follow this section to update your copy before continuing. S'il y a déjà des fichiers existants, remplacez-les par les nouveaux fichiers.

:::

### Ce dont vous avez besoin

- La dernière version de [GodMode9](https://github.com/d0k3/GodMode9/releases/latest) (le fichier `.zip` de GodMode9)

### Instructions

1. Éteignez votre console
2. Insérez votre carte SD dans votre ordinateur
3. Copiez le fichier `GodMode9.firm` depuis l'archive GodMode9 `.zip` vers le dossier `/luma/payloads/` sur votre carte SD
4. Copiez le dossier `gm9` depuis l'archive GodMode9 `.zip` vers la racine de votre carte SD
5. Réinsérez votre carte SD dans votre console

::: tip

GodMode9 is now up to date.

:::

## Creating a NAND Backup

1. Appuyez sur et maintenez (Start), et tout en maintenant (Start), allumez votre console. Ceci lancera GodMode9

<!--@include: ./_include/nand-backup.md -->

::: tip

Your NAND backup has been successfully created.

:::

## Restoring a NAND Backup

1. Éteignez votre console
2. Insérez votre carte SD dans votre ordinateur
3. Copy `<date>_<serialnumber>_sysnand_##.bin` from your computer to the `/gm9/out/` folder on your SD card
4. Réinsérez votre carte SD dans votre console
5. Appuyez sur et maintenez (Start), et tout en maintenant (Start), allumez votre console. Ceci lancera GodMode9
6. Appuyez sur (HOME) pour faire apparaître le menu d’action
7. Sélectionnez "Scripts..."
8. Sélectionnez "GM9Megascript"
9. Select "Restore Options"
10. Select "SysNAND Restore (safe)"
11. Select your NAND backup
12. Appuyez sur (A) pour autoriser l'écriture sur votre SysNAND (lvl3), puis entrez la combinaison de boutons donnée
    - This will **not** overwrite your boot9strap installation
    - Ce processus prendra un certain temps
13. Appuyez sur (A) pour continuer
14. Appuyez sur (B) pour revenir au menu principal
15. Select "Exit"
16. Appuyez (A) pour reverrouiller l'autorisation en écriture si vous y êtes invité

::: tip

Your NAND backup has been successfully restored. You can now delete `<date>_<serialnumber>_sysnand_###.bin` from your SD card.

:::

## Injecting any .CIA app into Health & Safety

::: info

Note that it is not possible to inject files into Health & Safety that are larger than it (including games and other large applications)

:::

1. Appuyez sur et maintenez (Start), et tout en maintenant (Start), allumez votre console. Ceci lancera GodMode9
2. Naviguez vers `[0:] SDCARD` -> `cias`
3. Press (A) on your `.cia` to select it
4. Select "CIA image options..."
5. Select "Mount image to drive"
6. Press (A) on the `.app` file
7. Select "NCCH image options"
8. Select "Inject to H&S"
9. Appuyez sur (A) pour autoriser l'écriture sur votre SysNAND (lvl1), puis entrez la combinaison de boutons donnée
10. Appuyez sur (A) pour continuer
11. Appuyez (A) pour reverrouiller l'autorisation en écriture si vous y êtes invité

::: tip

Your desired application has now been injected into Health & Safety.

:::

## Restoring Health & Safety after injecting a .CIA app

::: info

This will only work if the Health & Safety injection was performed by GodMode9 (not Decrypt9 or Hourglass9).

:::

1. Appuyez sur et maintenez (Start), et tout en maintenant (Start), allumez votre console. Ceci lancera GodMode9
2. Appuyez sur (HOME) pour faire apparaître le menu d’action
3. Select "More..."
4. Select "Restore H&S"
5. Appuyez sur (A) pour autoriser l'écriture sur votre SysNAND (lvl1), puis entrez la combinaison de boutons donnée
6. Appuyez (A) pour reverrouiller l'autorisation en écriture si vous y êtes invité

::: tip

Health & Safety has been reverted to normal.

:::

## Format an SD card

::: danger

**Note that this will erase the contents of your SD card!**

:::

1. Appuyez sur et maintenez (Start), et tout en maintenant (Start), allumez votre console. Ceci lancera GodMode9
2. Press (Right Shoulder) + (B) to unmount the current SD card and insert the one you want to format
   - If GodMode9 shows an initialization error when inserting the SD Card to be formatted, it can safely be dismissed

<!--@include: ./_include/format-sd-gm9.md -->

::: tip

Your SD card has successfully been formatted for use with the console.

:::

## Removing an NNID without formatting your console

::: info

This process will only log you out of your NNID. You will still not be able to use the NNID on another console, as the NNID remains linked to the console.

:::

1. Appuyez sur et maintenez (Start), et tout en maintenant (Start), allumez votre console. Ceci lancera GodMode9
2. Appuyez sur (HOME) pour faire apparaître le menu d’action
3. Sélectionnez "Scripts..."
4. Sélectionnez "GM9Megascript"
5. Select "Scripts from Plailect's Guide"
6. Select "Remove NNID"
7. Appuyez sur (A) pour continuer
8. Appuyez sur (A) pour autoriser l'écriture sur votre SysNAND (lvl1), puis entrez la combinaison de boutons donnée
9. Appuyez sur (A) pour continuer
10. Appuyez sur (B) pour revenir au menu principal
11. Select "Exit"
12. Appuyez (A) pour reverrouiller l'autorisation en écriture si vous y êtes invité
13. Appuyez sur (Start) pour redémarrer votre console

::: tip

You have now been logged out of your NNID.

:::
