***

<p align="center"><strong>ARIZONA STATE UNIVERSITY</strong></p>

<p align="center"><strong>ENGINEERING 314 - DANIEL AUKES</strong></p>
  
<p align="center"><strong>Weather Based Device Project</strong></p>

<p align="center"><strong>Team 201</strong></p>

<p align="center"><strong>Aiden Lynch, Finnton Wentworth, Richard Kovalcik, Glen Stevens</strong></p>

<p align="center"><strong>Submission Date: 1/23/2023</strong></p>

<p align="center"><strong>Team Organization:</strong></p>

The following sections will only cover the Team Charter and Mission Statement. The rest of the Team Organization can be found in **Appendix A: Team Organization**

**Team Charter:**

Shortly after we assembled our team and got to know one another better we decided to come up with our team charter. In this session, we decided to start talking about the initial goals and ideas for this project. We wanted to be able to determine our metrics of success to which we could come back to at the end of the semester and see if we achieved our goals. We each discussed our goals and noticed a lot of similarities between our ideals for this project. After careful consideration, we decided upon the following team charter.

_“With the presentation of our projects at the Innovation Showcase, our team is looking to create a professional deliverable that has a strong visual appeal to judges. We hope to develop strong skills in tools used by engineers currently in the workforce, such as GitHub, Cadence, and the various other software that will be utilized in this class, and to display our accomplishments using these tools in a clear way. By creating a product that is thoughtfully designed, we hope to hone our abilities as engineers and demonstrate our capabilities to industry members at the innovation showcase.”_

**Mission Statement:**

After we did the Charter, we decided to move on to the mission statement and decide our primary goal for this project. We took some of our ideas from the Team Charter and attempted to condense them into a singular statement. A problem we ran into was that we were not fully aware of what the scope of the final project would be so made some assumptions, based on project requirements and initial design ideas. After using the provided references we decided on the following mission statement:

_“To create an effective product that will accurately and quickly collect weather-based data.”_

## User Needs:

Viewing market options in weather sensor equipment allowed our team to perform benchmarking for our project concepts and generate user needs by analyzing real product reviews. Our team looked at five different available commercial solutions generated from Amazon searches and their product reviews to generate a list of needs from the customer’s own words. Both positive and negative reviews were viewed to determine what features in a weather sensor were desired and what should be cut or was missing from most products. 

**Need Generation and Sorting:**

Reading user reviews with the perspective of generating project features was most important to us. Since the scope of the project was fairly undefined with the exception of budget and the overarching requirements listed for the course, the team viewed amazon reviews, looking for requested features, as well as what the users viewed as extraneous on the products we reviewed. Looking for explicitly listed needs, as well as digging deeper into the wording of the reviews to see latent needs from the users. From these reviews, we generated a list of 103 needs, as seen in **Figure A**. 



<p align="center">Figure A: Full list of Generated Needs</p>

From this full list, we sorted these needs into six different categories: Hardware, Software, Interactivity/User Experience, Customization, Manufacturing, and Safety. These categories were chosen based on the aspect sections we included in our Product Requirements Document which was written following the review of our sorted user needs. Shown below in **Figure B** is our sorted list for the Hardware section, and the full list of sorted needs can be found in Appendix B: User Needs and Benchmarking. 	


<p align="center">Figure B: Hardware category of sorted user needs</p>
  
From these sorted needs, our team ranked the needs into three separate weights, with one to three stars denoting importance. The weight of a specific need was chosen by our team, with the greatest ranking given to needs that were generated from project requirements and effective functionality, as these were non-negotiable features for our final deliverable. Without including the three star needs, our project would fail to meet stated requirements or would lack qualities that would make it a functional or usable product. Below in **Figure C** is the evolution of the Hardware section, now ranked. 

<p align="center">Figure C: Ranked List of Hardware Needs</p>
  
Now with our generated list of user needs sorted and ranked, our team looked to characterize and formalize the project and needs through the construction of a Project Requirements Document, which would provide the background, objectives, and potential stakeholder experiences with our project. Although we felt that our main stakeholders ranged from Industry members to hobbyists, we chose to imagine the project’s use from the perspective of a field engineer as well as a student for our use case scenarios. 
  
