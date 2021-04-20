# Bogged Token List Info
## Overview
The Bogged Token List is a list of tokens with accurate and up-to-date information, powering additional information on the BSC.

[Bogged Charts](https://charts.bogged.finance) uses token logos from this source, alongside a number of other projects.

The repository contains token info from the Binance smart Chain.

## How to add token

Please note that brand new tokens are not accepted,
the projects have to be sound, with information available, and non-minimal circulation

### Quick starter

**Adding an BEP20 token checklist**:
- [ ] Make sure your smartcontract has more than 3,000 address holders, otherwise you will be rejected
- [ ] Fork the Github repository
- [ ] Create folder with name of token smartcontact address in [_checksum format_](https://developer.trustwallet.com/add_new_asset#checksum_format) `bsc/assets/<token_smartcontract_address>/`.
- [ ] Tell your designer that token image must be in PNG format, avoid transparent background, recommended size 256x256px, max. 512x512px, with max file size of 100kB. We use trust wallet's [image rules](https://developer.trustwallet.com/add_new_asset#image-requirements).
- [ ] Upload your logo with file named `logo.png` to previously created folder with smartcontract address, and if you done all correctly your path should look like this. `bsc/assets/0x1234567461d3f8Db7496581774Bd869C83D51c93/logo.png`
- [ ] Create `info.json` file with info about the token/project (we expand on Trustwallet's info.json, see below)
- [ ] Create a pull request to the main repo
- [ ] Pay the processing fee which is distributed to BOG Stakers.

Please do take a moment to look at an existing project to view how best to integrate into our list.

#### Format
info.json
```
{
    "name": "BOG Token",
    "website": "https://bogtools.io/",
    "telegram": "https://t.me/bogtools",
    "description": "Powering DeFi on BSC. The home of Charts, Limit Orders and more for Binance Smart Chain, all powered by the BOG Token.",
    "explorer": "https://bscscan.com/token/0xD7B729ef857Aa773f47D37088A1181bB3fbF0099",
    "type": "BEP20",
    "symbol": "BOG",
    "decimals": 18,
    "status": "active",
    "id": "0xD7B729ef857Aa773f47D37088A1181bB3fbF0099"
}
```

logo.png 
```recommended size 256x256px, max. 512x512px, with max file size of 100kB.```

in a Folder named after your Smart Contract Address in Checksum format.


## Disclaimer
BogTools allows anyone to submit new assets to this repository. However, this does not mean that we are in partnership with the projects.
BogTools will reject projects that are deemed as scam or fraudulent after careful review.
BogTools reserves the right to reject any project for any reason from listing on this platform.

## License
Please read License.md for details.
