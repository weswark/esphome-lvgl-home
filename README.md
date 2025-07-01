Add this code to esphome to install

```
# ESP32-S3-Touch-LCD-7
substitutions:
  name: "office-panel"
  friendly_name: "Office Panel"
  room: "Office"

# Wifi Setup
wifi:
  ssid: !secret wifi_ssid
  password: !secret wifi_password

# Packages
packages:
  setup:
    url: https://github.com/jtenniswood/esphome-lvgl/
    files: [device/esp32-s3-touch-lcd-7.yaml,
            addon/time.yaml,
            addon/backlight.yaml,
            addon/network.yaml,
            assets/fonts.yaml,
            assets/icons.yaml,
            theme/button.yaml,
            office/sensors.yaml,
            office/lvgl.yaml]
    refresh: 1sec
```
