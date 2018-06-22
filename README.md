# Homebuilt magnetometer using Arduino as a DAQ and LabVIEW control
Various LabVIEW programs I wrote to control a vibrating sample magnetometer that was homebuilt.

The code is broken into the various components.
1. A digital-to-analog converter was used to create analog voltages for controlling a Kepco BOP power supply. I tried an LTC1257 and an MCP4725. I ended up using the MCP4725 because of the I2C control over the SPI. I don't recall why at this point. I used an ADS1115 analog-to-digital converter to read a Hall sensor for a measurement of the applied magnetic field. GPIB communication was used to read a lock-in amplifier for the sample magnetization. The Arduino analog pins were used to measure the temperature of a platinum thermometer.
