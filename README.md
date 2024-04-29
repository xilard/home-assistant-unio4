# Integrate input and relay module under Home Assistant

This project contains demo scripts to shows how to connect input and relay module to [Home Assistant](https://www.home-assistant.io/).
It is very simple and fast preparation to work.

<p align="center">
  <img src="https://github.com/xilard/home-assistant-unio4/assets/25320041/bcc3d90b-d4e4-49cb-805d-44d5fae6db6c" />
</p>

## Prerequisites:
- Install add-ons in [Home Assistant](https://www.home-assistant.io/):
  - File explorer
  - Mosquitto broker (don't forget configure MQTT in 'Devices and Services')
- Power on [SECURECOM UNIO4](https://www.securecom.eu/en/our-products/signaling-and-control-with-mobile-application) module, WiFI or LTE versions
  - Configure WiFi or/and LTE: it can be done from a browser with a built-in web setup or a PC configurator with a USB connection
  - Configure MQTT settings, enter the Home Assistant address and MQTT broker port, like this: ![unio-mqtt](https://github.com/xilard/home-assistant-unio4/assets/25320041/0c79ad91-5d91-4710-9be3-8ae41b216a00)

## Projects:
### The `simple_input_and_relay` demonstrates how to use input and relay module in Home Assistant:
<p align="center">
  <img src="https://github.com/xilard/home-assistant-unio4/assets/25320041/46d971a8-5c5f-4e27-a961-bcdf7b3024fb" />
</p>

### The `simple_timed_relay` demonstrates the use of relays with hardware timing on the device. You can set how long you activate the relay:
<p align="center">
  <img src="https://github.com/xilard/home-assistant-unio4/assets/25320041/3ef8c24f-749f-4ea9-ac10-dcfa8bf0ec29" />
</p>

### The `automation_input_to_relay` connects input to relay output. When a input is activated the relay also is became activated:
<p align="center">
  <img src="https://github.com/xilard/home-assistant-unio4/assets/25320041/7e04fe22-a732-4192-a736-c8240f560486" />
</p>

### Next sample `automation_roller_shutter` is a ***ROLLER SHUTTER*** mover, this is also a timed relay solution. Room-1 and Room-2 timing is configured in the script:
<p align="center">
  <img src="https://github.com/xilard/home-assistant-unio4/assets/25320041/27077f0b-0a80-4105-b81b-b02c0e72256e" />
</p>

### Last sample `automation_irrigation_control` demonstrates an ***IRRIGATION control*** solution. The relays are activated consecutively from the specified time until the specified duration:
<p align="center">
  <img src="https://github.com/xilard/home-assistant-unio4/assets/25320041/a89f3659-c2a5-4bec-9ae3-28086b70bb40" />
</p>
