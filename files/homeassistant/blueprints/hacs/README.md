# Blueprints for HA-Bambulab HACs Integration 
[More Information](https://www.wolfwithsword.com/bambulab-homeassistant-blueprints/)

## Auto Bentobox Fans (HACs Version)

[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2FWolfwithSword%2FBambu-HomeAssistant-Flows%2Fblob%2Fmain%2Ffiles%2Fhomeassistant%2Fblueprints%2Fhacs%2Fbambu_nr_auto_bentobox_fans_hacs.yaml)

Automate turning on your bentobox or other air filtration system while a print is active and using a selected set of materials. It will automatically turn off 30 seconds after the print has ended or filament has cleared.

The list of filaments is user-definable for which it will be enabled for, but defaults to ASA, ABS, all CF and GF filaments, all Nylons, etc.

The bentobox or air-filtration system must be available as an entity in home-assistant as either a `switch` or a `fan`.

Note: This may currently only work for English translated versions. I am unable to test currently for state values where it is translated. You may need to convert/take control of the blueprint as an automation in HA and modify the values accordingly.