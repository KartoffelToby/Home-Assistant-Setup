# Home-Assistant-Setup
My personal Home Assistant Setup with deCONZ LIFX and others.

What devices i used so far:

- Euronics Sprit Zigbee Thermostat (deCONZ)
- Xiaomi Aquara Door/Window Sensor (deCONZ) 
- Xiaomi Aquara Multi Sensor       (deCONZ)
- Xiaomi Motion and LUX Sensor     (deCONZ)
- LIFX LED Strip                   (LIFX)
- LIFX Mini Color                  (LIFX)
- LIFX A19 Color                   (LIFX)
- DIY Plant Spot LED               (ESPHome)
- DIY BLE to MQTT                  (BLE)
- VegTrug Plant Sensor             (BLE)
- DIY Led Strip                    (WLED)
- Xiaomi Air Purifier mc2          (HACS)
---

## My Blueprints

### Hue Dimmer Switch - Light Control - deCONZ
[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fraw.githubusercontent.com%2FKartoffelToby%2FHome-Assistant-Setup%2Fmain%2Fblueprints%2Fautomation%2Fhomeassistant%2Fhuedimmersw.yaml)
```
Control lights like LIFX with a Philips Hue Dimmer Switch.

The top "on" button will turn the lights on to the last set brightness
(unless the force brightness is toggled on in the blueprint).

Dim up/down buttons will change the brightness smoothly and can be pressed
and hold until the brightness is satisfactory.

The bottom "off" button will turn the lights off.

Longpress "on" or "off" will turn on hole area of lights.
```
---

### Smart Thermostat - deCONZ
[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fraw.githubusercontent.com%2FKartoffelToby%2FHome-Assistant-Setup%2Fmain%2Fblueprints%2Fautomation%2Fhomeassistant%2Fsmart_thermostat.yaml)
```
The most deCONZ Zigbee TVR have an internal Temperature sensor. The fact that this sensor ist located direct to the radiator will generated false measurements. To fix this this blueprint uses an external temperature sensor and adjust the offset of the Thermostat to match the room temperature, it also will be linkt to an External window sensor group to turn off the heating if a window is open. And also turns off if a specific outside temperature is reached to avoid heating in summer
```
