[![hacs_badge](https://img.shields.io/badge/HACS-Integration-41BDF5.svg)](https://github.com/hacs/integration)
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

# My HA Icons

Additional Home Assistant icon repository, which includes some individual icons for personal use only. This repo also features some custom vectors created specifically by the author, inspired by his own needs, that are not represented by the official HA icon stream.

It wasn't be possible without the amazing work from:
* [Custom Brand Icons](https://github.com/elax46/custom-brand-icons) by @elax46
* [Homeassistant Custom Icons](https://github.com/mathoudebine/homeassistant-custom-icons) by @mathoudebine
* [HASS Hue Icons](https://github.com/arallsopp/hass-hue-icons) by @arallsopp

who did a lot to allow the author to create and share such a repo.



## How to install

### HACS (Recommended):
This is the recommended way to install _Krzysztonek Icons_.
_Krzysztonek Icons_ is a custom repository for HACS. To install this repo:

- Open HACS (installation instructions are [here](https://hacs.xyz/docs/installation/installation/)).
- Go to "Frontend" section
- Click button with "+" icon
- Search for **Krzysztonek Icons** and install it.
- Add the following to your `configuration.yaml`:
```
frontend:
  extra_module_url:
    - /hacsfiles/my-ha-icons/krzysztonek-icons.js
```
- Save, then restart Home Assistant.

### Manual:
- Copy `krzysztonek-icons.js` into your `config/www` folder on HA server.
- Go to Configuration -> Lovelace Dashboards -> Resources -> Add Resource
- set URL as `/local/krzysztonek-icons.js` and Resource Type as `Javascript Module`.
- Add the following to your `configuration.yaml`:
```
frontend:
  extra_module_url:
    - /local/krzysztonek-icons.js
```

- Save, then restart Home Assistant.


## Usage
- In your entity editor, specify an icon name followed by prefix `kris:`. Example: `kris:japanese-lantern`.
- If you set `state_color: true` in your card, you'll see the icon gets colorised based upon the current entity state.

### Example:

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

[//]: # (Start Krzysztonek Icons)

| Icon | Name | Icon | Name 
| :--- | :--- | :--- | :--- |
| ![kris:japanese-lantern-1](https://github.com/Krzysztonek/My-HA-Icons/blob/main/docs/svg/japanese-lantern-1-solid.svg)| kris:japanese-lantern-1 | ![kris:japanese-lantern-2-outline](https://github.com/Krzysztonek/My-HA-Icons/blob/main/docs/svg/japanese-lantern-2-outline.svg)| kris:japanese-lantern-2-outline |


[//]: # (End Krzysztonek Icons)


## Licensing
You are free to use this integration unlimited and free of charge for personal use only, unless you change anything of its content.

[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa] 
