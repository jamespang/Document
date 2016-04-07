# Specifications
* Microcontroller：ATmega328P-MU
* Operating Voltage：5V
* Digital I/O Pins：14
* PWM Channels：6
* Analog Input Channels：7
* DC Current per I/O Pin：40 mA
* Flash Memory：32 KB（ATmega328P-MU）
* RAM：2 KB（ATmega328P-MU）
* EEPROM：1 KB（ATmega328P-MU）
* Clock Speed：16 MHz

# Interface Function
![Seeeduino Lotus][Seeeduino_Lotus]
[Seeeduino_Lotus]: http://goo.gl/SVhpb2

1. Micro USB
2. Reset button
3. Analog Ports：Analog sensors can return readings ranging from 0 to 1023. Compared with digital sensors that only return 0 or 1, analog readings are more detailed and precise.
4. I2C Ports：I2C is a low-speed bus protocol that transfers data via two wire：SCL and SDA. SCL is the clock line that synchronizes data transfer over the I2C bus, and SDA is the data line.
5. Digital Ports: Normally, they are used when reading a digital sensor that only outputs 0 or 1, or turning ON or OFF an actuator.
6. UART Port: We can control serial device by this port.

# Driver Install
請參考 [Wiki](http://www.seeedstudio.com/wiki/Seeeduino_Lotus_v1.0)

# matchUP 整合要點
* 设备型号：添加 Seeeduino Lotus
* Workboard：添加 Seeeduino Lotus wireframe
* Compile API：经 Arduino.cc IDE 1.6.7 实测，开发板须选择 [**Arduino Uno**](https://www.arduino.cc/en/Main/ArduinoBoardUno)
* 模块拖拉：对 Input/Output port 做防呆
* Driver Install

| Interface           | Pin        | Quantity |
| ------------------- | ---------- | -------- |
| Digital Input       | D2～D7     |          |
| Digital Output      | D2～D7     |          |           
| Analog Input        | A0、A2、A6 |          |
| Analog Output（PWM）| A0、A2、A6 |          |
| I2C                 | SDA、SCL   | 2        |
| UART                | UART       | 1        |
