# Tiva C

A ready-made repository for writing, compiling and flashing code for the TI Tiva C.

Tested on Mac OS X 10.6.8, should work on most Macs and Linuxes.

## Requirements

 - [ARM EABI Toolchain Builder](https://github.com/jsnyder/arm-eabi-toolchain)
 - [lm4tools](https://github.com/utzig/lm4tools)
 - TI Tiva C TM4C123x or TM4C129x series dev board


## Usage

If you have the [energia enviroment](http://energia.nu/download/):

```bash
$ export ENERGIA_ROOT=/path/to/energia
$ cd boards/ek-tm4c123gxl/blinky
$ $ENERGIA_ROOT/hardware/tools/lm4f/bin/lm4flash
```

Assuming you're using the Tiva C Connected Launchpad dev board (`ek-tm4c1294xl`):

```bash
$ cd boards/ek-tm4c1294xl/blinky
$ make
$ lm4flash gcc/blinky.bin
# Great success!
```
