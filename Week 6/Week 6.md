# Workshop 6: Conceptual Design 

Relevant Lecture: Week 06 - Conceptual Design

## Announcements:

* Reflection 2 due date has been extended to Tuesday 2nd April - 9:00 AM.
* [Assignment 2]() has been released (Due on 15 April 2024, 9:00 AM).

# Introduction 
Design synthesis is a creative activity that transforms a system’s **_functional_** decomposition into a **_physical_** architecture (or **_system_** architecture for conceptual systems). Where functional architectures describe **_what_** the system must do, physical and system architectures describe **_how_** the system will do it. 

Determining the best possible solution for any particular problem has the potential to be very complicated, especially if the different solutions have little in common. Fortunately, it is possible in most cases to objectively evaluate each concept’s ability to satisfy the system requirements, allowing to perform a detailed **_concept comparison_**.  

Everything about the different concepts can be different… except for one thing: the set of concept-independent system requirements (defined in the SRS) which they all aim to satisfy. Concept comparison therefore depends entirely on the stakeholder’s needs and expectations, and their relative importance. Most of the time it comes down to **_cost, schedule, and complexity_**.

# Scenario
Asparagus is a high value crop horticultural crop for which the harvesting is almost entirely unautomated. Asparagus spears grow quickly (50-100mm per day in good conditions) and must be harvested when they are 225-275mm high.  They grow unevenly from neighbouring plants over a period of 70 days and cannot be harvested in a single “take all” harvest process as is most common in agricultural automation.


<img width="722" alt="Screen Shot 2023-03-26 at 1 18 32 pm" src="https://user-images.githubusercontent.com/125527438/227751683-5321e8f9-49ba-4ce4-b18b-427cdded23d5.png">


Present practice has a person walking the asparagus line each day, manually selecting the stalks that are of the correct height and cutting only these stalks.  The cost of labour is estimated at between $6,000-$8,000 per hectare, roughly 25% of the production cost of asparagus.  A moderate producer in Australia will have around 250 hectares of asparagus under cultivation and be paying around $2M per year in harvesting costs.  

The project scope is to consider automation or partial automation of asparagus harvest.    

The requirements for the project have been identified to be:   

### R1: Accuracy 

| ID | Description | Importance |
| -- | -- | -- |
| R1.1 | The harvester system shall be able to identify spears between 225 and 275mm | 3 |
| R1.2 | The harvester system shall be able to identify spears with diameters between 10 and 18mm | 3 |
| R1.3 | The harvester system shall be able to identify between erect spears and bent-over spears (maximum of 10% curvature) | 2 |
| R1.4 | The harvester system shall be able to identify between healthy and diseased spears. | 2 |
| R1.5 | The harvester system shall be able to dispatch bent-over spears, diseased spears, and weeds to the furrow. | 1 |
| R1.6 | The harvester system shall be able to identify between mature spears, immature spears, and emerging buds. | 1 |

### R2: Recovery Rate 

| ID | Description | Importance |
| -- | -- | -- |
| R2.1 | The harvester system shall have a spear recovery success rate of greater than 90%, including spears damaged in harvesting that will be discarded in future days | 2 |
| R2.2 | The harvester system shall harvest 250 hectares in at most 12 hours. | 1 |

### R3: Operation 

| ID | Description | Importance |
| -- | -- | -- |
| R3.1 | The harvester system shall be able to operate in all weather conditions (including when the furrows are wet and muddy). | 2 |
| R3.2 | The harvester system shall be able to operate in varying lighting conditions. | 1 |
| R3.3 | The harvester system shall be sturdy, reliable, and easily maintained. | 2 |

### R4: Cost 

| ID | Description | Importance |
| -- | -- | -- |
| R4.1 | The harvester system operating costs must be less than $2M per year. | 2 |


# Functional Decomposition
The systems engineering team has provided the following functional decomposition for the system.  

![Classify SubFunction (1) drawio](https://user-images.githubusercontent.com/125527438/227752077-7cbdbf31-fbd0-4e7b-ae78-60bf5d14b569.png)

In your groups: 

1. Work in groups to brainstorm different concept designs for the functional architecture.  

    * Start by identifying the key functions in the architecture.  Choose at most 3 functions to brainstorm.
    * Brainstorm a possible solution to these functions.  
    * From this brainstorming process - generate at least two different concept sketches. Try and get concept sketches that are quite different.  

2. Use the concept comparison process with the evaluation matrix to formally select a concept.    
   * Choose at most 5 of the requirements to score with the star method.

3. Work from this starting point to develop a systems architecture.    
    * Start by identifying the subsystems and components of the system.
    * Do functional allocation to identify the primary interfaces between subsystems.  You may identify additional subsystems during this process.  Make sure that all functions in the system are allocated to subsystems or across multiple subsystems.  

4. Identify secondary interfaces between the subsystems.  These are usually dependencies (physical, process, etc) introduced by the concept sketch due to the technological nature of the solution that are not directly captured by the functional decomposition. 


## Discussion Results

Please submit/upload your discussion results to the Padlet using the following links:
* [Tuesday Session](https://anu.padlet.org/u6554505/systems-engineering-tuesday-week-6-w0zyrh2mq3cryckt)
* [Friday Session](https://anu.padlet.org/u6554505/systems-engineering-friday-week-6-j1ggbmo5y6ueu5og)


# To Do List
1. Work on Reflection 2.
2. Work on Assignment 2.
3. Work on your Group Project.
4. Enjoy your Teaching Break (not studying break 🥲).


# Learning Outcomes 

1. Identify and analyse the various phases in a system's life-cycle, and demonstrate an understanding of the importance of considering a system's lifecycle early during the design process.
2. Identify, analyse and objectively resolve design trade-offs.
3. Understand different types of requirements, constraints, and assumptions encountered during systems design.
4. Describe systems in terms of their functionality instead of their components.

# Additional Reading 

* **NASA Systems Engineering Handbook**
  * Chapter 5: Product Realization (pages 71-81) 
* **US DoD Systems Engineering Fundamentals** 
  * Chapter 6: Design Synthesis (pages 57-63) 

