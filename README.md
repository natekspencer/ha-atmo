<!-- BEGIN AUTO-GENERATED HEADER -->

[![Release](https://img.shields.io/github/v/release/natekspencer/ha-atmo?style=for-the-badge)](https://github.com/natekspencer/ha-atmo/releases)
[![HACS Badge](https://img.shields.io/badge/HACS-default-41BDF5.svg?style=for-the-badge)](https://github.com/hacs/integration)
[![Buy Me A Coffee/Beer](https://img.shields.io/badge/Buy_Me_A_☕/🍺-F16061?style=for-the-badge&logo=ko-fi&logoColor=white&labelColor=grey)](https://ko-fi.com/natekspencer)
[![Sponsor on GitHub](https://img.shields.io/badge/Sponsor_💜-6f42c1?style=for-the-badge&logo=github&logoColor=white&labelColor=grey)](https://github.com/sponsors/natekspencer)

![Downloads](https://img.shields.io/github/downloads/natekspencer/ha-atmo/total?style=flat-square)
![Latest Downloads](https://img.shields.io/github/downloads/natekspencer/ha-atmo/latest/total?style=flat-square)

<!-- END AUTO-GENERATED HEADER -->

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://brands.home-assistant.io/atmo/dark_logo.png">
  <img alt="atmo logo" src="https://brands.home-assistant.io/atmo/logo.png">
</picture>

# Atmo for Home Assistant

Home Assistant integration for Atmotube Pro devices from ATMO.

<!-- BEGIN AUTO-GENERATED INSTALLATION -->

## ⬇️ Installation

### HACS (Recommended)

[![Open your Home Assistant instance and open a repository inside the Home Assistant Community Store.](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=natekspencer&repository=ha-atmo&category=integration)

This integration is available in the default [HACS](https://hacs.xyz/) repository.

1. Use the **My Home Assistant** badge above, or from within Home Assistant, click on **HACS**
2. Search for `Atmo` and click on the appropriate repository
3. Click **DOWNLOAD**
4. Restart Home Assistant

### Manual

If you prefer manual installation:

1. Download or clone this repository
2. Copy the `custom_components/atmo` folder to your Home Assistant `custom_components` directory
3. Restart Home Assistant

> ⚠️ Manual installation will not provide automatic update notifications. HACS installation is recommended unless you have a specific need.

## ➕ Setup

Once installed, your Atmotube device should be automatically discovered; simply add and confirm it when prompted.

If automatic discovery doesn't work, you can manually add the integration using the My Home Assistant badge below to jump directly to the setup.

[![Open your Home Assistant instance and start setting up a new integration.](https://my.home-assistant.io/badges/config_flow_start.svg)](https://my.home-assistant.io/redirect/config_flow_start/?domain=atmo)

Alternatively:

1. Go to [Settings > Devices & services](https://my.home-assistant.io/redirect/integrations/)
2. In the bottom-right corner, select **Add integration**
3. Type `Atmo` and select the **Atmo** integration
4. Follow the instructions to add the integration to your Home Assistant
<!-- END AUTO-GENERATED INSTALLATION -->

## ⚙️ Options

After this integration is set up, you can, optionally, configure the following:

- **Enable polling** - increases the precision on temperature and PM sensors by polling the Atmo device instead of relying on advertisement data exclusively.

## Entities

| Name                             | Domain | Description                                                                                               |
| -------------------------------- | ------ | --------------------------------------------------------------------------------------------------------- |
| Air Quality Score                | sensor | Composite score representing overall indoor air quality derived from multiple environmental measurements. |
| Battery                          | sensor | Current battery level of the Atmo device, reported as a percentage.                                       |
| Battery Charging                 | sensor | Indicates whether the device battery is currently charging.                                               |
| Humidity                         | sensor | Relative humidity of the surrounding air (%).                                                             |
| PM1                              | sensor | Concentration of particulate matter smaller than 1.0 µm (μg/m³).                                          |
| PM2.5                            | sensor | Concentration of particulate matter smaller than 2.5 µm (μg/m³), commonly associated with health impacts. |
| PM10                             | sensor | Concentration of particulate matter smaller than 10 µm (μg/m³).                                           |
| Pressure                         | sensor | Ambient air pressure measured by the device.                                                              |
| Temperature                      | sensor | Ambient temperature measured by the device.                                                               |
| Volatile Organic Compounds (VOC) | sensor | Estimated concentration of volatile organic compounds in the air (ppb).                                   |

---

<!-- BEGIN AUTO-GENERATED FOOTER -->

## ❤️ Support Me

I maintain this Home Assistant integration in my spare time. If you find it useful, consider supporting development:

- 💜 [Sponsor me on GitHub](https://github.com/sponsors/natekspencer)
- ☕ [Buy me a coffee / beer](https://ko-fi.com/natekspencer)
- 💸 [PayPal (direct support)](https://www.paypal.com/paypalme/natekspencer)
- ⭐ [Star this project](https://github.com/natekspencer/ha-atmo)
- 📦 If you’d like to support in other ways, such as donating hardware for testing, feel free to [reach out to me](https://github.com/natekspencer)

## 📈 Star History

[![Star History Chart](https://api.star-history.com/svg?repos=natekspencer/ha-atmo)](https://www.star-history.com/#natekspencer/ha-atmo)

<!-- END AUTO-GENERATED FOOTER -->
