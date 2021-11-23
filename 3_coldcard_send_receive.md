# Send and Receive Air-Gapped BTC Transaction

`WARNING!!!` First send a small amount i.e. 0.0001 BTC for both receive (deposit transaction) and send (spend transaction). And make sure to test backup recovery before depositing any real money!

### Import ColdCard wallet to Wasabi Wallet
[Download](https://wasabiwallet.io/#download), verify and install Wasabi Wallet.
[Read](https://zksnacks.gitbook.io/wasabidoc/docs/using-wasabi/coldwasabi) Wasabi Wallet docs for details.

ColdCard:
1. Insert `SD card` into ColdCard
2. Power up your ColdCard and unlock it with your PIN.
3. go to `Advanced > MicroSD Card > Export Wallet > Wasabi Wallet`. When asked for account, select account number (default is 0) and confirm the export. This will create new skeleton wallet file `new-wallet.json`.

Wasabi Wallet:
1. Insert `SD card` into laptop
2. Go to `Hardware Wallet tab` and click `Import Coldcard`
3. Select `new-wasabi.json` file from SD card
4. In `Load Wallet tab` select your coldcard wallet and click `Load Wallet`

### Receive your first BTC transaction to your ColdCard wallet
Wasabi Wallet:
1. Select `Receive tab` fill the address label and click `Generate Receive Address`
2. Copy newly generated BTC address and send small amount of BTC (i.e. 0.00001 BTC) to this address from exchange or another wallet provider
3. Wait to receive your BTC transaction. Once transactions is received you can view details of your received transaction in `History tab`

### Send and receive BTC air-gapped
Send and receive PSBT Partially Signed Bitcoin Transaction to your own ColdCard wallet address.

Wasabi Wallet:
1. Select `Receive tab` fill the address label and click `Generate Receive Address`
2. Copy newly generated BTC address
3. Click `Advanced > Build Transaction`
4. Select your last coin you want to spend
5. Paste and verify your BTC address to `Address`
6. Type in your `Amount`
7. Type in your `Fee`
8. Click `Build Transaction`
9. Insert `SD card` into laptop
10. Click `Export Transaction` and save PSBT file to SD Card

ColdCard:
1. Insert `SD card` into ColdCard
2. Power up your ColdCard and unlock it with your PIN.
2. Select `Ready To Sign`
3. ColdCard will recognise that we are consolidating transaction within our own wallet. Verify transaction details and approve the transaction. This will create new signed PSBT file.

Wasabi Wallet:
1. Insert `SD card` into laptop
2. Select `Tools > Transaction Broadcaster`
3. Click `Import Transaction` and select signed PSBT file on the SD card
4. Then click `Broadcast Transaction`