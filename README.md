[![Release](https://img.shields.io/github/v/release/natekspencer/ha-atmo?style=for-the-badge)](https://github.com/natekspencer/ha-atmo/releases)
[![Buy Me A Coffee/Beer](https://img.shields.io/badge/Buy_Me_A_☕/🍺-F16061?style=for-the-badge&logo=ko-fi&logoColor=white&labelColor=grey)](https://ko-fi.com/natekspencer)
[![HACS Custom](https://img.shields.io/badge/HACS-Custom-41BDF5.svg?style=for-the-badge)](https://github.com/hacs/integration)

![Downloads](https://img.shields.io/github/downloads/natekspencer/ha-atmo/total?style=flat-square)
![Latest Downloads](https://img.shields.io/github/downloads/natekspencer/ha-atmo/latest/total?style=flat-square)

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://brands.home-assistant.io/atmo/dark_logo.png">
  <img alt="atmo logo" src="https://brands.home-assistant.io/atmo/logo.png">
</picture>

# ha-atmo

Home Assistant integration for Atmotube Pro devices from ATMO.

# Installation

There are two main ways to install this custom component within your Home Assistant instance:

1. Using HACS (see https://hacs.xyz/ for installation instructions if you do not already have it installed):

   [![Open your Home Assistant instance and open a repository inside the Home Assistant Community Store.](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=natekspencer&repository=ha-atmo&category=integration)
   1. Use the convenient My Home Assistant link above, or, from within Home Assistant, click on the link to **HACS**
   2. Click on **Integrations**
   3. Click on the vertical ellipsis in the top right and select **Custom repositories**
   4. Enter the URL for this repository in the section that says _Add custom repository URL_ and select **Integration** in the _Category_ dropdown list
   5. Click the **ADD** button
   6. Close the _Custom repositories_ window
   7. You should now be able to see the _Atmo_ card on the HACS Integrations page. Click on **INSTALL** and proceed with the installation instructions.
   8. Restart your Home Assistant instance and then proceed to the _Configuration_ section below.

2. Manual Installation:
   1. Download or clone this repository
   2. Copy the contents of the folder **custom_components/atmo** into the same file structure on your Home Assistant instance
      - An easy way to do this is using the [Samba add-on](https://www.home-assistant.io/getting-started/configuration/#editing-configuration-via-sambawindows-networking), but feel free to do so however you want
   3. Restart your Home Assistant instance and then proceed to the _Configuration_ section below.

While the manual installation above seems like less steps, it's important to note that you will not be able to see updates to this custom component unless you are subscribed to the watch list. You will then have to repeat each step in the process. By using HACS, you'll be able to see that an update is available and easily update the custom component.

# Configuration

[![Open your Home Assistant instance and start setting up a new integration.](https://my.home-assistant.io/badges/config_flow_start.svg)](https://my.home-assistant.io/redirect/config_flow_start/?domain=atmo)

Once installed, your Atmotube device should be automatically discovered and you will just need to add and confirm the device.

There is also config flow for this integration. After installing the custom component, use the convenient My Home Assistant link above to take you directly to the integration.

Alternatively:

1. Go to **Configuration**->**Integrations**
2. Click **+ ADD INTEGRATION** to setup a new integration
3. Search for **Atmo** and click on it
4. You will be guided through the rest of the setup process via the config flow

# Options

After this integration is set up, you can, optionally, configure the following:

- **Enable polling** - increases the precision on temperature and PM sensors by polling the Atmo device instead of relying on advertisement data exclusively.

# Entities

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

## Support Me

I'm not employed by Atmo, and provide this custom component purely for your own enjoyment and home automation needs.

If you run into any issues, feel free to open an issue on GitHub, and I’ll do my best to assist!

If you found this integration useful and want to donate, consider [sponsoring me on GitHub][github-sponsor] or buying me a coffee ☕ (or beer 🍺) by using the link below:

[![Support me on ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)][ko-fi]

[github-sponsor]: https://github.com/sponsors/natekspencer
[ko-fi]: https://ko-fi.com/natekspencer
