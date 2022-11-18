### ENS160 Digital Metal-Oxide Multi-Gas Sensor

The ENS160 from ScioSense is a digital multi-gas sensor consisting of four independent heaters and gas sensor elements based on metal oxide (MOX) technology, and a controller. TrueVOC® air quality detection provides outputs such as eCO2, TVOC and AQI in compliance with worldwide IAQ standards.

The ENS160 includes a standard 2-wire digital I<sup>2</sup>C interface (SCL, SDA) or 4-wire digital SPI interface (SCLK, MOSI, MISO, CSn) for communication to the main host processor. For more information, refer to the datasheet linked in the Resources and Going Further.


<div style="text-align: center"><a href="../assets/imgs/20844_SparkFun_Air_Quality_ENS160-Sensor.png"><img src="../assets/imgs/20844_SparkFun_Air_Quality_ENS160-Sensor.png" alt="ENS160 Highlighted"></a></div>

### Qwiic Connectors

Our Qwiic Ecosystem makes sensors pretty much plug and play. There are two Qwiic connectors on either side of the Indoor Air Quality Sensor - ENS160 Sensor board to provide power and I2C connectivity simultaneously.

<div style="text-align: center"><a href="../assets/imgs/20844_SparkFun_Air_Quality_ENS160-QwiicConnectors.png"><img src="../assets/imgs/20844_SparkFun_Air_Quality_ENS160-QwiicConnectors.png" alt="Qwiic Connectors Highlighted"></a></div>

### Power

Ideally, power will be supplied via the Qwiic connectors on either side of the board. Alternatively, power can be supplied through the header along the bottom side of the board labeled `3V3` and `GND`. The ENS160 functions at 1.8V so an on-board regulator 


VDD input range is <b>1.71</b>-<b>1.98V</b>, 
VDDIO input range is <b>1.71</b>-<b>3.6V</b>. 


<div style="text-align: center"><a href="../assets/imgs/20844_SparkFun_Air_Quality_ENS160-GND3V3Pins.png"><img src="../assets/imgs/20844_SparkFun_Air_Quality_ENS160-GND3V3Pins.png" alt="GND and 3V3 Pins Highlighted"></a></div>



### I<sup>2</sup>C Pins

The I<sup>2</sup>C pins break out the functionality of the Qwiic connectors. Depending on your application, you can connect to these pins via the plated through holes for SDA and SCL. 

<div style="text-align: center"><a href="../assets/imgs/20844_SparkFun_Air_Quality_ENS160-SCLSDAPins.png"><img src="../assets/imgs/20844_SparkFun_Air_Quality_ENS160-SCLSDAPins.png" alt="SDA and SCL Pins Highlighted"></a></div>

### ADDR/POCI, Chip Select, and Interrupt Pins

The ADDR/POCI and Chip Select Pins are for use with SPI functionality. The interrupt pin is broken out to use for triggered events.

<div style="text-align: center"><a href="../assets/imgs/20844_SparkFun_Air_Quality_ENS160-ADRCSINTPins.png"><img src="../assets/imgs/20844_SparkFun_Air_Quality_ENS160-ADRCSINTPins.png" alt="ADDR, CS, and INT Pins Highlighted"></a></div>

### Power LED

When power is supplied to the board, this LED will light up. 

<div style="text-align: center"><a href="../assets/imgs/20844_SparkFun_Air_Quality_ENS160-PWRLED.png"><img src="../assets/imgs/20844_SparkFun_Air_Quality_ENS160-PWRLED.png" alt="ADDR, CS, and INT Pins Highlighted"></a></div>

### Jumpers

####I<sup>2</sup>C Jumper

Like our other Qwiic boards, the Indoor Air Quality Sensor comes equipped with pull-up resistors on the clock and data pins. If you are daisy-chaining multiple Qwiic devices, you will want to cut this jumper; if multiple sensors are connected to the bus with the pull-up resistors enabled, the parallel equivalent resistance will create too strong of a pull-up for the bus to operate correctly. As a general rule of thumb, disable all but one pair of pull-up resistors if multiple devices are connected to the bus. To disable the pull up resistors, use an X-acto knife to cut the joint between the two jumper pads highlighted below. 

<div style="text-align: center"><a href="../assets/imgs/20844_SparkFun_Air_Quality_ENS160-I2CJumperUpdated.png"><img src="../assets/imgs/20844_SparkFun_Air_Quality_ENS160-I2CJumperUpdated.png" alt="I2C Jumper Highlighted"></a></div>

####Address Jumper

By default, the 7-bit un-shifted I<sup>2</sup>C address of the board is 0x53. However, by manipulating the jumper on the back of the board, this address can be changed: 

|  VDD | 0x53 (Default) |
|:----:|:--------------:|
|  GND |      0x52      |
| OPEN |    Undefined   |



<div style="text-align: center"><a href="../assets/imgs/20844_SparkFun_Air_Quality_ENS160-ADDRJumperUpdated.png"><img src="../assets/imgs/20844_SparkFun_Air_Quality_ENS160-ADDRJumperUpdated.png" alt="I2C Jumper Highlighted"></a></div>

####LED Jumper

If power consumption is an issue, cutting this jumper will disable the Power LED on the front of the board.

<div style="text-align: center"><a href="../assets/imgs/20844_SparkFun_Air_Quality_ENS160-LEDJumperUpdated.png"><img src="../assets/imgs/20844_SparkFun_Air_Quality_ENS160-LEDJumperUpdated.png" alt="LED Jumper Highlighted"></a></div>




### Board Dimensions

Like most of our standard Qwiic boards, the SparkFun Indoor Air Quality Sensor - ENS160 measures 1 inch by 1 inch.

<div style="text-align: center"><a href="../assets/imgs/20844_SparkFun_Air_Quality_ENS160-BoardOutline.png"><img src="../assets/imgs/20844_SparkFun_Air_Quality_ENS160-BoardOutline.png" alt="Board Dimensions"></a></div>
