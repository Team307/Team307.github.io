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
- [Block Diagram](#block-diagram)
- [Component Selection](#component-selection)
- [Microcontroller Selection](#microcontroller-selection)
- [Master Appendix](#master-appendix)

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

Our team strives to have a successful product, we believe that with concise communication and dedication to hard work, and schedule commitment, we can achieve our goals.

A product that meets our stakeholder’s expectations, working with no bugs or other interruptions that can hold the product from being a complete product.
Not only receiving an A on the project but also being able to understand and explain fluidly how the system works.
Building a professional relationship with group members and faculty through thoughtful questions, respectful answers, and clear communication.
Expanding our individual knowledge and skill sets through peer guidance and teaching. We will allow ourselves to not only be available for teaching but to be taught.
Holding ourselves and our team members accountable to the tasks assigned and the standards set forth in this charter. This will create an environment where we are working together as peers toward our common goals.

<br/>

## Product Mission Statement

**To develop an interactive system that reacts to environmental changes and be displayed at the ASU showcase while achieving our course objectives and requirements.**


Our group believes we have knowledgeable team members and strong-minded individuals who will stay true to the mission statement and follow the team charter religiously. With both these strong Charter and statements, we believe that we will have a successful product for our professors and our stakeholders. For the rest of the sections in our team organization assignment, refer to Appendix A: Team Organization on the Appendix Page.


---
# User Needs, Benchmarking, and Requirements
---

<br/>

## Summary

_The User Needs assignment was the kick-off to our group's brainstorming for this project, we did not know entirely what our project will end up being but came up with ideas shortly after understanding what the project description was asking for out of us. First, we invested our time in the project description to truly understand what we can and cannot have included in our design. Afterward, we individually did research on similar products and created a VOC chart. We found products that were like the theme of our project was and looked at positive and negative reviews and pulled out what was explicitly and latently being called out in the review. This helped our group weigh out the important needs for what our users will be expecting or should expect._

_Next, we created a Jam Board of sixty needs that our product should have to be a successful product. Each of us jotted down roughly 12 to 15 needs each. After we had the sixty needs, we then sought to organize the needs by color; Blue being the most important need for our design, green being a medium need, and yellow being the lowest need for our group's design. Before we rated our needs, our group compared our needs to what was being called out in VOC reviews and reviewed which of our needs stood out the most of what users are asking for in products. After we organized them in groups by color, we then had our user needs that we felt needed to be implied to our project and design. Our design will be assessed over the aspects we provided in our user needs in many ways. We will approach each assignment and step throughout the building process by looking at our user's needs and verifying that we are following what is important to the users to create a successful design. After each completion of each part of this product, we will refer back to our user needs and ask ourselves the following:_
- _Are we satisfying the needs in our design?_
- _Does this meet the course requirements?_ 

<br/>
  <br/>

## Introduction

The Innovation Showcase is an event held at Arizona State University for upper divisional engineering students that showcase their final project to their professors and stakeholders as well as other students that visit and public. The main focus of this event is to explore what engineering students have developed over the course of the semester and see how they apply the knowledge they have gained and infuse it into a functional design. Specifically for Engineering 314 students, their project is to produce a system that interacts and corresponds with the environment and is required to use serial sensing and actuation. Another requirement is that their project/design must broadcast their environmental data using WiFi using the MQTT protocol. Students must include a design that senses at least two environmental conditions and two separate serial sensors. It is also required in the plan to include at least one motor controlled by a motor controller over I2C or SPI-based protocol. The working product of the engineering groups will be presented at the showcase on April 28th, 2023, and will be evaluated by professors for correct functionality as well as meeting the course requirements.

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

-	Can we improve the battery life and reduce the amount of battery recharge?

-	Are there better materials that can be applied to the product other than plastic while still remaining cost-effective?

-	Can we improve on the customization of the software so the user can choose what environmental condition to focus collecting data on?
  
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

# Block Diagram
---

<br/>

## Summary


_ this is where are summary will go for the Block Diagram

---
# Component Selection
---

<br/>

## Summary


_this is where we will add a summary

---
# MicroController Selection
---

<br/>

## Summary

_this is where our summary will go



---
# Master Appendix
---

[Appendix](https://team307.github.io/Appendix/)