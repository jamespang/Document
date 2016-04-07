# Specifications
* Digital I/O pins：2
* I2C port：1
* Analog Input channels：2（Multiplex with I2C）

# Hardware Overview
![Grove - Joint v2.0][Grove_Joint_v2.0]
[Grove_Joint_v2.0]: http://goo.gl/BzD7WT
* Battery Interface - This moudle can battery powered（**A2**）.
* Light Sensor - There's a light sensor on the board which is connected to **A0** pin.
* Status LED - There're 3 LEDs indicate the status of the board. Tx(**D1**), Rx(**D0**) and L1(**D10**)
* INPUT Port - The INPUT Port is a Grove I2C interface as well as two analog channels(**A4** & **A5**).
* OUTPUT Port - The OUTPUT Port is a Grove Interface too including two digital I/Os (**D5** & **D6**).
* Button - The button is connected to **D2**, It can be used as a switch as well.
* Micro USB Port - It can be used for power supply and download the code.
* Power LED - The LED+ connect to VCC and LED- connect to **D6**, you can turn **D6** HIGH to turn off this led to save power.
* CHRG LED - The LED+ connect to VCC and LED- connect to **A3**, you can turn **A3** HIGH to turn off this led to save power.

# Driver Install
* Windows / Linux
* OS X

請參考 [Wiki](http://www.seeedstudio.com/wiki/Grove_-_Joint_v2.0)

# matchUP 整合要點
* 设备型号：添加 Grove - Joint
* 设备型号：移除 Genuino
* 设备型号：选择不同设备型号时，必须切换成相对应的平台
* 平台：移除切换成 Grove - Joint 平台的按钮
* UI：操作发生变动时，设备型号变回 Arduino Uno
* Compile API：经 Codebender 实测，开发板须选择 [**Arduino Fio**](https://www.arduino.cc/en/Main/ArduinoBoardFio)
* 模块拖拉：对 Input/Output port 做防呆

| Interface           | Pin      |
| ------------------- | -------- |
| Digital Input       | A4、A5   |
| Digital Output      | D5、D6   |           
| Analog Input        | A4、A5   |
| Analog Output（PWM）| D5、D6   |
| I2C                 | SDA、SCL |
