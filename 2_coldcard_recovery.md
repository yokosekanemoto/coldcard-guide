# ColdCard Recovery Guide

### Test wallet seed backup recovery
`WARNING!!!` This action will cause you to loose all your funds associated with this wallet. Make sure you have written down 24-word seed on the `coldcard backup card` and on a `metal plate` just in case.

Recover from 24-word seed written on a card and stamped on a metal plate:
1. Login to your ColdCard
2. Delete your seed from ColdCard `Advanced > Danger Zone > Seed Functions > Destroy Seed`.
3. Read the notification text carefully and confirm
4. Login to your ColdCard
5. Select `Import Existing > 24 Words` and add all 24 words from: 
   1. your [coldcard backup card](https://coldcardwallet.com/docs/static/pdf/coldcard-backup-card-v2.png)
   2. your stamped metal plate
6. Verify Master Key Fingerprint by selecting `Advanced > View Identity` or [follow passphrase wallet recovery](#Test-passphrase-wallet-backup-recovery)

Recover from SD card digital backup:
1. Login to your ColdCard
2. Delete your seed from ColdCard `Advanced > Danger Zone > Seed Functions > Destroy Seed`.
3. Read the notification text carefully and confirm
4. Login to your ColdCard
5. Insert `SD card A` with saved digital seed backup
6. Select `Import Existing > Restore Backup`
7. Select `backup.7z` file and select 12 words written on the [microSD backup card](https://coldcardwallet.com/docs/static/pdf/microsd-password-v1.png)
8. Login to your ColdCard
9. Verify Master Key Fingerprint by selecting `Advanced > View Identity` or [follow passphrase wallet recovery](#Test-passphrase-wallet-backup-recovery)

### Test passphrase wallet backup recovery

Recover from passphrase written on a card and stamped on a metal plate:
1. Login to your ColdCard
2. Select `Passphrase > OK`
3. `Add Word` Add all passphrase words from:
   1. your [passphrase backup card](https://coldcardwallet.com/docs/static/pdf/recovery-card-v1.png)
   2. your stamped metal plate
4. Select `APPLY`
5. Verify that the Master Key Fingerprint on [passphrase backup card](https://coldcardwallet.com/docs/static/pdf/recovery-card-v1.png) and the one on your ColdCard match.

Recover from SD card backup:
1. Login to your ColdCard
2. Insert `SD card B` with saved passphrase
3. Select `Passphrase > OK > Restore Saved`
4. Verify that the Master Key Fingerprint on [passphrase backup card](https://coldcardwallet.com/docs/static/pdf/recovery-card-v1.png) and the one on your ColdCard match.