Our list of sorted needs were kept in their sorted categories for the PRD, and converted to project aspects for reviewing final project success. These were given priorities based on the weight assigned to them during the ranking process, although since the scale ranged from P1-P10 instead of 1-3 stars, we were able to create more depth within our aspect ranking. 
  
The full PRD can be found in **Appendix C: Project Requirements Document**


## Design Ideation:

**Idea Generation:**

We initiated our design ideation by generating one hundred design ideas. These ideas can be viewed below in **Figure D.**

<figure class="image">  

<div style="text-align: center">  

<img src="media/100Concpets.jpg" width="50%"><br>  

</div>

<p align="center">Figure D: 100 design Ideas</p>
  
Idea Sortation and Ranking:
Once we had generated our 100 design ideas, we proceeded to sort them into three categories. These categories being miscellaneous, weather balloon, and drone which can be viewed respectively in **Figure E**, **Figure F**, and **Figure G**. After this process, we ranked our ideas vertically from the most to least practical. A few of the aspects we looked for in practicality were ease of implementation, feasibility, and requirement satisfaction. 

<figure class="image">  

<div style="text-align: center">  

<img src="media/MiscConcpets.jpg" width="50%"><br>  

</div>
  
<p align="center">Figure E: Miscellaneous</p>

  
<figure class="image">  

<div style="text-align: center">  

<img src="media/WeatherBalloonConcpets.jpg" width="50%"><br>  

</div>
  
<p align="center">Figure F: Weather Balloon</p>
  
<figure class="image">  

<div style="text-align: center">  

<img src="media/DroneConcpets.jpg" width="50%"><br>  

</div>

<p align="center">Figure G: Drone</p>


**Concept 1: Weather Balloon**

Aiden Lynch was in charge of the Weather Balloon design concept. The fundamental idea is that we have a system attached to a balloon that will be able to sense multiple different environmental factors at different altitudes. See **Figure H** below for the picture of the figure and for a description of the device.

<p align="center">Figure H: Weather Balloon</p>

We have the balloon that will raise the device up in the sky to collect readings. We are discussing whether to use an actual weather balloon, a helium balloon, or a biodegradable balloon to limit waste. We have a strong string/rope that will connect the balloon to the top of the box whether it be on a hook or another method with a closed top. We have two currently undefined weather-based sensors that will be connected to the PCB inside of the unit inside the box. Connected to the top we have a bidirectional motor that will be the actuation and will be in charge of cutting the rope to bring the device back for the users. We also have attached a GPS tracker that will be utilized through wifi to allow us to receive the readings while also being able to track the balloon. Some benefits is that we can use the string at the bottom to accurately measure a variety of different heights by increasing the sting length. Another pro is that it is a very visually appealing project and very easy to understand the fundamental idea of how it works. The biggest con we believe is retrieval of the box if it gets too high and the non-wasting of balloons during testing.

**Concept 2: Water Buoy**

Finnton Wentworth visualized concept #2, a floating water based sensor array. The device would be able to collect a physical sample of water as well as transmitting various environmental data. 


<p align="center">Figure I: Water Buoy </p>

Design concept #2 looks to act as a deployable water quality  and condition sensor. The user would place the buoy in a body of water to collect and transmit data based on the attached sensors. The main point of actuation is in a sample collection bay door, which sits under the surface of the water. Once the door closes, the water sample can be collected later when the device is retrieved for lab analysis.

The microcontroller and batteries will be stored in a sealed chamber within the main housing of the device, with wires running out connecting to the motor, lights, and external sensors, and sealed to prevent water from damaging the electronics.. The body of the device will be constructed from some waterproof material, most likely printed PLA. One major risk of this design is damaged to the sensitive components due to moisture or water. Some inexpensive moisture control strategies would be including silica gel packets within the electronics housing. 


**Concept 3: Drone**

Glen Stevens was in charge of the Drone kit design concept. The idea was to create a kit that could be attached to a drone that would then read weather conditions as the drone flew around. See **Figure J** below for a model of the concept.

<p align="center">Figure J: Drone Kit</p>



  
## Appendix A: Team Organization

## Appendix B: User Needs and Benchmarking

## Appendix C: Project Requirements Document
