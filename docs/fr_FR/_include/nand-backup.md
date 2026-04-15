1. Appuyez sur (HOME) pour faire apparaître le menu d’action
2. Sélectionnez "Scripts..."
3. Sélectionnez "GM9Megascript"
4. Sélectionnez "Backup Options"
5. Sélectionnez "SysNAND Backup"
6. Appuyez sur (A) pour confirmer
   - Ce processus prendra un certain temps
   - If you get an error, look for your issue in the [troubleshooting guide](troubleshooting-finalizing-setup.html)
7. Appuyez sur (A) pour continuer
8. Appuyez sur (B) pour revenir au menu principal
9. Select "Exit"
10. Appuyez (A) pour reverrouiller l'autorisation en écriture si vous y êtes invité
11. Naviguez vers `[S:] SYSNAND VIRTUAL`
12. Press (A) on `essential.exefs` to select it
13. Sélectionnez "Copy to 0:/gm9/out"
    - If you see "Destination already exists", press (A) on "Overwrite file(s)"
14. Appuyez sur (A) pour continuer
15. Maintenez (R) appuyé et appuyez sur (Start) en même temps pour éteindre votre console
16. Insérez votre carte SD dans votre ordinateur
17. Copy `<date>_<serialnumber>_sysnand_##.bin`, `<date>_<serialnumber>_sysnand_##.bin.sha`, and `essential.exefs` from the `/gm9/out/` folder on your SD card to a safe location on your computer
    - Copy these backups to multiple locations (such as online file storage, an external hard drive, etc.)
    - These backups will save you from a brick and/or help you recover files from the NAND image if anything goes wrong in the future
18. Delete `<date>_<serialnumber>_sysnand_##.bin` and `<date>_<serialnumber>_sysnand_##.bin.sha` from the `/gm9/out/` folder on your SD card after copying it
    - The other backup files are negligible in size and may be kept on your SD card for ease of access
19. Réinsérez votre carte SD dans votre console
