[Home](https://team307.github.io/) | 

---
# Software Implementation
---

## Software Approach

The Software Proposal was created in our group in order to capture the software flow and visually explain what is being done in the background that operates all our electrical components in a fluid environment. This diagram does not display any actual code but expresses the design's software functionality Our group had discussed many approaches to how we wanted our software to run with the goal of meeting our stakeholder's needs and keeping it relatively simple and easy to understand. We discussed that when we created the software it needs to be straightforward with a focus on LED lights in appropriate areas to help discover bugs and to make testing and debugging easy. Our group will be primarily using MPLab and MCC to program our microcontroller and sensors.

The software is divided into 4 sections:

* Main Loop
* Initialize System
* Refresh System
* Motor Drivers

<br/>

![Software proposal](https://user-images.githubusercontent.com/122499832/224884183-7c1c6421-7758-4ccf-94c4-9332b08e496e.jpg)

<br/>

When looking at our user needs/project requirements there were specific points we had to make sure that our code met. One requirement is we need to make sure that we include interrupts in the software which can be found in the Main loop; after the system initializes and determines the state of where the software it is at is when our interrupts are enabled. This is where the weather/ climate data is received, The program then reads sensor data and interprets the data. At this stage of the software is when the system enables the interrupt, if the required value isn’t read then it will loop back until a value that is read signals to engage the mister. This meets our requirement of needing an actuator that is controlled based on data that was being read by a sensor. Our sensor that is used for this requirement is our humidity sensor. EUSART will also be used to communicate data to the ESP32 and this will then be transmitted on WiFi to meet that connectivity requirement as well. We are also using both I^2C and SPI serial communication to meet that requirement as well as our sensors use I^2C and our motor driver uses SPI.

<br/>

## Top 5 biggest Changes

The software design process proved to be challenging in many ways and forced our team to make significant changes to our original software design in order to get our product to work successfully. these are the five biggest changes that our team made to the software and code.


1. Changes getchar to int get to allow the pic to use Eusart to the ESP32

2. Removed while loops that were supposed to output values simultaneously for the temperature sensor and the humidity sensor.

3. Wrote functions to call, to streamline Main C.

4. Had to remove interrupts due to interfering with the code.

5. Changed The WiFi address for MQTT to Hotspot off a personal phone in order to get a better connection from the ESP32.

In the end, the majority of the changes that we made to our code proved to be pointless because everything that we changed proved to not be beneficial because we couldn't get the Esp3n and the humidity sensor to work.


<br/>

## Software  Design Version 2.0 Discussion

Our team ran into issue after issue with our code, we believe that our software diagram was great and represented a clear and concise run with how our software ran and was outlined but all our group's issues were within the code. For starters, our team focused on using components that were used for in-class check-offs as well as homework assignments because we believed in staying with a component that we have familiarized ourselves with. each sensor originally had working code, but when it came to debugging and having the code for each system run simultaneously, we ran into roadblocks. with the 2.0 version, we would focus on creating a code that involves all systems running smoothly. In order to achieve this we would divide the code by each team member that falls in their subsystem and request to have two or more working formats of code. this would allow us to have more options to choose from when it comes to building and debugging. We believe this would be beneficial because the code that we originally had working was no longer working for our system and having more working code to choose from would be helpful. After successfully getting the code, our group would then make sure that our software diagram flows the same way that our code flows.


<br/>

## MQTT Topic Table & Code

Please refer to the **Master Appendix** and scroll down to **Appendix H** to view our teams MQTT and Code.

<br/>