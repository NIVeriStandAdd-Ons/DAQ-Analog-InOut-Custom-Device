# DAQ-Analog-InOut-Custom-Device
To measure or generating analog signals, multiplexed cards will switch through all added channels, so the more channels that are added, the longer it will take to read through all the channels.
In hardware-timed single-point mode, DAQ is inline and guaranteed to get a sample every iteration. The acquisition or generation rates are determined by the PCL rate. If the PCL rate is 1000 Hz, the aquisition or generation will hanppen every 1ms. If too many AI and AO channels are added, lots of HP Loop Duration will be occupied by AI and AO tasks. The actual PCL rate will be impacted. This custom device is developed with inline-async type. It will observably decrease the HP Loop duration.


### LabVIEW Version ###

LabVIEW 2021 64-bit

### Built Availability ###

This IP is built and available for NI VeriStand 2021 and later.

### Quality, Limitations ###

This code is medium quality and not mature. Use at your own risk. It is developed in LabVIEW 2021 64-bit.


### Dependencies ###

NI-DAQmx

### License ###

*This repository and any materials provided by NI therein are provided AS IS. NI DISCLAIMS ANY AND ALL LIABILITIES FOR AND MAKES NO WARRANTIES, EITHER EXPRESS OR IMPLIED, INCLUDING WITHOUT LIMITATION ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR  PARTICULAR PURPOSE, OR NON-INFRINGEMENT OF INTELLECTUAL PROPERTY. NI shall have no liability for any direct, indirect, incidental, punitive, special, or consequential damages for your use of the repository or any materials contained therein.*
