# Notes

## Software

I am using [RetroPie](http://retropie.org.uk)

## Cabinent

## Controls


### Buttons
Button layout template from slagcoin 
[Sega printed at 96 dpi](https://www.slagcoin.com/joystick/layout/sega2_m.png)

The arcade stick is too close

Mouting pi and hats.
Super glue with nylon off sets is weak

With plywood driling 3/32 hole works well with nylon and brass m2.5 screw offsets

For the button assignments I am using the 
[libretro MAME 2003+ Modern Fightstick layout](https://docs.libretro.com/library/mame2003_plus/#default-retropad-layouts)
![Modern Fightstick](https://docs.libretro.com/image/core/mame2003-plus/fightstick.png)


## Install notes

### Base install with SSH
 * RetroPie 4.7.1
 * Set timezone to US/ Pacific
 * Turn on SSH
 * ssh using default password
 * change passwd
 * `ssh-copy-id pi@retropie`
 
### PicadeHat
 
 * `curl https://get.pimoroni.com/picadehat | bash`
 
### usb controllers
 
  * copy controller configs 
    ```
    scp retropie/configs/all/retroarch/autoconfig/*.cfg \
    pi@retropie:/opt/retropie/configs/all/retroarch/autoconfig/
    ```
  * Ensure the first player is the first USB controller on the minihub 
    and the mini hub is in pi USB 2 which is the upper left.
    * the ethernet port is USB 1.
  * Turn on the joystick select option for retro arch.
    * Not sure if this is needed on fresh installation.

## Open Problem
 
  * No sound  




