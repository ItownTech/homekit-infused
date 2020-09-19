# Homekit Infused

## Framework Content
- [Introduction](index.md)
- [Framework Documentation](framework.md)
- [Updates](updates.md)
- [Issues & Questions](issues.md)
- [About Me](about.md)
- [Thanks](thanks.md)

## Addons Content
- [Addons Documentation](addons.md)
- [Addon List](https://github.com/jimz011/homekit-infused/blob/master/docs/addon_list.md)

# About Homekit Infused
Homekit Infused v3.x.x is a templated lovelace setup in YAML mode. The main goal of this project was to make it easy for people to have a nice interface that is similar to Apple's Homekit.

HKI consists out of 2 main components, the Framework (which can be run standalone) and the addons (which requires the framework)
The framework is basically a header that has notification support, some sensors, a greeting, the menu, the footer and 35 empty views that can be filled to your likings.
You can easily run the Framework on its own without the need for any of the addons, you can use any card you find on either the HA docs or on the forums since it is entirely in YAML. This means you can have very wild setups like standard lovelace would, but not needing to worry about the header, notifications and a lot of styling. 

The addons are predefined sets of code that are either plug and play or requires very little user input to make them work. The addons are currently all styled the same way so that the user doesn't need to fiddle with it to get it right and there are many 'addons' that just require a copy/paste. Addons can also be made by anyone that wants to contribute to this project. You don't need to be a custom-card developer since addons in HKI are just blocks of code together creating the illusion of having installed an addon whilst in reality you are just learning to code in YAML with a lot of ease (you can ask avid HKI users on how simple this is!). 

HKI v2, v1 and v0 users, this is nothing like any of those versions. The performance of this project is so much better that none of those versions can be compared to this one. I suggest upgrading very soon, updates are so easy since v3 that you would be stupid not to :D!

Homekit Infused was created as a private project and released to the public as it was requested by many. In the past year the setup has changed quite a bit, not only aesthetically but also codewise. My goal was to make it easier for people to use what I have created without compromising too much on customization that users have made after installing my previous versions of HKI. The setup is still just as 'modular' as it ever was and you will find many improvements over the previous versions if you are an avid user of my setup. New users might find this project very interesting as well, as not only does it give you this wonderful interface, but it will also give you insight on how a bartender (yes that is me) creates code without having any coding knowledge beforehand other than some basic HTML back in the early 2000s.

Oh, and did I mention that your existing dashboard made with the lovelace UI editor will be untouched and will still be available to you? You can continue building/experimenting with your current dashboard whilst having HKI installed. HKI is an independent dashboard that can be set as the default on a per user basis.

### Follow me on YouTube
[Click Here for all the latest updates/videos](https://www.youtube.com/channel/UCYfcLj3IuQ-1mrnqgCk8f0w)

# Disclaimer
Warning:
- I am not responsible for any data loss or defects that are caused by user error.
- Any custom addon used in this project is not made by me.

# Hardware I use personally for this setup
#### Computer
- Intel i5 4690 3,6GHz
- 32GB DDR3 1600MHz RAM
- 4x HDD (2x 3TB, 2x 2TB)
- 2x SSD (1x 120GB, 1x 480GB)

- Hypervisor used: Unraid
- Docker: Yes
- VM's: Windows 10 and Ubuntu 20.04
- Home Assistant: Home Assistant Core running on docker in Unraid

#### Smart Devices
- 6x Philips Hue dimmers (deCONZ controlled)
- 3x IKEA Tradfri remotes (deCONZ controlled)
- 1x Koogeek kh01cn hardware switch (connected through HA with Homekit Controller)
- 7x LED strips (around 30 meters in total) with MagicHome controllers (Flashed with ESPHome, varying from RGB to RGBWC)
- 9x Ikea Tradfri smart switches  (deCONZ controlled)
- 10x Ikea Tradfri bulbs (ranging from normals to color temperature ones)  (deCONZ controlled)
- 4x Philips Hue lights (ranging from filament to color temperature ones)  (deCONZ controlled)
- 3x Sonoff POW R2 (to monitor the washingmachine, dryer and dishwasher)
- 7x Sonoff Basic used as light or device switches (Flashed with ESPHome)
- 2x Sonoffs TH-16 (used to monitor temperature and humidity, but also doubles as a switch)  (Flashed with ESPHome)
- 1x TP-Link HS110 Energy Reading smart switch (to monitor the refrigerator)
- 2x Blitwolf SHP13 Energy Reading smart switch (to monitor the freezer and unraid server)
- 1x Honeywell smoke detector by Xiaomi  (deCONZ controlled)
- 6x Aqara door/window sensors by Xiaomi (3 used on doors, 3 on windows)  (deCONZ controlled)
- 3x Aqara temperature/humidity sensors by Xiaomi  (deCONZ controlled)
- 1x Xiaomi Roborock S55 (Rooted and flashed with Valetudo RE)
- 1x Apple TV 4K
- 1x Nvidia Shield TV Pro (2019)
- 2x Samsung smart TV
- 2x Google Nest mini's
- 1x Google Home mini
- 1x Google Home standard
- 2x Google Nest Hub
- 2x Aqara motion sensor by Xiaomi (deCONZ controlled)
- 3x IKEA Tradfri Motion sensors (deCONZ controlled)
- 1x Xiaofang Camera (rooted and flashed with Dafang Hacks)
- 1x Simple webcam (in motioneye)
- 1x deCONZ stick by Dresden Elektronic
- 1x Xiaomi Mija Gateway (Lumigateway version 3) (I only ever use this as speaker/light, no other devices are attached to this and it is cut off from the internet)
- 1x Xiaomi Aqara Airconditioning Companion (version 3) (I don't have a compatible airco yet, though it does work as a switch and energy reader, not yet in my HA)

There is probably more, but I can't think of it right now XD
