# Blueprints for HomeAssistant

This is a collection of largely unrelated blueprints I use in HomeAssistant.

## Appliance Job Complete Notificaition

Send notification of the job completion of a Washer/Dryer/etc to
one or more notification services.

## Dimmer Minimum Ignite

Ensures that when a light is turned on to a brightness that is too low to make it actually light up,
that it is temporarily set to a higher value (to get it to turn on) before being lowered back down
to the desired brightness.

For example, if a LED bulb is first turned on to 3%, it often won't light up at all. This automation
will set it to 20% (configurable) for about a second, before dimming it back down to 3%, where it
will stay light at a low level.

## Door Direction

Connects to a door sensor and a motion sensor, allowing setting actions
for when the door is opened after the motion is tripped or not. This is
especially useful for automatically triggering lights based on someone
exiting or entering.
