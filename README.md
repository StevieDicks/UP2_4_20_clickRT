# UP2_4_20_clickRT

Both `receive.c` and `transfer.c` are created from <https://raw.githubusercontent.com/raspberrypi/linux/rpi-3.10.y/Documentation/spi/spidev_test.c>  

### Usage
- Set current value in `transfer.c` on line 46 `uint16_t value = ...` (this will be changed later)  
  - Current (mA) = `value` / 10  
- Compile with `gcc -o transfer transfer.c` and `gcc -o receive receive.o` (will add Makefile if necessary)  
- Run these programs from root, using `sudo ./transfer` and `sudo ./receive`  
