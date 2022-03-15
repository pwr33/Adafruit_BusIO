Fork of Adafruit BusIO so that I2Cdevice allows a pointer to an initialised Wire class to be passed in without being reinitialised using Wire.begin() again

Useful for running on an esp-01 module using Wire.begin(0,2) before using any of the adafruit sensor classes that use this interface.

note that I only wanted SGP30 and SHT31 libraries and they are the only ones that I modified to use this.

Thanks for original, as usual with adafruit a bit overkill, and the overkill did not even include the feature I wanted, whereas sparkfun sgp30 library defaults to just passing in the pre initialised wire pointer, they have no sht3 series library.... and I do not beleive in reinventing the wheel, but its like discovering down the road you just used their pentagram shaped wheel LOL and you should have "reinvented" it! $fn=30; LOL

# Adafruit Bus IO Library [![Build Status](https://github.com/adafruit/Adafruit_BusIO/workflows/Arduino%20Library%20CI/badge.svg)](https://github.com/adafruit/Adafruit_BusIO/actions)


This is a helper library to abstract away I2C & SPI transactions and registers

Adafruit invests time and resources providing this open source code, please support Adafruit and open-source hardware by purchasing products from Adafruit!

MIT license, all text above must be included in any redistribution
