# esptool-test

Simple script to test a USB-to-serial adapter using esptool.py 
with different baud rate settings.

```
$ ./esptool-test.sh 

Usage:   ./esptool-test.sh PORT         FLASH_SIZE
Example: ./esptool-test.sh /dev/ttyUSBx 0x100000
```

The script then tries reading the MAC, the flash ID, the chip ID, 
reading the full flash memory, erasing the flash memory, generating
a block of random data, and writing that data to the flash memory.

The script performs these operations at 3000000, 1500000, 921600, 
460800, 230400, and 115200 baud, to test the performance of the 
serial adapter and the SPI flash ROM.
