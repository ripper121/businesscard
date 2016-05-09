//D5= 2.7V, D6 = 1.8V, D7=0V
avrdude -c dragon_isp -p attiny85 -U lfuse:w:0xF1:m -U hfuse:w:0xD6:m -U efuse:w:0xFE:m
avrdude -c dragon_isp -p attiny85 -U flash:w:bootloader8Mhz.hex:i

avrdude -c dragon_isp -p attiny85 -U lfuse:w:0xF1:m -U hfuse:w:0xD5:m -U efuse:w:0x06:m
avrdude -c dragon_isp -p attiny85 -U flash:w:trinketgemma_v1.hex:i