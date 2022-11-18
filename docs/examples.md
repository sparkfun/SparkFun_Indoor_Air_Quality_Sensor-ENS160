=== "Example 1: Basic Readings"
    Once the library is installed, go ahead and open up **File**->**Examples**->**SparkFun Indoor Air Quality Sensor - ENS160**->**example1_basic**. Make sure to select your board (SparkFun RedBoard) and COM port before hitting upload to begin experimenting with the air quality sensor.

    <div style="text-align: center"><a href="../assets/imgs/Example1_Menu.jpg"><img src="../assets/imgs/Example1_Menu.jpg" alt="Menu Location as listed above"></a></div>

    Alternatively, you can copy and paste the code below to a shiny new Arduino file:

    ??? "Example 1 Arduino Code"
        ```
        --8<-- "https://raw.githubusercontent.com/sparkfun/SparkFun_Indoor_Air_Quality_Sensor-ENS160_Arduino_Library/main/examples/example1_basic/example1_basic.ino"
        ```

    Once you've got your code uploaded, open up a [Serial Monitor](https://learn.sparkfun.com/tutorials/terminal-basics) and check out your output. In the example below, you can see where the board gave me baselines, then readings from my breath. Maybe I should've held off on that peanut butter toast... 

    <div style="text-align: center"><a href="../assets/imgs/Example1_Output.png"><img src="../assets/imgs/Example1_Output.png" alt="Serial monitor output"></a></div>

=== "Example 2: Interrupts"
    Once the library is installed, go ahead and open up **File**->**Examples**->**SparkFun Indoor Air Quality Sensor - ENS160**->**example2_interrupts**. Make sure to select your board (SparkFun RedBoard) and COM port before hitting upload to begin experimenting with the air quality sensor.

    <div style="text-align: center"><a href="../assets/imgs/Example2_Menu.jpg"><img src="../assets/imgs/Example2_Menu.jpg" alt="Menu Location as listed above"></a></div>


    Alternatively, you can copy and paste the code below into a nice new Arduino sketch: 

    ??? "Example 2 Arduino Code"
        ```
        --8<-- "https://raw.githubusercontent.com/sparkfun/SparkFun_Indoor_Air_Quality_Sensor-ENS160_Arduino_Library/main/examples/example2_interrupts/example2_interrupts.ino"
        ```

    Note that depending on which processor board you are using, you may need to alter the Interrupt Pin. Since we're using a RedBoard here, our Interrupt Pin is 2 (`ensInt = 2`). Also, in this example, we've [soldered headers](https://learn.sparkfun.com/tutorials/how-to-solder---through-hole-soldering) to our Air Quality Sensor so that we can use the interrupt pin. Your hardware hookup should look something like the following: 

    <div style="text-align: center"><a href="../assets/imgs/Air Quality Sensor Action Shot-1.jpg"><img src="../assets/imgs/Air Quality Sensor Action Shot-1.jpg" alt="Use the Qwiic connectors to connect the boards to each other and use a jumper to connect the INT pin to Pin 2 of the RedBoard"></a></div>


    Once you've got your code uploaded, open up a [Serial Monitor](https://learn.sparkfun.com/tutorials/terminal-basics) and check out your output. You should see something like the following:

    <div style="text-align: center"><a href="../assets/imgs/Example2_Output.png"><img src="../assets/imgs/Example2_Output.png" alt="Serial monitor output"></a></div>

=== "Example 3: RH and Temperature Compensation"
    This example shows how to give the ENS160 Temperature and Relative Humidity Data for compensation. Note that the values that are given for compensation are not populated in their registers until the Air Quality Sensor is set to "Standard" operation and when data is ready i.e. the data ready bit is set. Also note that there will be some rounding of the temperature and relative humidity values when they're given to the sensor and again when they're read back.

    Go ahead and open up **File**->**Examples**->**SparkFun Indoor Air Quality Sensor - ENS160**->**example3_temp_rh_compensation**. Make sure to select your board (SparkFun RedBoard) and COM port before hitting upload to begin experimenting with the air quality sensor.

    <div style="text-align: center"><a href="../assets/imgs/Example3_Menu.jpg"><img src="../assets/imgs/Example3_Menu.jpg" alt="Menu Location as listed above"></a></div>

    Alternatively, you can copy and paste the code below into a nice new Arduino sketch: 

    ??? "Example 3 Arduino Code"
        ```
        --8<-- "https://raw.githubusercontent.com/sparkfun/SparkFun_Indoor_Air_Quality_Sensor-ENS160_Arduino_Library/main/examples/example3_temp_rh_compensation/example3_temp_rh_compensation.ino"
        ```
        
        
    Your hardware hookup should look something like the following: 

    <div style="text-align: center"><a href="../assets/imgs/Air Quality Sensor Action Shot-2.jpg"><img src="../assets/imgs/Air Quality Sensor Action Shot-2.jpg" alt="Use the Qwiic connectors to connect the boards to each other"></a></div>

        
    Once you've got your code uploaded, open up a [Serial Monitor](https://learn.sparkfun.com/tutorials/terminal-basics) and check out your output. You should see something like the following:

    <div style="text-align: center"><a href="../assets/imgs/Example3_Output.jpg"><img src="../assets/imgs/Example3_Output.jpg" alt="Serial monitor output"></a></div>


=== "Example 4: SPI"
    This example shows basic data retrieval from the SparkFun Indoor Air Quality Sensor - ENS160 using SPI.

    Go ahead and open up **File**->**Examples**->**SparkFun Indoor Air Quality Sensor - ENS160**->**example4_basic_spi**. Make sure to select your board (SparkFun RedBoard) and COM port before hitting upload to begin experimenting with the air quality sensor.



    <div style="text-align: center"><a href="../assets/imgs/Example4_Menu.jpg"><img src="../assets/imgs/Example4_Menu.jpg" alt="Menu Location as listed above"></a></div>

    Alternatively, you can copy and paste the code below into a nice new Arduino sketch: 

    ??? "Example 4 Arduino Code"
        ```
        --8<-- "https://raw.githubusercontent.com/sparkfun/SparkFun_Indoor_Air_Quality_Sensor-ENS160_Arduino_Library/main/examples/example4_basic_spi/example4_basic_spi.ino"
        ```


    Hookup for this example is a bit more complicated. 


    <div style="text-align: center"><a href="../assets/imgs/Air Quality Sensor Action Shot- 03.jpg"><img src="../assets/imgs/Air Quality Sensor Action Shot- 03.jpg" alt="Spi Wiring is a bit messy"></a></div>

    | RedBoard Pin | Air Quality Sensor Pin |
    |:------------:|:----------------------:|
    |     3.3V     |          3.3V          |
    |      GND     |           GND          |
    |      13      |           SCL          |
    |      12      |        ADR/POCI        |
    |      11      |        SDA/PICO        |
    |      10      |           CS           |


    So! Everything is hooked up and you've got your code uploaded - now you can open up a [Serial Monitor](https://learn.sparkfun.com/tutorials/terminal-basics) and check out your output. You should see something like the following:

    <div style="text-align: center"><a href="../assets/imgs/Example4_Output.jpg"><img src="../assets/imgs/Example4_Output.jpg" alt="Serial monitor output"></a></div>
