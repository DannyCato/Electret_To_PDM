# Electret To PDM

This is a KiCad project that uses a FAN3852 to convert analog electret microphone data to PDM data. It is mounted on a 2-layer PCB with all the parts on the top layer

Additionally, it has grounded mounting pads and a power good LED to see if the connection is working.

## Usage

To be used where there is no better option to turn analog microphone signals into a digital signal. In my case, a Sigma-Delta ADC was used to convert the PDM data into PCM data so that it could more easily be converted into a WAV File for our data collection.

A 1-4 MHz Clock signal should be provided for the FAN Chip to produce PDM data. 

## Connectors
MOLEX SL 70555 series connectors (4 pin for PDM side and 2 pin for Electret side) are used for this board, but switching them out for something else is not difficult

## Schematic

![Schematic](images/Schematic.png)

## Layout

The back layer is almost entire a Ground Plane aside for the few times where wires need to cross over others.

![Layout Front](images/Layout_Front.png)
