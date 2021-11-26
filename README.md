# Ape Tax 🦍🧮

If you want to run the UI yourself, check the following steps:

## Project setup

```bash
yarn
```

### Compiles and hot-reloads for development

```bash
yarn run dev
```

### Compiles and minifies for production

```bash
yarn build
```

### Lints and fixes files

```bash
yarn lint
```

## Add an experimental experiment

#### With prompt
To add a new vault to the list, you need to run the following command : `node scripts/newVault.js --fast`.  
This will prompt you with several information:  
- What's the name of your vault ? (*ex: Hardrock Farmer*)
- What's the logo for your vault ? (*ex: 🎸👨‍🌾*)
- Which chain ? (*oneOf: Mainnet (1), BSC (56), Polygon (137), Fantom Opera (250), Arbitrum One (42161)*)
- What's the address of your vault ? (*ex: 0x33bd0f9618cf38fea8f7f01e1514ab63b9bde64b*)
- Who is the dev of this vault ? (*ex: emilianobonassi*)

<img width="482" alt="Capture d’écran 2021-08-04 à 00 26 37" src="https://user-images.githubusercontent.com/9974362/128094349-de173732-ec31-4314-9d34-b73221a9099f.png">

#### With arguments
You can add some arguments to the script in order to specify some elements. The missing arguments will be prompted as above.  
Here are the arguments :  
- `name` for the name of your vault (*ex: `node scripts/newVault.js --name="Hardrock Farmer"`*)
- `logo` for the logo of your vault (*ex: `node scripts/newVault.js --logo=🎸👨‍🌾`*)
- `chain` for the chain of your vault. Valid options are 1, 56, 137 or 250. (*ex: `node scripts/newVault.js --chain=1`*)
- `address` for the address of your vault (*ex: `node scripts/newVault.js --address=0x33bd0f9618cf38fea8f7f01e1514ab63b9bde64b`*)
- `dev` for the name of the dev of your vault (*ex: `node scripts/newVault.js --dev=emilianobonassi`*)
- `abi` for the ABI to use for your vault. Valid options are yVaultV2 or LidoVault. (*ex: `node scripts/newVault.js --abi=yVaultV2`*)
- `type` for the type of vault. Valid options are experimental or weird. (*ex: `node scripts/newVault.js --type=experimental`*)
- `status` for the status of this vault. Valid options are new, active, withdraw, stealth or endorsed. (*ex: `node scripts/newVault.js --status=active`*)
- `coingecko` to specify the coingeckoID to use for this want token. (*ex: `node scripts/newVault.js --coingecko=true-usd`*)

All in one :
```
node scripts/newVault.js --name="Hardrock Farmer" --logo=🌾🌾 --chain=1 --address=0xFD0877d9095789cAF24c98F7CCe092fa8E120775 --dev=emilianobonassi --abi=yVaultV2 --type=experimental --status=active --coingecko=true-usd
```

## Use the API 🤖
Please see details in the `API.md` file.