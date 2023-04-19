# Blueprints for HomeAssistant

This is a collection of largely unrelated blueprints I use in HomeAssistant.

## Dimmer Minimum Ignite

[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fgregmac%2FHomeAssistant-Blueprints%2Fblob%2Fmain%2Fdimmer_minimum_ignite_level.yaml)

Ensures that when a light is turned on to a brightness that is too low to make it actually light up,
that it is temporarily set to a higher value (to get it to turn on) before being lowered back down
to the desired brightness.

![image](https://user-images.githubusercontent.com/1216375/226121740-e9fbb6fd-39ef-46cd-9392-138ca55a3d71.png)

For example, if a LED bulb is first turned on to 3%, it often won't light up at all. This automation
will set it to 20% (configurable) for about a second, before dimming it back down to 3%, where it
will stay light at a low level.

## Door Direction

[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fgregmac%2FHomeAssistant-Blueprints%2Fblob%2Fmain%2Fdoor_direction_trigger.yaml)

Connects to a door sensor and a motion sensor, allowing setting actions
for when the door is opened after the motion is tripped or not. This is
especially useful for automatically triggering lights based on someone
exiting or entering.

## Laundry Notification

[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fgregmac%2FHomeAssistant-Blueprints%2Fblob%2Fmain%2Flaundry_notification.yaml)
 
Send notification of the job completion and job remaining time of a Washer and/or Dryer to
one or more notification services.


For example: *"The Dryer is finished. The washer will be finished in 42 minutes."*


Support for:

* Voice notifications (Google Assistant)

* Mobile notifications

* Custom actions
