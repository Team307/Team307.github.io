[Home](https://team307.github.io/) | 

---
# Hardware Implementation
---

<br/>

## Summary

The voltage regulator and MCC sub systems were designed Sam Masamitsu. The switching voltage regulator takes +9V and brings it down to 3.3V which is used by the MCC, the two sensors, and the motor actuator. The MCC communicates with the temperature and humidity sensor to send readings via ESP32 to a computer. It also tells the motor driver when to activate the mister changing the humidity within the enclosed enviroment. This meets the user needs by measuring a minimum of two atmospheric readings and having an acuator that activates in response to the sensors. The MCC will communicate via I2C wit the sensors and ISP with the motor driver. The design was primarly driven by the team's understanding of what the system requirements were. The team decided to use sensors that were already being tested in class to mitigate the amount of unknown issues. 



<br/>

![Final Schematic](https://user-images.githubusercontent.com/122499832/233190883-8cdc6d47-7c06-4f02-a94e-c3420a3dc0f3.jpg)


<br/>

Please refer to the **Master Appendix** and scroll to **Appendix G** for a view of our Bill of Materials.

## Team PCB Front & Back Screen Shots

**Top**

![PCB TOP](https://user-images.githubusercontent.com/122499832/233799141-aaa4fe73-3da3-4b04-b1c8-b0ad2b927000.PNG)

**Bottom**

![PCB Bottom](https://user-images.githubusercontent.com/122499832/233799144-8aabca42-8ce5-4b31-b526-f03965200009.PNG)

<br/>

## Team PCB Front & Back Photos

**Top**

![Top PCB pic](https://user-images.githubusercontent.com/122499832/233799145-90254991-64fb-4162-84d9-ae4a12d27a52.jpg)

**Bottom**

![Bottom PCB pic](https://user-images.githubusercontent.com/122499832/233799147-61b67a27-15dd-411d-822c-e45ca14dba93.jpg)


<br/>

## Hardware design Version 2.0 Discussion

<br/>

As a team, there are several changes that we would make to our design. First of all, there would be an inclusion of more debugging LEDs to assist in the troubleshooting of the board. This would help our team by lighting up and showing which components are having issues and would have saved us time by going through each individual component and investigating what our issue could possibly be. We would also make the sensors on daughter boards so we could have more freedom in where we placed the board. In regards to running traces, we would have both of the I2C sensors on the same I2C pins for the PIC to leave pins open for the SPI motor driver. Lastly, we would have added a pad for a 330 uf capacitor to rectify the signal post inductor of the variable power regulator.
