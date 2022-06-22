# tequ-baranidesign-weather-daq
Data acquisition software for Barani Design MeteoTemp and MeteoWind weather sensors.

## Requirements
- Baranidesign MeteoWind
- Baranidesign MeteoTemp
- Raspberry Pi

## Node-Red installation

```
bash <(curl -sL https://raw.githubusercontent.com/node-red/linux-installers/master/deb/update-nodejs-and-nodered)
sudo systemctl enable nodered.service
sudo reboot
node-red admin init
```

## Usage

Open Node-Red interface and install the "node-red-contrib-modbus" module from the menu. Then import the weatherstation.json flow.
