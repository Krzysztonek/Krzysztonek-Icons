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



## :gear: How to install

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
:warning: If you install it manually, you won't be notified about <ins>any further releases or updates any longer</ins>. :warning:
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


## 🎮 Usage
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

## 📖 What icons are inside

Basically, this repo contains several typical Chinese and Japanese structures being typically found in gardens or natural open spaces in Far Eastern countries.
Some familiar gardening tools are also included.

[//]: # (Start Krzysztonek Icons)

| Icon | Name | Icon | Name 
| :--- | :--- | :--- | :--- |
| ![kris:japanese-lantern-1](https://github.com/Krzysztonek/My-HA-Icons/blob/main/docs/svg/japanese-lantern-1-solid.svg)| kris:japanese-lantern-1 | ![kris:japanese-lantern-2-outline](https://github.com/Krzysztonek/My-HA-Icons/blob/main/docs/svg/japanese-lantern-2-outline.svg)| kris:japanese-lantern-2-outline |


[//]: # (End Krzysztonek Icons)



## ✍️ Want to contribute?
If you find a bug or would like to contribute new icons, please consider forking this repository and submitting a PR, attaching your own `*.png` or `*.svg`.

__Contributions are always welcome!__ :heart:

## 🙏 Donate
If you find this repository useful, you are warmly welcome to donate this project.

Each single donation counts much! You can choose one of the options below, which suits you much:


<table>
  <tr>
    <th><i><b>Platform</i></b></th>
    <th><i><b>Payment methods</i></b></th>
    <th><i><b>Link</i></b></th>
    <th><i><b>Comments</i></b></th>
  </tr>
  <tr>
    <td><b>Ko-fi</b></td>
    <td>
      <li> PayPal</li>
      <li> Credit card</li>
    </td>
    <td>
      <a href='https://ko-fi.com/krzysztonek' target='_blank'><img height='35px' src='https://storage.ko-fi.com/cdn/kofi6.png?v=6' border='0' alt='Buy Me a Coffee at ko-fi.com' />
    </td>
    <td>
      <li> No fee</li>
      <li> Single or monthly payment</li>
    </td>
  </tr>
  <tr>
    <td><b>buycoffee.to</b></td>
    <td>
      <li> BLIK</li>
      <li> Bank transfer</li>
    </td>
    <td>
      <a href="https://buycoffee.to/krzysztonek" target="_blank"><img src="https://buycoffee.to/btn/buycoffeeto-btn-primary.svg" height="35px" alt="Postaw mi kawę na buycoffee.to"></a>
    </td>
    <td>
      <li> No fee</li>
      <li> Single or monthly payment</li>
    </td>
  </tr>
  <tr>
    <td><b>PayPal</b></td>
    <td>
      <li> PayPal</li>
    </td>
    <td>
      <a href="https://paypal.me/krzysztonek" target="_blank"><img src="https://www.paypalobjects.com/webstatic/mktg/logo/pp_cc_mark_37x23.jpg" border="0" alt="PayPal Logo" height="35px" style="height: auto !important;width: auto !important;"></a>
    </td>
    <td>
      <li> No fee</li>
    </td>
  </tr>
  <tr>
    <td><b>Revolut</b></td>
    <td>
      <li> Revolut</li>
      <li> Credit Card</li>
    </td>
    <td>
      <a href="https://revolut.me/krzysztonek" target="_blank"><img src="https://assets.revolut.com/assets/favicons/favicon-32x32.png" height="32px" alt="Revolut"></a>
    </td>
    <td>
      <li> No fee</li>
    </td>
  </tr>
</table>

[ko_fi_shield]: https://img.shields.io/static/v1.svg?label=%20&message=Ko-Fi&color=F16061&logo=ko-fi&logoColor=white

[ko_fi]: https://ko-fi.com/krzysztonek

[buycoffee_to_shield]: https://shields.io/badge/buycoffee.to-white?style=flat&labelColor=white&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAABhmlDQ1BJQ0MgcHJvZmlsZQAAKJF9kT1Iw1AUhU9TpaIVh1YQcchQnayIijhKFYtgobQVWnUweemP0KQhSXFxFFwLDv4sVh1cnHV1cBUEwR8QVxcnRRcp8b6k0CLGC4/3cd49h/fuA4R6malmxzigapaRisfEbG5FDLzChxB6MIZ+iZl6Ir2QgWd93VM31V2UZ3n3/Vm9St5kgE8knmW6YRGvE09vWjrnfeIwK0kK8TnxqEEXJH7kuuzyG+eiwwLPDBuZ1BxxmFgstrHcxqxkqMRTxBFF1ShfyLqscN7irJarrHlP/sJgXltOc53WEOJYRAJJiJBRxQbKsBClXSPFRIrOYx7+QcefJJdMrg0wcsyjAhWS4wf/g9+zNQuTE25SMAZ0vtj2xzAQ2AUaNdv+PrbtxgngfwautJa/UgdmPkmvtbTIEdC3DVxctzR5D7jcAQaedMmQHMlPSygUgPcz+qYcELoFulfduTXPcfoAZGhWSzfAwSEwUqTsNY93d7XP7d+e5vx+AIahcq//o+yoAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH5wETCy4vFNqLzwAAAVpJREFUOMvd0rFLVXEYxvHPOedKJnKJhrDLuUFREULE7YDCMYj+AydpsCWiaKu29hZxiP4Al4aWwC1EdFI4Q3hqEmkIBI8ZChWXKNLLvS0/Qcza84V3enm/7/s878t/HxGkeTaIGziP+EB918nawu7Dq1d0e1+2J2bepnk2jFEUVVF+qKV51o9neBCaugfge70keoxxUbSWjrQ+4SUyzKZ5NlnDZdzGG7w4DIh+dtZEFntDA98l8S0MYwctNGrYz9WqKJePFLq80g5Sr+EHlnATp+NA+4qLaZ7FfzMrzbMBjGEdq8GrJMZnvAvFC/8wfAwjWMQ8XmMzaW9sdevNRgd3MFhvNpbaG1u/Dk2/hOc4gadVUa7Um425qii/7Z+xH9O4jwW8Cqv24Tru4hyeVEU588cfBMgpPMI9nMFe0BkFzVOYrYqycyQgQJLwTC2cDZCPeF8V5Y7jGb8BUpRicy7OU5MAAAAASUVORK5CYII=


[buy_me_a_coffee_shield]: https://img.shields.io/static/v1.svg?label=%20&message=Buy%20me%20a%20coffee&color=6f4e37&logo=buy%20me%20a%20coffee&logoColor=white

[buy_me_a_coffee]: https://www.buymeacoffee.com/krzysztonek

[paypal_me_shield]: https://img.shields.io/static/v1.svg?label=%20&message=PayPal.Me&logo=paypal

[paypal_me]: https://paypal.me/krzysztonek

[revolut_me_shield]: https://img.shields.io/static/v1.svg?label=%20&message=Revolut&logo=revolut

[revolut_me]: https://revolut.me/krzysztonek

## Licensing
You are free to use this integration unlimited and free of charge for personal use only, unless you change anything of its content.

[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa] 
