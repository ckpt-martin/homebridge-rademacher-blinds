# homebridge-rademacher-blinds
Homebridge plugin for Rademacher blinds.
Forked from jortgies original version reverted back to the last version that supported the HomePilot version1.
Since this is a simple hack of the original to allow HomePilot 1 support again, the easiest method is to install the original version and just replace the index.js file in your node-modules/homebridge-rademacher-blinds directory.

# Installation
Follow the instruction in [homebridge](https://www.npmjs.com/package/homebridge) for the homebridge server installation.
The plugin is published through [NPM](https://www.npmjs.com/package/homebridge-rademacher-blinds) and should be installed "globally" by typing:
```
npm install -g homebridge-rademacher-blinds
```
Update your config.json file. See config.json in this repository for a sample.
The "inverted" configuration switch can be used to show open shades as closed or closed shades as open. (true per default because 0% in the homepilot means open, whereas 0% in the Home app means closed)

# Configuration

Configuration sample:
```
  "platforms": [
      {
        "platform": "RademacherBlinds",
        "name": "RademacherBlinds",
        "url": "http://192.168.0.1/deviceajax.do",
        "inverted": true
      }
    ]
```
