
Direct Digital Synthesizer (DDS) using Vivado HLS
======================================

This readme file contains these sections:

1. OVERVIEW
2. SOFTWARE TOOLS AND SYSTEM REQUIREMENTS
3. DESIGN FILE HIERARCHY
4. INSTALLATION AND OPERATING INSTRUCTIONS
5. OTHER INFORMATION (OPTIONAL)
6. SUPPORT
7. LICENSE
8. CONTRIBUTING
9. Acknowledgements
10. REVISION HISTORY

## 1. OVERVIEW

This example shows the implementation of a DDS using Vivado HLS tool. The initial target device is K7 -1, but the design – described in C++, can be targeted to most of Xilinx FPGAs. 

Specification:
* Frequency resolution: clock rate / 2^32 (ie., 0.07 Hz for 300 MHz clock)
* 120 dB SFDR 
* Clock rate = 400 MHz

## 2. SOFTWARE TOOLS AND SYSTEM REQUIREMENTS

Any Vivado HLS release from 2014.1 to 2016.1


## 3. DESIGN FILE HIERARCHY
```
    CONTRIBUTING.md
    dds.cpp
    dds.h
    ddsfine.txt
    dds_test.cpp
    DDS_v4.pdf
    dds_wrap.cpp
    directives_axi.tcl
    LICENSE.md
    README.md
    run.tcl
```

## 4. INSTALLATION AND OPERATING INSTRUCTIONS

The procedure to build the HLS project is as follows:

TCL file to run HLS tool:
```
vivado_hls run.tcl
```
## 5. OTHER INFORMATION

For more information check here: [Full Documentation][]
[Vivado HLS User Guide][]

## 6. SUPPORT

For questions and to get help on this project or your own projects, visit the [Vivado HLS Forums][]. 

## 7. License
The source for this project is licensed under the [3-Clause BSD License][]

## 8. Contributing code
Please refer to and read the [Contributing][] document for guidelines on how to contribute code to this open source project. The code in the `/master` branch is considered to be stable, and all pull-requests should be made against the `/develop` branch.

## 9. Acknowledgements
The Library is written by developers at [Xilinx](http://www.xilinx.com/) with other contributors listed below:

## 10. REVISION HISTORY

Date		|	Readme Version		|	Revision Description
------------|-----------------------|-------------------------
JAN2014		|	1.0					|	Initial Xilinx release
24MAR2016	|	1.1					|	Verified for 2016.1



[Contributing]: CONTRIBUTING.md 
[3-Clause BSD License]: LICENSE.md
[Full Documentation]: DDS_v4.pdf 
[Vivado HLS Forums]: https://forums.xilinx.com/t5/High-Level-Synthesis-HLS/bd-p/hls 
[Vivado HLS User Guide]: http://www.xilinx.com/support/documentation/sw_manuals/xilinx2015_4/ug902-vivado-high-level-synthesis.pdf