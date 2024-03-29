---
# Home
---


<br/>

# Project Name: Mobile Environmental Sensing

<br/>

# Team 307

<br/>

## Class: EGR 314, Spring 2023

<br/>

## Team Members : Connor O, Samuel M, Jake Tangeman, Jadrian Padilla

<br/>

### Arizona State University, Class: EGR 314 PM Session, Professor Travis Kelley

<br/>
  <br/>

---
# Presentation
---

<br/>
  <br/>
    <br/>

<iframe width="560" height="315" src="https://www.youtube.com/embed/Yx9dJdSQKJo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

<br/>
  <br/>

---
**Table of Contents**  

- [Home](#Home)
- [Team Organization](#Team-Organization)
    - [Summary](#summary)
    - [Team Charter](#team-charter)
    - [Product Mission Statement](#product-mission-statement)
- [User Needs, Benchmarking, and Requirements](#user-needs-benchmarking-and-requirements)
    - [Introduction](#introduction)
    - [objectives](#objectives)
    - [Stakeholders](#stakeholders)
    - [Use Cases](#use-cases)
    - [Aspects](#aspects)
- [Design Ideation](#design-ideation)
- [Selected Design](#selected-design)
- [Block Diagram](#block-diagram)
- [Component Selection](#component-selection)
- [Power Budget](#power-budget)
- [Microcontroller Selection](#microcontroller-selection)
- [Hardware Proposal](#hardware-proposal)
- [Software Proposal](#software-proposal)
- [Master Appendix](#master-appendix)

  <br/>


---
# Introduction
---

 <br/>

The Innovation Showcase is an event held at Arizona State University for upper divisional engineering students that showcase their final project to their professors and stakeholders as well as other students that visit and public. The main focus of this event is to explore what engineering students have developed over the course of the semester and see how they apply the knowledge they have gained and infuse it into a functional design. Specifically for Engineering 314 students, their project is to produce a system that interacts and corresponds with the environment and is required to use serial sensing and actuation. Another requirement is that their project/design must broadcast their environmental data using WiFi using the MQTT protocol. Students must include a design that senses at least two environmental conditions and two separate serial sensors. It is also required in the plan to include at least one motor controlled by a motor controller over I2C or SPI-based protocol. The working product of the engineering groups will be presented at the showcase on April 28th, 2023, and will be evaluated by professors for correct functionality as well as meeting the course requirements.

Members of Group 307 have collaborated with each other to determine the ultimate weather device that meets course requirements while maintaining a simplistic approach in order to ensure a fully functional device to display at the showcase. Our design consists of electrical components that will correspond with one another to determine the temperature and humidity of an enclosed environment. Our design will have inexpensive parts and will utilize components that are supplied within the campus. The mechanical parts will also be inexpensive and easily replaceable if lost or damaged. The groups focus on creating a simple software environment and coding aspects that will be user-friendly to anyone who engages with our product.


<br/>

---
# Team Organization 
---

<br/>

## Summary

_In EGR 314 we formed our group with four members and became group 307. The first event that happened with our group was the exchange of contact information in order for us to be able to communicate properly. We have three sources of contact information which are Texting, emailing, and discord. The primary communication ways will be texting and discord for audio and video chat. In our group, we hold each other accountable for remaining communicative with each other and provide constructive feedback and input whenever it is needed. When our group approached the team charter for our Team Organization assignment, we focused on each member's desired need and want from this class to be successful. Each member provided a statement that ultimately led to what we felt would lead to a successful goal and a promising product. Afterward, our group came together and created the following Team Charter and a meaningful mission Statement._

<br/>
  <br/>

## Team Charter

**Our team strives to have a successful product, we believe that with concise communication and dedication to hard work, and schedule commitment, we can achieve our goals.**

**A product that meets our stakeholder’s expectations, working with no bugs or other interruptions that can hold the product from being a complete product.**
**Not only receiving an A on the project but also being able to understand and explain fluidly how the system works.**
**Building a professional relationship with group members and faculty through thoughtful questions, respectful answers, and clear communication.**
**Expanding our individual knowledge and skill sets through peer guidance and teaching. We will allow ourselves to not only be available for teaching but to be taught.**
**Holding ourselves and our team members accountable to the tasks assigned and the standards set forth in this charter. This will create an environment where we are working **together as peers toward our common goals.**

<br/>

## Product Mission Statement

**To develop an interactive system that reacts to environmental changes and be displayed at the ASU showcase while achieving our course objectives and requirements.**


Our group believes we have knowledgeable team members and strong-minded individuals who will stay true to the mission statement and follow the team charter religiously. With both these strong Charter and statements, we believe that we will have a successful product for our professors and our stakeholders. For the rest of the sections in our team organization assignment, refer to Appendix A: Team Organization on the Appendix Page.


---
# User Needs, Benchmarking, and Requirements
---

<br/>



_The User Needs assignment was the kick-off to our group's brainstorming for this project, we did not know entirely what our project will end up being but came up with ideas shortly after understanding what the project description was asking for out of us. First, we invested our time in the project description to truly understand what we can and cannot have included in our design. Afterward, we individually did research on similar products and created a VOC chart. We found products that were like the theme of our project was and looked at positive and negative reviews and pulled out what was explicitly and latently being called out in the review. This helped our group weigh out the important needs for what our users will be expecting or should expect._

_Next, we created a Jam Board of sixty needs that our product should have to be a successful product. Each of us jotted down roughly 12 to 15 needs each. After we had the sixty needs, we then sought to organize the needs by color; Blue being the most important need for our design, green being a medium need, and yellow being the lowest need for our group's design. Before we rated our needs, our group compared our needs to what was being called out in VOC reviews and reviewed which of our needs stood out the most of what users are asking for in products. After we organized them in groups by color, we then had our user needs that we felt needed to be implied to our project and design. Our design will be assessed over the aspects we provided in our user needs in many ways. We will approach each assignment and step throughout the building process by looking at our user's needs and verifying that we are following what is important to the users to create a successful design. After each completion of each part of this product, we will refer back to our user needs and ask ourselves the following:_
- _Are we satisfying the needs in our design?_
- _Does this meet the course requirements?_ 

<br/>
  <br/>



## Objectives

The primary goal of our team is to create a simple yet robust, hands-on design that allows the user to detect a change in temperature in an environment as well as detect the humidity levels in that same environment and display the data on an LED screen. It is important to the design to maintain a focus on inexpensive and reusable materials for the modular components that will be used by the user. Our group's belief is that simple and inexpensive parts and presentations will lead to an impactful learning course for all users that come across our design. Our focus is that anyone of any age and language background could easily pick up the device and understand how to use the system. The final product will consist of two sensors which will allow the user to interpret two environmental conditions and display that data on the screen to the user.

<br/>

## Stakeholders

**Professors**: The Primary Stakeholders for this project, in charge of looking for and determining the design and project meets expectations. Looking for new and exciting ways for groups to apply their knowledge in their designs and product. Looking for products that sense two environmental conditions while using two sensors. Will disqualify a project if the group is using preexisting products.

**Showcase Visitors**- Public viewers and ASU students that are interested in different products and/or new technologies that they can observe and increase knowledge of current and future environmental data suppliers.

**Volunteers**- Individuals that interact with research teams as well as visitors and provide information, tutorials, and important safety and guidance.

**Research Teams**- Scientists and engineers that are looking to discover new ways to explore how to interpret temperature or other weather-related information. Their research focuses on engagement in interests, identity, and exposure.

<br/>

## Use Cases

**The Visitor**: An outside visitor hears of the showcase that focuses on products that interact with environmental weather conditions and is intrigued. This visitor is constantly outdoors and sometimes in harsh conditions. He/She is looking for something that will be small and compact and sturdy enough to handle severe weather conditions. 

**Hiking Interaction**: This hiker has borrowed a prototype of our product and puts the design to the test when they go on week-long hiking trips. They utilize the device by checking what the temperature is outside and reading off humidity levels in the environment that they are in.

<br/>

## Aspects

The product research and design will focus on materials that will correctly determine weather conditions while maintaining an inexpensive design.

<br/>

**1.	Product Design**
  
- **1.1** The product shall contain materials that are inexpensive and easy to find.

- **1.2** The product shall consist of at least one motor.

- **1.3** The motor shall be controlled by a motor controller.

- **1.4** The product shape should be small enough to fit in a pocket or a small bag.

- **1.5** The product shall consist of materials such as plastic and metal.

- **1.6** The product shall be weatherproof.

<br/>

**2.	Software/ Functionality**

  - **2.1** The Product shall function in harsh environments.
  
  - **2.2** The product shall interpret two or more environmental conditions.
  
  - **2.3** The product shall function based on coding and allow for motors to operate between different speeds
  
  - **2.4** The product shall Sense with two separate serial sensors.
  
  - **2.5** The charger shall provide 12+ hours of operation usage.

<br/>

**3.	Interactivity**

  - **3.1** The products shall be designed to withstand damage and accidental drop age
  
  - **3.2** The software shall be easy-understanding software for any user.
  
  - **3.3** The product shall be available for any age.
  
  - **3.4** The product shall have little to no assembly necessary.
  
  - **3.5** The product shall consist of buttons to swap between data points.

<br/>

**4.	Customization**

  - **4.1** The product sensing parts shall be interchangeable.
  
  - **4.2** The product should have the ability to change between different weather conditions.
  
  - **4.3** The product shall be appealing to all age groups.
  
  - **4.4** The product shall be used for more than one scenario.

<br/>

**5.	Manufacturing**

  - **5.1** The total cost of the product shall be less than $100
  
  - **5.2** The materials of the product shall be inexpensive and easily accessible.
  
  - **5.3** Materials need to be sturdy and lightweight.
  
  - **5.4** The product shall only take 10 minutes to build
  
  - **5.5** The product shall not follow concepts of existing projects.

<br/>

**6.	Safety**

  - **6.1** Protective gloves will be provided
  
  - **6.2** Protective eyewear will be provided and mandated depending on the materials that are being used.
  
  - **6.3** Electrical components must be at a safe voltage.
  
  - **6.4** Any sharp objects will be facilitated.

<br/>

## Open Questions

-	Will the battery be replaceable or rechargeable?

**We will be using a replaceable battery and will also provide ourselvs a battery backup incase unseen issues happen.**

-	Can we improve the battery life and reduce the amount of battery recharge?

**We can improve battery life if we have the design connected to a power source that connects to the wall.**

-	Are there better materials that can be applied to the product other than plastic while still remaining cost-effective?

**Our group determined that plastic was the cheapest option.**

-	Can we improve on the customization of the software so the user can choose what environmental condition to focus collecting data on?

**Are Team did not have enough time to test and debug the software to includ the option where a user can control environmental conditions.**
  
<br/>  
  
## Milestones

-	Concept Presentation: 1.23.2023 

-	Design Presentation: 3.17.2023

-	Design Freeze:4.24.2023

-	Planned Release: 4.28.2023


---
# Design Ideation
---

<br/>

## Summary

_The process that our group followed for the design ideation is fairly straightforward and simplistic. Our group discussed after class on campus and over the phone via text messages was the easiest way to bounce ideas back and forth from one another. Our brainstorming methods were an open format approach to allow for individual brainstorming before switching to group brainstorming. Our group did not face any scenarios of brainstorming that haven't worked yet. An idea created by an individual group member would create a branch of discussions and often lead to further expanding on one idea or creating another idea to apply to the group's design ideation. Each team member played a similar role when creating ideas, which was individually brainstorming concepts and bringing them to a group discussion for further discussion and brainstorming. We then created a Jam Board and put our needs on sticky notes; as seen in Appendix C. The organization process was chaotic in the beginning but with each member having experience using the Jam board, it became organized quickly. Our 100 design ideas were then separated into groups and each group was then colored by the importance of the design idea._

_The process of organization for the Jamboard was an equal group member session in Discord where we all joined online on a shared screen and talked about each sticky note. After discussing the importance of each note the group ranked the sticky note together and placed them in the required group. Our group has three sketches and they were done by Samuel, Jake, and Jaydrian. A sketch has yet to be selected as our primary design._

<br/>
  <br/>

## Design 1

![Design Concept 1](https://user-images.githubusercontent.com/122499998/213979043-16a1a8ac-b5f1-49d3-9f35-0d540b30768d.svg)

Set up in a + formation with a temperature sensor at each end of the legs. One leg will also have a humidity sensor. There is a motor in the center connected to a rod that a solar panel will be connected to. The motor will spin and turn to face the temperature sensor that is reading the highest temperature as this will most likely be the sensor that is facing the sun.

<br/>

## Design 2

![Design Concept 2](https://user-images.githubusercontent.com/122499998/213979192-374ce69b-720a-4d42-b3d8-adfbf4cf4eeb.svg)

In our second design concept, we will have an enclosed water reservoir with a spray nozzle. The motor will actuate the release mechanism for the mister. A humidity sensor, thermometer, and mister will all be enclosed within a plastic dome. Should the humidity be under a given level at a specified temperature, the motor will activate and mist the dome to bring the humidity to its desired level.

<br/>

## Design 3

![Design Concept 3](https://user-images.githubusercontent.com/122499998/213979279-99e99768-e3a7-4c7c-8c2c-5f0927bf1510.svg)

Our third concept, similar to our second, will have an enclosed water tank to be sprayed using a mister. Though this design would measure ambient temperature and humidity and would use a combination of adjusting fan speed and spraying water to reach the desired temperature and humidity levels. The internals will be encased in a plastic octagonal casing with a tapered top where the sensors, misters, and fans will be placed.*

---
# Selected Design
---

<br/>

## Design 2

<br/>

When determining what design to go with out of the three that we had sketched, our group decided that our second design approach was the best pathway. We felt that the particular design had the best ideas from designs one and three and we did not include any other design ideas that weren't already there. Our decision for picking this design was made by setting up a discord meeting and discussing what would be simple yet fun to build and we all agreed that design two was the best option. The design that we pursued does not deviate from the design ideation section.

![Design Concept 2](https://user-images.githubusercontent.com/122499998/213979192-374ce69b-720a-4d42-b3d8-adfbf4cf4eeb.svg)

<br/>

In our second design concept, we will have an enclosed water reservoir with a spray nozzle. The motor will actuate the release mechanism for the mister. A humidity sensor, thermometer, and mister will all be enclosed within a plastic dome. Should the humidity be under a given level at a specified temperature, the motor will activate and mist the dome to bring the humidity to its desired level.



---
# Block Diagram
---

<br/>

## Summary


The team's original block diagram received feedback from the professors and the teaching team and made comments on some issues that needed to be resolved. These issues included missing manufacturers for all parts excluding the MCU. We also received comments that UART is not a parallel interface, as well as being told that our ICSP uses more than one pin. Some other feedback on our block diagram was that our labels required more information when it came to labeling serial interfaces as well as some arrows that were being implemented wrong and needed a tidy cleanup before our group could publish the final block diagram design. You will see below that our Final Block Diagram reflects all those changes. 



<br/>

![Block Diagram-314-Team-307](https://user-images.githubusercontent.com/122499832/233797627-bc5bec8d-46c7-45b3-86f6-a193508a950d.jpg)

The Block Diagram is essential for our electrical system design and clearly illustrates which subsystem belongs to who. Each group member is in charge of testing and debugging in order to verify that the subsystem works and is prepared to be tested for the completed subsystem. For Team 307’s approach on our block Diagram, we organized the important architecture of our hardware and displayed how the systems are interconnected for working functionality. Included in this Diagram is our ESP32 WiFi modulator which allows for RX/TX communication which allows for sending and receiving information, our Humidity Sensor, and our temperature sensor which meets the criteria for this course to include two serial sensors, the MicroController and the Motor/Motor Driver which fulfills the actuator requirement for our design. To see the team's original block Diagram please refer to the **Master Appendix** and scroll to **Appendix F: Original Block Diagram**.


---
# Component Selection
---

<br/>

## Approach to Part Selection


Group 307 read the class projects course requirements very closely to ensure that we were not looking at parts that were deemed unusable for our electrical design. While doing research on components, we focused on parts that incorporated detailed datasheets as well as immediate accessibility. With current microchip and manufacturing issues across the globe we wanted to be certain that we had immediate access to start testing and debugging our current concept selection.

To begin comparing possible components that would be necessary to create each system for our project we would first consider components that we worked with in class. Since we are familiar with them, having had to create working code and circuitry for previous assignments these would set our standards for other components. We first listed out the pros and cons of the parts we used in previous assignments then we would look for similar components that would offer solutions to the cons we had listed. For subsystems that required a part not used in a previous assignment we would choose a few components that each had different strengths and weaknesses.  

Once our possible choices were listed out we then chose the best option prioritizing ease of use, such as a package size manageable enough to hand solder as well as familiarity working with the component. 


<br/>

## HIH6030 Humidity Sensor

<br/>

![Humidity sensor component](https://user-images.githubusercontent.com/122499832/221627479-56b7943b-d2bd-48f0-9f3b-e0fa425c0626.PNG)

<br/>
 The HIH6030 Sensor is manufactured by Honeywell and has the ability to sense humidty and temperature, however, our group will only be implementing the humidity sensor for this component. Below are a few reasons why we pursued with this sensor for our system.
 
 * I2C output
 * Humidity snese range is between 0%-100% with a 4.5% accuracy
 * voltage supply is 2.3V-5.5V
 * Surface mountable
 * Readily Available


<br/>

## TC1047VNBTR Temp Sensor

<br/>

![Temp Sensor component](https://user-images.githubusercontent.com/122499832/221627556-d35612f9-6038-49d7-8d84-1cfa175ce3a7.PNG)

<br/>

The TC74 temperature sensor manufactured by Microchip is a serial sensor that measures the temperature. it can measure temperatures between -40C to 125C and outputs Data using I2C. the voltage supply range for this sensor is a minimum of 2.7V to 5.5V. This sensor will be surface mounted onto the PCB board.

<br/>

## PNN7RE08JD Motor

<br/>

![Motor Component](https://user-images.githubusercontent.com/122499832/221627503-67d84ce6-249a-46b1-a6ac-d04b53e3858f.PNG)

<br/>

Manufactured by NMB Technologies, is a standard DC motor with an RPM rating of 16364 RPMs. We went with this motor specifically due to its long shaft, this allows our group to easily mount with the internal spray bottle. The voltage 


<br/>

## IFX9201SGAUMA1 Motor Driver

<br/>

![Motor Driver Component](https://user-images.githubusercontent.com/122499832/221627518-9875718c-5160-4cdd-a185-358a5cafe405.PNG)

<br/>

This motor driver is already readily available to us. We did not need to worry about order times and so we could already start working and troubleshooting with this device. Due to already using it for a previous assignment, we are already familiar with how it operates and works. It meets our requirements and is able to complete the desired function needed for our design.


<br/>

## MAX5033AASA+ Switching Voltage Regulator

<br/>

![Switching voltage](https://user-images.githubusercontent.com/122499832/221717772-09a840c1-6111-45c4-b536-fdb6c7ce73a4.png)


<br/>

The class requirement needs us to  use a switching voltage regulator. This one matches this requirement as well as is in the proper voltage range of 3.3V. It also will provide enough amperage for running all of our schematics.

<br/>
## Component Selection Assignment

For an in depth exploration of all our initial choices for components, please refer to Appendix D in the Appendix section.


<br/>

---
# Power budget
---

<br/>

## Current Power Budget


Each of our components was easily accessible from the distributors purchasing sites and provided all the information we needed to conduct a power budget table. For our group to be certain that the components that we had selected will indeed work with our electrical design, we created a power budget for the overall system which displays usage across voltage, amps, etc.

<br/>

![updated power budget](https://user-images.githubusercontent.com/122499832/235246667-4a5fab0e-642d-444c-ab76-3b8614dc8dbf.jpg)

<br/>

We calculated both the maximum power draw as well as the power draw under normal operating conditions. These calculations were used to choose a power supply that could operate our system at max power for an hour. It was also used to ensure each power rail could safely  support the current being drawn by each component.

---
# MicroController Selection
---

<br/>

## PIC18F27Q10 Microcontroller

Our group 307 sat and researched multiple chips that would work best for our electrical design and we determined that the PIC18F27Q10 Microcontroller was the best fit. we decided to utilize and interpret this microcontroller based on the following attributes the microcontroller has.

  * Supply voltage ranges 1.8V-5.5V
  * inexpensive compared to other microcontrollers
  * 28 GPIO pins
  * Max GPIO pin current is 50mA
  * Supports esternal interupts
  * Surface mount and through hole packages
  * Works with MPLAB and Microchip Code Configurator

 This microcontroller satisfies project-specific requirements and the Microcontroller also comes with the adequate data sheets needed to supply our group with the necessary information to function our group design properly. there is plenty of sample code available via Microchip as well as other trusted resources.

<br/>

![Microcontroller selection](https://user-images.githubusercontent.com/122499832/221628253-5316b9a2-1428-466b-bac0-d7ffb6f6fb1c.PNG)

<br/>

This is an overview of our Micrcontroller selection, to see the whole assignment of all three of our initial selections, please refer to the master appendix and scroll down to **Appendix E**.


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

---
# System Verification
---

![Final VOC](https://user-images.githubusercontent.com/122499832/235246699-42ed309a-8747-4eb6-b522-8cb0795b05ab.jpg)

<br/>

---
# Lessons Learned
---

There are many lessons learned that group 314 had gained by the end of this semester and completing our final project. Some of these lessons would have been great to know about prior to the class starting and deciding how our group would approach our project. Below is a list of our ten mos important lessons that we have learned throughout this semester.

1. Dont buy a MacBook for an engineering course.

2. Order more parts than you think will be enough, we thought we ordered just enough and we were wrong.

3. The basic skills on how to solder and wearing protection.

4. Reference pin numbers and label signals when designing block diagrams.

5. Utilize as many parts as possible from room 109.

6. Wear protective gear when using the solderer oven.

7. Finish assignments before the due date to give us more time to troubleshoot.

8. Understand the course requirements, read what we are allowed to use before getting something before its to late, and have to go do more research.

9. Trying to make a simple project definitely did not go as simple as we wanted it.

 10. Creating a PCB design is very time-consuming and small errors can set you behind or call for a redo because the PCB becomes unmanufacturable.

These are the top ten lessons that our group felt were learned throughout the semester. There definitely been more learning curves than what were listed but we felt that these were the lessons that stood out the most.


<br/>

---
# Recommendations For Future Students
---


EGR 314 is just as an emotional roller coaster ride as EGR 304 is only you more prepared for the crushing feelings this time around. There have been many moments where our group felt that our project was running smoothly and there were times that our group felt like switching majors. With that being said, our group came together and discussed a list of recommendations for not only future EGR 314 students but for 304 students as well. This list is meant to be viewed as a recommendation for it is based on opinions and our group's view of how the course went for us.

1. If you have an option between Cadence or Kicad in your 304 course, do yourself a favor and do not use Kicad and force yourself to go through the pain of Cadence. This will benefit you greatly because you will have a better idea of the ins and outs of cadence than we did.

2. Give yourself some time to understand MPLabX, it is a very touchy software and can be tedious many times when using it for different Microcontrollers.

3. Following up with MPLabX, there is not enough time to get a full grasp of MQTT and Thotty. We recommend watching educational videos before getting to this segment of the course to understand micropython and how these two programs interact with each other.

4. Communication is gold, create a group text immediately and make sure everyone is aware of what is due and what needs to be done. Not only have communication between your group members but also communicate with the Professor and TAs, unfortunately, information and requirements change frequently and even if you didnt know something or weren't communicated properly, expectations will be held.

5. Utilize as many resources as you can from the classroom, everything you need for testing and debugging is there. If you can't be at the campus as much as you can, invest in tools for your home. Chances are high that you will need to solder or use a voltage meter or need a power supply and going back and forth can be overwhelming.

Our group hopes that this list provides usefulness to future students of EGR 314 as well as 304. As they all say, This too shall pass.


<br/>

---
# Master Appendix
---

[Appendix](https://team307.github.io/Appendix/)