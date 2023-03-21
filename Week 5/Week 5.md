# Workshop 5: Functional Analysis & Allocation 

Relevant lecture: Week 5: Conceptual Design 

## Introduction 

An essential activity in early conceptual design is the development of a functional description of the system. **Functions** refer to specific or discrete actions (or series of actions) that are necessary to achieve a particular objective. Such actions may ultimately be accomplished using equipment, software, people, facilities, data, or various combinations thereof. However, at this point in the system’s life-cycle (conceptual and preliminary design) the aim is to specify the ‘whats’, and not the ‘hows’. 

**Functional Analysis** is a process used to translate system level requirements into detailed functional and performance requirements. It is an iterative and recursive process that responds to the ongoing activities of both the requirements and design loops, allowing the identification of functional issues to prompt the re-examination of higher-level requirements or lower-level component selection. The result of functional analysis and allocation is the generation of the Functional Architecture, which is used during Design Synthesis to construct and configure various design alternatives that satisfy the system’s functional and performance design criteria.   

## Activity 1: Reverse Engineering 
In groups of three, reverse engineer an automatic teller machine (ATM). You should begin by considering what high-level functions an ATM performs and why it performs them. You may also want to sketch out a typical real-world ATM’s physical system architecture (i.e., the products that constitute the ATM including cash storage, keypad, screen, card slot), and identify all of its external interfaces; its internal interfaces are not as important at this stage. Thinking about an example ATM design might help you identify functions that you may have otherwise missed. 

 1. Consider the physical realization of the ATM and draw up a systems architecture for a typical ATM (hole in the wall) with functions allocated to subsystems.   
 2. Establish a functional description of an ATM.  You should get a function flow block diagram for the ATM function. 
 3. Choose a key function of the ATM and consider concept generation for this function.  Expand this out to a system architecture for your system.  
 4. From the insight gained in the concept generation step, can you propose an alternative systems architecture for the function of the ATM.  



## Activity 2: Functional Analysis 
You are part of the future technologies team at ACTEW tasked with designing the support infrastructure for electric vehicle (EV) use in Canberra. ACTEW has negotiated with the ACT government and relevant stakeholders to install five prototype EV charging stations in the Canberra Centre parking garage; and two super charger stations (extremely high charging rate) outside Akiba on Bunda Street. ACTEW also wants to provide EV drivers with the capability to install private EV charging stations in their garages. 

Personal EV chargers typically require a single phase supply supporting up to 7.4 kW of power at a nominal supply voltage of 240 V AC (alternating current), and can potentially fully charge an EV within eight hours. The chargers intended for use in parking garages are required to charge cars more rapidly (between 1 and 2 hours for a full charge), and require a 3-phase supply to draw up to 25 kW of AC power. The super chargers intended for Akiba draw up to 120 kW DC (direct current), and—depending on the vehicle—are capable of charging an EV from zero to full in approximately 10 minutes.  

ACTEW will purchase chargers from commercial vendors. Your task is not to design the actual chargers. Your task is to design the charging stations. You decide that the best way to do this is to first analyse each station’s functionality. 

In groups of three: 
* Design the functional architecture for one of the three types of charging stations (parking garage stations, super charger stations outside Akiba, or private charging stations). Include all applicable interfaces (internal and external) and consider what kind of technology may be required to implement the stations. It may help you to sketch out a potential physical architecture of the station so you don’t forget anything. 
* For your choice of system undertake a concept generation process for the key functions.  Generate at least two concept sketches.  
* Select a concept sketch and expand this into a system architecture with functional allocation.  


## Learning Outcomes 

1. Identify, analyse and objectively resolve design trade-offs 
2. Understand different types of requirements, constraints, and assumptions encountered during systems design 
3. Describe systems in terms of their functionality instead of their components 

## Additional Reading   

NASA Systems Engineering Handbook 

  * Chapter 4: System Design (pages 40-52) 

NASA Systems Engineering Handbook 

  * Appendix F: Functional, Timing, and State Analysis (pages 285-288) 

US DoD Systems Engineering Fundamentals 

  * Chapter 5: Functional Analysis & Allocation (pages 45-55) 




