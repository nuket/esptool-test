# esptool-test

Simple script to test a USB-to-serial adapter using esptool.py with different baud rate settings.

```
$ ./esptool-test.sh 

Usage:   ./esptool-test.sh PORT         FLASH_SIZE
Example: ./esptool-test.sh /dev/ttyUSBx 0x100000
```

The script then tries reading the MAC, the flash ID, the chip ID, reading the full flash memory, erasing the flash memory, and writing the flash memory.

The script performs these operations at 115200, 230400, 460800, and 921600 baud, to test the performance.
