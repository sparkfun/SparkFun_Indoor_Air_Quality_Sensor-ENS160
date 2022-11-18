The [SparkFun Indoor Air Quality Sensor - ENS160 (Qwiic)](https://www.sparkfun.com/products/20844) makes use of the ENS160 from ScioSense - a digital multi-gas sensor solution with four sensor elements that can be used in a wide range of applications including building automation, smart home, and HVAC. The independent hotplate control allows the detection of volatile organic compounds (VOCs) including ethanol, toluene, hydrogen and oxidizing gases with superior sensitivity. The ENS160 supports intelligent algorithms to process raw sensor measurements on-chip. These algorithms calculate CO2-equivalents, TVOC, air quality indices (AQIs) and perform humidity and temperature compensation, as well as baseline management, all on chip. Raw sensor measurements can be read for further customization. Let's dig in!



<div style="text-align: center">
  <table style="border-style:none">
    <tr>
      <td>
        <a href="https://www.sparkfun.com/products/20844">
          <div style="text-align: center"><img src="https://cdn.sparkfun.com/r/500-500/assets/parts/2/0/6/1/0/ENS160-_01.jpg" alt="SparkFun Indoor Air Quality Sensor - ENS160 (Qwiic)" height="500px"></div>
          <h3 style="text-align: left">SparkFun Indoor Air Quality Sensor - ENS160 (Qwiic)
          </h3>
        </a>
        <div style="text-align: left"><span style="text-align: left">SEN-20844</span></div>
      </td>
    </tr>
  </table>
  </div>


### Required Materials

To follow along with this tutorial, you will need the following materials. You may not need everything though depending on what you have. Add it to your cart, read through the guide, and adjust the cart as necessary.

<div>
<table style="border-style:none">
    <tr>
        <td width="140">
            <a href="https://www.sparkfun.com/products/20844">
              <div style="text-align: center"><img src="https://cdn.sparkfun.com/assets/parts/2/0/6/1/0/ENS160-_01.jpg" alt="SparkFun Indoor Air Quality Sensor - ENS160 (Qwiic)" height="140"></div>
              <h3 style="text-align: left">SparkFun Indoor Air Quality Sensor - ENS160 (Qwiic)</h3>
            </a>
            <span>SEN-20844</span>
        </td>
        <td width="140">
            <a href="https://www.sparkfun.com/products/15123">
              <div style="text-align: center"><img src="https://cdn.sparkfun.com//assets/parts/1/3/4/9/2/15123-SparkFun_RedBoard_Qwiic-01a.jpg" alt="SparkFun RedBoard Qwiic" height="140"></div>
              <h3 style="text-align: left">SparkFun RedBoard Qwiic</h3>
            </a>
            <span>DEV-15123</span>
        </td>
        <td width="140">
            <a href="https://www.sparkfun.com/products/14426">
              <div style="text-align: center"><img src="https://cdn.sparkfun.com//assets/parts/1/2/4/5/2/14426-Qwiic_Cable_-_50mm-01.jpg" alt="Qwiic Cable - 50mm" height="140"></div>
              <h3 style="text-align: left">Qwiic Cable - 50mm</h3>
            </a>
            <span>PRT-14426</span>
        </td>
    </tr>
    <tr>
    <td width="140">
        <a href="https://www.sparkfun.com/products/10215">
          <div style="text-align: center"><img src="https://cdn.sparkfun.com//assets/parts/4/5/5/8/10215-01.jpg" alt="USB micro-B Cable - 6 Foot" height="140"></div>
          <h3 style="text-align: left">USB micro-B Cable - 6 Foot</h3>
        </a>
        <span>CAB-10215</span>
    </td>
    </tr>
</table>
</div>



### Suggested Reading

If you aren't familiar with the Qwiic system, we recommend reading [here for an overview](https://www.sparkfun.com/qwiic).

<div style="text-align: center">
<table style="border-style:none">
  <tr>
   <td>
   <div style="text-align: center"><a href="https://www.sparkfun.com/qwiic"><img src="https://cdn.sparkfun.com/r/457-457/assets/learn_tutorials/8/2/Qwiic-registered-black.png" alt="Qwiic Connect System" title="Click to learn more about the Qwiic Connect System!"></a></td></div>
  </tr>
  <tr>
    <td><div style="text-align: center"><i><a href="https://www.sparkfun.com/qwiic">Qwiic Connect System</a></i></div></td>
  </tr>
</table>
</div>

If you aren’t familiar with the following concepts, we also recommend checking out a few of these tutorials before continuing.

<table style="border-style:none">
    <tr>
        <td style="vertical-align: text-top;" width="264px">
            <a href="https://learn.sparkfun.com/tutorials/i2c">
            <div style="text-align: center"><img src="https://cdn.sparkfun.com/c/264-148/assets/learn_tutorials/8/2/I2C-Block-Diagram.jpg" style="width:264px; height:148px; object-fit:contain;"></div>
            <h3 style="text-align: left">I2C
            </h3></a>
        </td>
        <td style="vertical-align: text-top;" width="264px">
            <a href="https://learn.sparkfun.com/tutorials/serial-basic-hookup-guide">
            <div style="text-align: center"><img src="https://cdn.sparkfun.com/c/264-148/assets/learn_tutorials/5/9/7/14050-01.jpg" style="width:264px; height:148px; object-fit:contain;"></div>
            <h3 style="text-align: left">Serial Basic Hookup Guide
            </h3></a>
        </td>
        <td style="vertical-align: text-top;" width="264px">
            <a href="https://learn.sparkfun.com/tutorials/redboard-plus-hookup-guide">
            <div style="text-align: center"><img src="https://cdn.sparkfun.com/c/264-148/assets/learn_tutorials/1/7/5/8/18158-SparkFun_RedBoard_Plus-01.jpg" style="width:264px; height:148px; object-fit:contain;"></div>
            <h3 style="text-align: left">RedBoard Hookup Guide
            </h3></a>
        </td>
    <tr>
</table>
