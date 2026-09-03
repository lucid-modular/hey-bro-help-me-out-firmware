# Firmware

Make sure to install the latest version of the firmware.

## What you need

- A USB cable that carries data (not a charge-only cable)
- The `.uf2` firmware file
- A computer running Windows, macOS, or Linux

## Steps

1. Unplug the module from your rack, or make sure the rack power is turned off.
2. Locate the small white **BOOTSEL** button on the green PCB (the Pi Pico) attached to the back of the module. It's on the top of the Pico, near the USB connector.
3. Plug the USB cable into your computer.
4. Hold down the **BOOTSEL** button.
5. While still holding **BOOTSEL**, plug the USB cable into the Pico.
6. Release **BOOTSEL** after about a second. The Pico now appears on your computer as a USB drive named `RPI-RP2`, just like a memory stick. If it doesn't show up, unplug and repeat steps 3–5; make sure you are holding the button before power is applied.
7. Open the `RPI-RP2` drive and drag (or copy and paste) the `.uf2` file onto it. Only copy one `.uf2` file.
8. The Pico writes the firmware automatically. Within a few seconds the drive will disappear and the board will reboot into the new firmware. This is expected — it is not an error.
9. Unplug the USB cable (without holding **BOOTSEL**).
10. Reinstall the module in your rack or turn on the rack power.

## Tips and troubleshooting

- Never unplug the cable while the file is copying.
- If you don't see the drive at all, try a different cable or USB port — charge-only cables are the most common cause.
