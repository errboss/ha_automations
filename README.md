# Home Assistant Automation Blueprints

![Home Assistant](https://img.shields.io/badge/Home%20Assistant-Blueprint-blue)
![MQTT](https://img.shields.io/badge/MQTT-supported-green)
![License](https://img.shields.io/badge/license-MIT-lightgrey)

Collection of practical **Home Assistant automation blueprints** designed to simplify everyday smart home scenarios such as controlling blinds with a rotary knob or automatically turning off an electric kettle.

---

# Available Blueprints

| Blueprint | Description |
|----------|-------------|
| Smart Kettle Auto-Off | Automatically switches off a kettle connected to a smart plug when boiling finishes |
| Smart Knob Blinds Control (Simple) | Control blinds tilt using a Smart Knob dimmer via MQTT |
| Smart Knob Blinds Control (Advanced) | Advanced blinds control with smart toggle logic |

---

# 1. Smart Kettle Auto-Off

Automatically turns off a smart plug connected to an electric kettle based on power consumption and a safety timeout.

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://raw.githubusercontent.com/errboss/ha_automations/main/smart_kettle_auto_off.yaml)

## Features

- Detects kettle start from smart plug state  
- Monitors real power consumption  
- Automatically switches off the plug when boiling finishes  
- Safety timer prevents the kettle from running indefinitely  

## Requirements

- Smart plug (`switch`)
- Power sensor (`sensor`)
- Timer entity (`timer.kettle_timer`)

---

# 2. Smart Knob Blinds Control (Simple)

Control blinds tilt using a Smart Knob dimmer via MQTT.

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://raw.githubusercontent.com/errboss/ha_automations/main/smart_knob_blinds_simple.yaml)

## Features

- Control blind tilt using knob rotation  
- Supports multiple blinds  
- Works with Zigbee2MQTT MQTT events  

---

# 3. Smart Knob Blinds Control (Advanced)

Advanced automation for controlling blinds using a Smart Knob with additional smart logic.

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://raw.githubusercontent.com/errboss/ha_automations/main/smart_knob_blinds_advanced.yaml)

## Features

- Rotation adjusts tilt angle  
- Button press toggles open / close  
- Stops blinds if already moving  
- Smart decision logic based on tilt threshold  