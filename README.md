# M5StX Library for M5Stack, M5StickC+, M5Core2 and your own derivatives

## This fork diffs

* Unified M5Stack-compatible stack for M5Stack, M5Core2, M5Stick and custom devices
* Made to run my own M5ez-based projects on suitable devices
* No full compatibility intended, tested but all native libraries included
* TFT_eSPI updated to 2.3.64 with M5FontCreator support
* Some Cyrillic fonts added 
* Unified backlight, battery charging and power off functions on all devices
* M5Button for M5Core2-like devices with touchscreen
* ezSound instead of Speaker lib


## 1. Get Started

#### Here is the article to get started

*1.For MacOS*

https://docs.m5stack.com/#/en/quick_start/m5core/m5stack_core_get_started_Arduino_MacOS

*2. For Windows*

https://docs.m5stack.com/#/en/quick_start/m5core/m5stack_core_get_started_Arduino_Windows


## 2. Example

https://github.com/m5stack/M5Stack/tree/master/examples

## 3. API Reference

https://github.com/m5stack/M5Stack/blob/master/src/M5StX.h#L19


## 4. H/W Reference

#### Pinout

*There are several kinds of M5Cores, There is [their difference in schematic](https://github.com/m5stack/M5-Schematic/blob/master/Core/hardware_difference_between_cores.md).*

**LCD & TF Card**

*LCD Resolution: 320x240*

<table>
 <tr><td>ESP32 Chip</td><td>GPIO23</td><td>GPIO19</td><td>GPIO18</td><td>GPIO14</td><td>GPIO27</td><td>GPIO33</td><td>GPIO32</td><td>GPIO4</td></tr>
 <tr><td>ILI9341</td><td>MOSI/MISO</td><td>/</td><td>CLK</td><td>CS</td><td>DC</td><td>RST</td><td>BL</td><td> </td></tr>
 <tr><td>TF Card</td><td>MOSI</td><td>MISO</td><td>CLK</td><td> </td><td> </td><td> </td><td> </td><td>CS</td></tr>

</table>

**Button & Speaker**

<table>
 <tr><td>ESP32 Chip</td><td>GPIO39</td><td>GPIO38</td><td>GPIO37</td><td>GPIO25</td></tr>
 <tr><td>Button Pin</td><td>BUTTON A</td><td>BUTTON B</td><td>BUTTON C</td></tr>
 <tr><td>Speaker</td><td> </td><td> </td><td> </td><td>Speaker Pin</td></tr>
</table>

**GROVE A**

<table>
 <tr><td>ESP32 Chip</td><td>GPIO22</td><td>GPIO21</td></tr>
 <tr><td>GROVE A</td><td>SCL</td><td>SDA</td></tr>
</table>


### M-BUS
![image](docs/M-BUS.jpg)


#### Note:

* How to install USB driver for establishing serial port

  https://docs.m5stack.com/#/en/related_documents/establish_serial_connection

* How to upgrade M5Stack Libary

  https://docs.m5stack.com/#/en/related_documents/upgrade_m5stack_lib
