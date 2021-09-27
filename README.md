# Bogged Token List Info
## Overview
The Bogged Token List is a list of tokens with accurate and up-to-date information, powering additional information on the BSC.

[Bogged Charts](https://charts.bogged.finance) uses token logos from this source, alongside a number of other projects.
[Bogged.Finance Trading](https://bogged.finance) uses token logos and information from this source.

There are also third party projects which use this source for more up-to-the minute data.

The repository contains token info from the Binance smart Chain.

## How to add token

Please note that brand new tokens are not accepted,
the projects have to be sound, with information available, and non-minimal circulation

### Requirements
Requirements: 300 holders and 1000 transactions. 

Processing Fee for tokens which link to their BoggedChart on their Telegram (whether that's in their bot, or in the description) and Website: **FREE!**

Normal Processing Fee: **0.5BNB.**


### Quick starter

**Adding an BEP20 token checklist**:
- [ ] Make sure your smartcontract has more than 300 address holders & 1000 transactions, otherwise you will be rejected. Dust attacks do not qualify.
- [ ] Fork the Github repository
- [ ] Create folder with name of token smartcontact address in [_checksum format_](https://developer.trustwallet.com/add_new_asset#checksum_format) `bsc/assets/<token_smartcontract_address>/`.
- [ ] *** MAKE SURE THE FOLDER NAME IS IN CHECKSUM FORMAT *** https://ethsum.netlify.app/
- [ ] Tell your designer that token image must be in PNG format, avoid transparent background, recommended size 256x256px, max. 512x512px, with max file size of 100kB. We use trust wallet's [image rules](https://developer.trustwallet.com/add_new_asset#image-requirements).
- [ ] Upload your logo with file named `logo.png` to previously created folder with smartcontract address, and if you done all correctly your path should look like this. `bsc/assets/0x1234567461d3f8Db7496581774Bd869C83D51c93/logo.png`
- [ ] Create `info.json` file with info about the token/project (we expand on Trustwallet's info.json, see below)
- [ ] Create a pull request to the main repo
- [ ] Pay the 0.5 BNB processing fee to 0x075775b21Fc78FE9F12967715C360279d2Ee2472 which is distributed to BOG Stakers.
- [ ] Tag @LukeBogTools once done with tx confirmation

Please do take a moment to look at an existing project to view how best to integrate into our list.

#### Format
info.json
```
{
    "name": "BOG Token",
    "website": "https://bogtools.io/",
    "telegram": "https://t.me/bogtools",
    "discord": "https://discord.gg/bogtools",
    "twitter": "https://twitter.com/bogtools",
    "description": "Powering DeFi on BSC. The home of Charts, Limit Orders and more for Binance Smart Chain, all powered by the BOG Token.",
    "explorer": "https://bscscan.com/token/0xD7B729ef857Aa773f47D37088A1181bB3fbF0099",
    "type": "BEP20",
    "symbol": "BOG",
    "decimals": 18,
    "slippage": 3,
    "status": "active",
    "id": "0xD7B729ef857Aa773f47D37088A1181bB3fbF0099",
    "vested": [
        "0x1EA4b64A3BA73849ef9f53176EBeAF47D6cC25F4"
    ],
    "audits": [
        "https://github.com/BogTools/Bogged-Token-List/blob/main/audit.pdf"
    ]
}
```

The vested field is for addresses holding tokens that are not currently in circulation, any tokens held in these addresses will be excluded from marketcap calculations. We automatically filter out burn addresses 0x0...1, 0x0...0 and 0x0...dead, you do not need to add these.

The audits field is for any token audits you would like to be displayed on charts.

If neither of these apply to your token you may leave them empty as follows:

```
{
    ...
    "vested": [ ],
    "audits": [ ]
}
```

logo.png 
```recommended size 256x256px, max. 512x512px, with max file size of 100kB.```

in a Folder named after your Smart Contract Address in Checksum format.

## What's next?
* [Advertise on BogCharts](https://a-ads.com/campaigns/new?selected_site_id=529945&selected_source_type=site&partner=1701147)
* [Get a free Telegram Price Bot](https://charts.bogged.finance/promotetelegram)
* [Add your token to the promoted token list on BogCharts and reach 1m people a week!](https://charts.bogged.finance/promote)

## Disclaimer
BogTools allows anyone to submit new assets to this repository. However, this does not mean that we are in partnership with the projects.
BogTools will reject projects that are deemed as scam or fraudulent after careful review.
BogTools reserves the right to reject any project for any reason from listing on this platform.

## Rules
Alerts in JSON are not accepted. Only BogTools is permitted to add alerts to tokens.

## License
Please read License.md for details.
