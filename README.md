# tequ-baranidesign-weather-daq
Data acquisition software for Barani Design MeteoTemp and MeteoWind weather sensors.

## Requirements
- Baranidesign MeteoWind
- Baranidesign MeteoTemp
- Raspberry Pi
- [USB to RS485 Adapter](https://www.dfrobot.com/product-1029.html)

## Connections

### Adapter wiring
The supplied cable should have 4 wires coming out of one side, these are to be connected to the USB to RS485 Adapter.

| Adapter PIN | Wire Color |
| ----------- | ---------- |
| B485A | Green |
| B485B | Yellow |
| GND | White |
| 5V | VCC |

Yes, white is ground.
After that, just connect the other side of the supplied cable to the sensor and the adapter to you device's USB port.

### Raspberry PI users
If you are using a Raspberry PI, you'll need to enable serial with `sudo raspi-config`




## Node-Red installation

```
bash <(curl -sL https://raw.githubusercontent.com/node-red/linux-installers/master/deb/update-nodejs-and-nodered)
sudo systemctl enable nodered.service
sudo reboot
node-red admin init
```

## Usage

Open Node-Red interface and install the "node-red-contrib-modbus" module from the menu. Then import the weatherstation.json flow.
