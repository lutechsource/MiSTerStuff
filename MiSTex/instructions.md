
# RP2040 Firmware Update (This is using the Rev1 baseboard)
- MiSTex has a builtin RP2040
- Solder a wire to both holes in J9 on the baseboard
- Connect a USBC cable to RP2040 port on baseboard
- Plug other end of USBC cable to a PC. 
-- You will want to plug into a USB-C hub, otherwise if plug directly to PC USB port, transfer rate will be many times slower
- Connect other end of USB cable to PC (While still holding the BOOTSEL button)
- Pi Pico is not in Mass Storage mode and will appear as a Mass Storage device on your computer.
- Copy dirtyJtag.uf2 file to Pico's Mass Storage drive on your computer
- The Pico will automatically disconnect itself from the PC after the copying is done. This means the firmware is now updated.



# RP2040 Firmware Update
