# MAX1415

This is arduino code for the MAX1415 ADC Chip. It allows for simply interfacing with that chip.

## Chip/Code setup
``` C
#include <max1415.h> //include the lib

const int ChipSelectPin = 53;
const int DataReadyPin = 2;

max1415 myChip(ChipSelectPin, DataReadyPin); //Setup the max1415 SPI communication
```

## Reading the value
``` C
volt = GetReadingNumber(); //Get reading from CH1. CH2 is not supported yet.
```
