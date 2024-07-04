# Blueprints for Bambu HomeAssistant-NodeRed Integration

[More Information](https://www.wolfwithsword.com/bambulab-homeassistant-blueprints/)

## Auto Bentobox Fans

[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2FWolfwithSword%2FBambu-HomeAssistant-Flows%2Fblob%2Fmain%2Ffiles%2Fhomeassistant%2Fblueprints%2Fnodered%2Fbambu_nr_auto_bentobox_fans.yaml)

Automate turning on your bentobox or other air filtration system while a print is active and using a selected set of materials. It will automatically turn off 30 seconds after the print has ended or filament has cleared.

The list of filaments is user-definable for which it will be enabled for, but defaults to ASA, ABS, all CF and GF filaments, all Nylons, etc.

The bentobox or air-filtration system must be available as an entity in home-assistant as either a `switch` or a `fan`.

## Notify on Print Error

[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2FWolfwithSword%2FBambu-HomeAssistant-Flows%2Fblob%2Fmain%2Ffiles%2Fhomeassistant%2Fblueprints%2Fnodered%2Fbambu_nr_notify_print_error.yaml)

Send a notification whenever a print-halting error has occurred with your printer. The notification will include the model and name of the source printer, as well as a full description of the error if it is known.

These errors are *not* the HMS notifications, but rather the top-level error that would result in a notification halting your print, giving a popup on the printer screen and a push notification via Handy app. In other words, this automation can replace this functionality entirely.

Limitation: The descriptions are currently only available in English

The notifications can be sent to any number of the following:
  - HomeAssistant built-in notification centre
  - HomeAssistant Mobile-App push notifications to any number of phones
  - Windows Desktop Push Notifications via [HASS Agent](https://github.com/LAB02-Research/HASS.Agent)
  - Alexa speaker TTS Announcements via [Alexa Media Player](https://github.com/alandtse/alexa_media_player)
  
Additionally, you can setup multiple custom actions with your own configuration if desired.

You can also setup a list of error codes to ignore.
  
## Notify on Print End

[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2FWolfwithSword%2FBambu-HomeAssistant-Flows%2Fblob%2Fmain%2Ffiles%2Fhomeassistant%2Fblueprints%2Fnodered%2Fbambu_nr_notify_print_state.yaml)

Send a notification when a print has finished successfully or failed / was cancelled. Does not notify on pause or pause-by-error (use Notify on Print Error for error notifs)

The notifications can be sent to any number of the following:
  - HomeAssistant built-in notification centre
  - HomeAssistant Mobile-App push notifications to any number of phones
  - Windows Desktop Push Notifications via [HASS Agent](https://github.com/LAB02-Research/HASS.Agent)
  - Alexa speaker TTS Announcements via [Alexa Media Player](https://github.com/alandtse/alexa_media_player)
  
Additionally, you can setup multiple custom actions with your own configuration if desired.
