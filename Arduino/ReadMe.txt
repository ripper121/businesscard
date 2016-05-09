avrdude -c dragon_isp -p attiny85 -U lfuse:w:0xF1:m -U hfuse:w:0xD6:m -U efuse:w:0xFE:m
avrdude -c dragon_isp -p attiny85 -U flash:w:bootloader8Mhz.hex:i