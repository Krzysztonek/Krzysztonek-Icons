[![hacs_badge](https://img.shields.io/badge/HACS-Integration-41BDF5.svg)]()
[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]
[![GitHub release (latest by date)](https://img.shields.io/github/v/release/krzysztonek/krzysztonek-icons)](https://github.com/krzysztonek/my-ha-icons/releases)
![GitHub file size in bytes](https://img.shields.io/github/size/krzysztonek/my-ha-icons/krzysztonek-icons.js?label=plugin%20size)
![GitHub last commit](https://img.shields.io/github/last-commit/krzysztonek/my-ha-icons)
[![Man Hours](https://img.shields.io/endpoint?url=https%3A%2F%2Fmh.jessemillar.com%2Fhours%3Frepo%3Dhttps%3A%2F%2Fgithub.com%2Fkrzysztonek%2Fmy-ha-icons.git)](https://jessemillar.com/r/man-hours)

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg


[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

# __Krzysztonek Icons__ for Home Assistant

Additional Home Assistant icon repository, which includes some individual icons for personal use only. This repo also features some custom vectors created specifically by the author, inspired by his own needs, that are not represented by the official HA icon stream.

It wasn't be possible without the amazing work from:
* [Custom Brand Icons](https://github.com/elax46/custom-brand-icons) by @elax46
* [Homeassistant Custom Icons](https://github.com/mathoudebine/homeassistant-custom-icons) by @mathoudebine
* [HASS Hue Icons](https://github.com/arallsopp/hass-hue-icons) by @arallsopp

who did a lot to allow the author to create and share such a repo.



## How to install

### <ins>HACS (Recommended):</ins>
_Krzysztonek Icons_ is a custom repository for [HACS](https://hacs.xyz/). This is the recommended way to install _Krzysztonek Icons_. If you install it via HACS, <ins>you will be notified about new releases or updates</ins>.

To install this repository:

- Open HACS (installation instructions are [here](https://hacs.xyz/docs/installation/installation/));
- Go to "Frontend" section;
- Click vertical three-dots hamburger button from the upper-right corner of your screen and choose "Custom repositories";
- Enter or paste the below URL in the Repository field:
```
https://github.com/Krzysztonek/Krzysztonek-Icons
```
- Choose "Dashboard" as a Type, press 'ADD' button and close the window;
- Now type _Krzysztonek Icons_ in the Search field of the HACS dashboard;
- Click vertical three-dots hamburger button next to the repo you found (on the right), and choose 'DOWNLOAD';
- In the next window click 'DOWNLOAD' again;<br>
  _(This repo will be installed in `/config/www/community/Krzysztonek-Icons` folder on your HA server)_
- Clear cache as prompted;
- Restart Home Assistant once downloaded, and enjoy your additional set of icons.

### <ins>Manual:</ins>
:warning: If you install it manually, you will be notified about <ins>neither new releases nor updates</ins>. :warning:
- Copy `krzysztonek-icons.js` file into `config/www` folder on your HA server.
- Go to Configuration -> Lovelace Dashboards -> Resources -> Add Resource
- set URL as `/local/krzysztonek-icons.js` and Resource Type as `Javascript Module`.
- Add the following to your `configuration.yaml`:
```
frontend:
  extra_module_url:
    - /local/krzysztonek-icons.js
```

- Save, then restart Home Assistant and enjoy your additional set of icons.


## Usage
- In your entity editor, specify an icon name followed by prefix `kris:`. Example: `kris:japanese-lantern`.
- If you set `state_color: true` in your card, you'll see the icon gets colorised based upon the current entity state.

#### Example:

```
title: My Garden
state_color: true
type: entities
entities:
  - entity: light.stone_lantern
    name: My Stone Lantern
    icon: kris:japanese-lantern
```

## What icons are inside

Basically, this repo contains several typical Chinese and Japanese structures being typically found in gardens or natural open spaces in Far Eastern countries.
Some familiar gardening tools are also included.

[//]: # (Start Krzysztonek Icons)

| Icon | Name | Icon | Name 
| :--- | :--- | :--- | :--- |
| ![kris:japanese-lantern-1](https://github.com/Krzysztonek/My-HA-Icons/blob/main/docs/svg/japanese-lantern-1-solid.svg)| kris:japanese-lantern-1 | ![kris:japanese-lantern-2-outline](https://github.com/Krzysztonek/My-HA-Icons/blob/main/docs/svg/japanese-lantern-2-outline.svg)| kris:japanese-lantern-2-outline |


[//]: # (End Krzysztonek Icons)



## Want to contribute?
If you find a bug or would like to contribute new icons, please consider forking this repository and submitting a PR, attaching your own `*.png` or `*.svg`.

__Contributions are always welcome!__ :heart:

## Donate
If you find this repository useful, you are welcome to donate this project.

![Static Badge](https://img.shields.io/badge/revolut.me-revolut?style=plastic&logo=revolut&logoSize=imd&labelColor=dodgerblue&link=https%3A%2F%2Frevolut.me%2Fkrzysztonek)

![Static Badge](https://img.shields.io/badge/PayPal-paypal?style=plastic&logo=paypal&logoSize=imd&label=%20&labelColor=lime&color=dodgerblue&link=https%3A%2F%2Fpaypal.me%2Fkrzysztonek)

[![coffee](https://www.buymeacoffee.com/assets/img/custom_images/black_img.png)](https://www.buymeacoffee.com/Mhdxy7u6JH)

<a href="https://buycoffee.to/krzysztonek" target="_blank"><img src="https://buycoffee.to/img/share-button-primary.png" style="width: 127px; height: 33px" alt="Postaw mi kawę na buycoffee.to"></a>



## Licensing
You are free to use this integration unlimited and free of charge for personal use only, unless you change anything of its content.

[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa] 
