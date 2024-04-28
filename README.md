# Integrate input and relay module under Home Assistant

This project contains 4 demo scripts to shows how to connect input and relay module to Home Assistant. It is very simple and fast preparation to work.

## Prerequisites:
- Install add-ons in Home Assistant:
  - File explorer
  - Mosquitto broker (don't forget configure MQTT in 'Devices and Services')
- I use a [SECURECOM UNIO4](https://www.securecom.eu/en/our-products/signaling-and-control-with-mobile-application) module, WiFI or LTE versions
  - Configure WiFi or/and LTE
  - Configure MQTT settings, enter the Home Assistant address and MQTT broker port, like this: ![unio-mqtt](https://github.com/xilard/home-assistant-unio4/assets/25320041/0c79ad91-5d91-4710-9be3-8ae41b216a00)

### 1. This sample `simple_input_relay` demonstrates how to use input and relay module in Home Assistant:
![simple-input-output](https://github.com/xilard/home-assistant-unio4/assets/25320041/15b7b32d-ba3d-42a8-ae05-79b9593d6ee6)

### 2. The following sample `automation-timed-relay` demonstrates the use of relays with hardware timing on the device. You can set how long you activate the relay:
![automation-timed-relay](https://github.com/xilard/home-assistant-unio4/assets/25320041/3ef8c24f-749f-4ea9-ac10-dcfa8bf0ec29)

### 3. Next sample `automation-shutter` is a ***SHUTTER*** mover, this is also a timed relay solution. Room-1 and Room-2 timing is configured in the script.
![automation-shutter](https://github.com/xilard/home-assistant-unio4/assets/25320041/27077f0b-0a80-4105-b81b-b02c0e72256e)

### 4. Last sample `automation-input-to-output` connects input to relay output. When a input is activated the relay also is became activated.
![automation-input-to-output](https://github.com/xilard/home-assistant-unio4/assets/25320041/7e04fe22-a732-4192-a736-c8240f560486)
