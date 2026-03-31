# the claw

## Goals

- Relatively cheap while remaining as large as possible
- Easily moddable

## parts

- Build plate - 500x500mm
  - [Heated base](https://www.amazon.com/dp/B0DLVDGVFF)
  - Got FR4 sheet for build surface from Eagle Circuits
- [filament extruder bits (not hotend)](https://www.aliexpress.us/item/3256806663498456.html)
- hotend: E3D V6?
  - [hotend and heater](https://www.aliexpress.us/item/3256809886017151.html)
  - [bowden tube](https://www.aliexpress.us/item/2251832704009739.html)
- 24V 25A 3+ rail PSU
- [2020 V-slot rails](https://www.amazon.com/European-Standard-Anodized-Aluminum-Extrusion/dp/B099MPZ9K5)
  - Get 10x 1220mm and cut to length, much cheaper.
- [Openbuilds 2020 gantry plate](https://www.aliexpress.us/item/3256808602761907.html)

### mainboard and stuff

- [octopus pro w/ tmc2209](https://biqu.equipment/products/bigtreetech-octopus-pro-v1-0-chip-f446)
  - doesn't cost much more than octopus, and can use pt100, meaning can do up to 485 C if using a PT100/1000 thermistor. also has sensorless homing.
- [btt MINI12864 v2.0](https://biqu.equipment/collections/lcd-screen/products/bigtreetech-mini12864-v2-0-lcd-screen-rgb-backlight-mini-display-supports-marlin-diy-for-skr-3d-printer-part-1)
- [MOSFET for bed](https://www.amazon.com/High-Power-Adjustment-Electronic-Controller-Brightness/dp/B0FMJH3DML) - could do it on the board itself, but should I upgrade, this is far more viable to swap out obviously. And it's also a known, tested design, which is also good when dealing with 350W.

## Expansion board

see [the-claw-expansion-board](https://github.com/askiiart/the-claw-expansion-board)

## Pick and place

see [the-claw-pnp](https://github.com/askiiart/the-claw-pnp)

## Random Notes

easyeda2kicad like this:

```sh
easyeda2kicad --full --lcsc_id=C265342 --output ./easyeda
```
