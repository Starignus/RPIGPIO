# Introduction to Raspberry Pi

* [What is a Raspberry Pi](#rpi1)
* [Models of Raspberry Pi](#rpi2)
* [Raspberry Pi Board](#rpi3)
* [Why Raspberry Pi?](#rpi4)


## <a name="rpi1"></a> What is a Raspberry Pi

Raspberry Pi is a small computer of the size of a credit card that you can plug in a TV/monitor, keyboard and mouse. You can use it in the same way as you desktop PC or laptop does, like generating spreadsheets, word processing, browsing the internet, and playing games. It also plays high-definition video. However, what does more interesting Raspberry Pi (RPi), is the capability to make electronics projects with it! The main aim of RPI's design is to teach young people to program and to create new ideas. It has a free licence Linux operative system hold in an SD card and powered by a USB phone charger.

<img src="pi3card.png" alt="rpicard" style="width: 300px;"/>

## <a name="rpi2"></a> Models of Raspberry Pi

There are different models of Raspberry Pi.


<img src="raspberry-pi-products.jpg" alt="rpiproducts" style="width: 500px;"/>

All of them have different hardware specifications.

<img src="RPIspecific.png" alt="specifications" style="width: 400px;"/>


We will be working with the **RPi 3 Model B** that was launched in February 2016; The microprocessor is a Broadcom chip BCM2837 SoC <sup>[1](#myfootnote1)</sup>,  it uses a 1.2GHz 64-bit quad-core ARM Cortex-A53 CPU, has 1GB RAM, integrated 802.11n wireless LAN, and Bluetooth 4.1.

<a name="myfootnote1">1</a>: SoC: System on Chip. A computer on a single chip.


## <a name="rpi3"></a> Raspberry Pi Board

<img src="RPI3B.jpeg" alt="rpiboard2B" style="width: 350px;"/>

The RPi board shown in the figure, at the right-hand side, you have the **USB ports** and blow that on the right is the port for **Ethernet**. Behind the USB ports,  there is an **interface IC chip** or controller of the USBs and Ethernet. At the top,  you can find the general purpose **I/O GPIO pins** (40 pins). Down the bottom middle is the **CSI (Camera Serial Interface) camera** connector. You can get a camera for Raspberry PI and plug it in. Also, you have the option to connect a webcam to a USB. At the right-hand side, you can find a **DSI (Display Serial Interface) connector** which you can use to connect an LCD screen. At the bottom, you can find the **HDMI port**. HDMI to plug it straight into a monitor. At the bottom, you can find the HDMI port. HDMI to plug it straight into a monitor. Next to the HDMI you can see the **USB power connector** and also an **audio port**.

<center> <img src="RPI2Bback.png" alt="backrpiboard2B" style="width: 200px;"/> </center>

### Important

* Always make sure you supply only 5 V to the RPi.
* Unlike Arduino, RPi does not have over-voltage protection on the board (yet) as Arduino, be careful when making GPIO connections.
* Please DO NOT connect over 3.3V  or less than + 0V as input.
* Never demand that any output pin source or sink more than 16 mA.
* Pins can supply only maximum 50 mA.


## <a name="rpi4"></a> Why Raspberry Pi?

Why we chose RPI? When you compare RPI with Arduino, at first instance you can think that RPI is just faster and better and superior (Better processor and RAM memory). However,  Arduino, even though is older,  is well suited to certain tasks. Therefore, I would not say RPi is superior to Arduino or Arduino is superior to RPi. It just depends on what you want to use them. They are different and suitable for various aims.

| Name | Raspberry Pi 3 B | Arduino 101 or Genuino 101|
| ----- | -----| ---- |
| Release | February 2016 | October, 2016|
| Size | 85.60 mm × 56.5 mm | 68.6 mm × 53.4 mm |
|Processor| 64-bit quad-core ARM Cortex-A53 | 32-bit Intel Curie, two tiny cores an x86 (Quark SE) and an ARC|
|Frequency| 1.2GHz | 32MHz|
| RAM | 1 GB | 24 kB|
| Flash Memory| SD card (2 to 16 GB) | 196 Kb|
|Operating system| Linux | None|
|Integrated Development Environment| Scratch, IDLE, any that Linux support| Arduino IDE|
| On Board Network| 10/100 Mbit/s Ethernet, 802.11n wireless, Bluetooth 4.1 | Bluetooth LE|
| Multitasking| Yes |No|
|Operating Voltage | 5 V   | 3.3V (5V tolerant I/O)|
| Input Voltage (recommended)| 5V | 7-12V|
|USB| 1 | 4 (via the on-board 5-port USB hub) |
| Digital GPIO| 17 ( GPIO can be reconfigured as UART, I²C, SPI, PWM)|14  (of which 4 provide PWM output)|
| Analog | 0 | 6 |
|Digital PWM | 0 | 4 |
|Video Output| HDMI | None|
|Audio Output|HDMI| None|

References of table:
* Arduino [[1](https://www.arduino.cc/en/Main/ArduinoBoard101), [2](https://en.wikipedia.org/wiki/List_of_Arduino_boards_and_compatible_systems)]
* RPI [[1](https://en.wikipedia.org/wiki/Raspberry_Pi#RAM), [2](http://elinux.org/RPi_Low-level_peripherals#cite_note-7)]

Another main difference between RPI and Arduino is that RPI has an operative system, whereas Arduino has not. The latter, you can run the code and run directly on the microcontroller. The presence of an operative system, make all the precess slower since the application does not directly interact with the microcontroller. What it means is that the application can not change a pin directly (turn from high to low or low to high), it has to go through the operative system. But there are many advantages of having an operative system.

<center> <img src="OSIot.png" alt="OS" style="width: 200px"/> </center>


<img src="OSIot.png" alt="alt text" width="200" height="200">

![](OSIot.png = 100)

The first thing you get is really a user interface. Arduino does not have a real user interface. It means that can do too much with it unless you write a program telling how to manipulate the pins, and may be is going to do something. In the case of having an operative system as in PRI, you can perform different tasks at the same time (multitasking); send and email, browsing the internet, coding and run the code to control the pins. We will see more about the RPI-Linux operating system with more detail in a bit.
