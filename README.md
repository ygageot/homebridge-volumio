# "homebridge-volumio" Plugin

With this plugin you can create HomeKit speaker services for Volumio.

## Compatibility notice
Speakers were introduced within the HomeKit protocol in iOS 10. However the Home App from Apple doesn't support
controlling speakers. Even in current iOS 11 support was not added to the Home App. Though most third party 
HomeKit apps (I like the Example of [Eve App](https://itunes.apple.com/app/elgato-eve/id917695792)) are able to control
speakers. I'm guessing that speaker support will be included in the final iOS 11 release build or within the release of
the HomePod.

## Installation
First of all you should already have installed `Homebridge` on your device. Follow the instructions over at the
[HomeBridge Repo](https://github.com/nfarina/homebridge)

To install the `homebridge-volumio` plugin simply run `sudo npm install -g homebridge-volumio`

### Configuration

Here is an example configuration. 
If you have several Volumio equipments, use the `name` parameter.

```
    "accessories": [
        {
            "accessory": "VOLUMIO",
            "name": "Volumio",
        }
    ]
```
