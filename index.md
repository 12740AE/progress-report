# Smart Dorm/Home Securit Progress Report

## 1. Current progress

We’ve procured all of the sensors we plan on using, to get an initial feel of what kind of readings/range of readings we can expect to get. The following was procured, along with 3.5’’ door hinges to build the model door for this project:

**Sensors needed**

Distance sensor: Ultrasonic Ranging Detector HC-SR04 [Tutorial](https://thepihut.com/blogs/raspberry-pi-tutorials/hc-sr04-ultrasonic-range-sensor-on-the-raspberry-pi)

Accelerometer sensor: ADXL 335 3 axis [Tutorial](https://www.abelectronics.co.uk/kb/article/28/adc-differential-pi-with-adxl335-accelerometer) [Tutorial2](https://www.abelectronics.co.uk/kb/article/28/adc-differential-pi-with-adxl335-accelerometer)

Photoresistor: comes with kit

Light sensor: comes with kit

<p align="center"> <img src="./image/progress1.png" width="350"> </p>

<p align="center">
Figure 1: Door hinges and ADXL 335 accelerometer acquired for project 
</p>

We already know where to get the distance sensor, and have checked the hours for the IDeATe woodshop to build the model door shown in Figure 2. The team worked together to find a simple and easily portable design that modeled our concept. 

<p align="center">
<img src="./image/progress2.png" width="350">
</p>

<p align="center">
Figure 2: Diagram of model door we intend to make in woodshop
</p>

For the lock detection sensor:
For the lock bolt, we decided to just use a dowel in guide holes, shown in Figure 3, just for the proof of concept of the lock-detection capacitive touch sensor. We may need a second Raspberry Pi for the door frame since leads and the sensor are not directly on the door, but on the frame side instead. We will decide how to embed the sensor in the doorframe after building our model through to October 1st. 

<p align="center">
<img src="./image/progress3.png" width="350">
</p>

<p align="center">
Figure 3: Diagram for lock-detection capacitive touch sensor with aluminum foil. 
</p>

Considering other sensors for door open/close detection:
We also had to consider other ways to detect someone entering/leaving the room- or the door opening/closing to signify this event. In our kit, we also have a passive IR sensor. This sensor seems to best be for detecting if there is generally something moving in the area by detecting the IR radiation emitted from people. According to Arrow.com, the circular housing around the sensors is to “widen the sensing area”, which we don’t need for a very localized event as opening a door. A much better sensor to us is possibly an active IR sensor since we know exactly where our movement will occur: within the range of the door frame. We will still try the accelerometer and possibly the light sensor as well. 

## 2.Problems Encountered
**(1)Difficulties setting up working Raspi at home without equipment**

Since we intended to do a lot of work off campus, we tried to  connect the raspberry pi to share internet with our pcs and at-home wifi (no one has a monitor, keyboard, or required HDMI cable off-campus). The initial connection by bridging the wifi and ethernet in our laptop worked and we were able to find the dynamic Raspi IP address to input into Putty using Advanced IP Scanner, to SSH in an setup wireless connections through the Raspi’s command line. However, the wireless connection was unsuccessful (not sure why), and we decided to go through the multiple steps to stay with sharing the pc’s internet with the Raspi. We used these tutorials for [sharing wifi through an ethernet cable](https://www.hackster.io/Anwaarullah/sharing-wifi-with-raspberry-pi-using-a-lan-cable-ae1f44) and [setting up wifi through the command line](https://www.raspberrypi.org/documentation/configuration/wireless/wireless-cli.md). 

**(2)Difficulties on placing the sensor (see Future Plan)**

## 3.Future Plan
For the first half of the week of September 29th, we will be building the door frame as shown in Figure 2 in either the IDeATe or CEE woodshop. Then we’ll be able to determine how to install/feasibility of the capacitive lock sensor. 
We will also try to run code to access sensor readings for the distance sensor, accelerometer, photo resistor and light sensor. Over the past weekend, we have not been able to use the Raspi easily but spent time collecting possible resources. 




