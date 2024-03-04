# Workshop 3: Requirements Analysis
Relevant lecture: L02 and L03: Stakeholder needs and Requirements Specifications

## Introduction
Requirements analysis is fundamental to the systems engineering process in that it identifies, evaluates, and translates customer needs and expectations into functional and operational system requirements. Put simply, it is the process used for determining what the customer truly needs.

A key output of requirements analysis is a document called a System Requirements Specification (SRS). The SRS contains a set of concept-independent system-level requirements that define explicitly what the customer needs. It is solution agnostic, which means it does not in any way assume a particular solution or concept. In many cases, it forms a contract between developers (engineers, project managers, etc.) and the client, defining explicitly what the developers’ obligations are to the client with respect to the delivery of a solution, as well as the client’s obligations to the developers.

Requirements expressed in the SRS should indicate whether a provision is mandatory or
non-mandatory. The specific wording of a requirement in the SRS does this.
* Use **must** to express provisions that are mandatory.
* Use **shall** to express provisions that are required to meet validation requirements of the client (requirements that must be met in order to satisfy the contract)
* Use **should** and **may** to express non-mandatory provisions or requirements that are desirable but do not necessarily need to be satisfied
* Use **will** to express provisions that will be supplied by the customer.

The cost of mischaracterizing the customer’s needs can be expensive, especially if an error is discovered after conceptual design. Requirements analysis is therefore arguably one of the most important phases in the system’s life-cycle.

## Activity 1: Good and bad requirements
Discuss what’s wrong (if anything) with the following requirements:
1. The electric vehicle (EV) must be capable of travelling faster than any other vehicle in its class.
2. The energy storage system shall store enough energy to power the EV’s motor for four hours of continuous driving.
3. The EV’s chassis shall minimise aerodynamic drag to maximise performance.
4. The EV’s user interface must be intuitive and enjoyable.
5. In the event that the EV’s auto-pilot system experiences a critical failure, the EV will immediately enter a safe state and alert the driver to resume manual control. Furthermore, if the EV’s driver monitoring system detects that the driver has fallen asleep, it will alert them to resume manual control.

In small groups - workshop good requirements (possibly including derived requirements) for the five requirements. 

[Click Here to submit your answers](https://padlet.com/imanhosseini/system-engineering-workshop-uvv29yk8ndd6748i)

## Activity 2: Writing good requirements.
What might be some of the requirements associated with an emergency alert system for seniors? Emergency alert systems are often made as a pendants and worn by seniors in order to call for help should they fall or need immediate care in their homes. 

<img width="364" alt="Screen Shot 2023-03-10 at 11 30 25 am" src="https://user-images.githubusercontent.com/125527438/224192515-d5196bd1-297a-4347-9f10-3da53dec67df.png">



In the full group workshop 3-5 needs in tabular form.

| **ID** | **Description** | **Importance** | **Source** | **Validation** | **Notes** |
| --- | --- | --- | --- | --- | --- |
| N1.1 | Short Description of need | One of Desirable, Highly desirable, Essential. | Most concerned stakeholder | How would this need be validated | Any Additional Notes |

Now split into small groups write requirements for each need.

Remember that you may need to write several requirements for a single need. Sometimes, you may capture aspects of several needs in a single requirement.

Once you have done this, come back together in a group and present one of your requirement statements to the rest of the class. 


## Activity 3: Web Content Accessibility Guidelines 2.0 Standard
Web accessibility is a crucial aspect in delivering an accessible and inclusive online environment for all users. The Web Content Accessibility Guidelines (WCAG) standard was developed to provide a comprehensive set of guidelines for making web content accessible to people with disabilities and older people, and people who cannot use, or struggle with, digital services. 

WCAG 2.2 is the current version, released by the Worldwide Web Consortium (W3C) in October 2023. Compliance with WCAG 2.2 is achieved by satisfying the **Success Criteria** listed within the guidelines. For Australian Government agencies, web content needs to meet WCAG level AA.   

Guidance is presented in layers including overall **principles**, general **guidelines**, testable **success criteria**, and a collection of **sufficient and advisory techniques**, and documented failures, with examples, additional resources and code.

* Navigate to WCAG 2.2: [Web Content Accessibility Guidelines (WCAG) 2.2 (w3.org)](https://www.w3.org/TR/WCAG22/)
* How to meet WCAG (Quick Reference): [How to Meet WCAG (Quickref Reference) (w3.org)](https://www.w3.org/WAI/WCAG22/quickref/)

## The Scenario: 
A health and nutrition company has hired your design team to design a website that provides users with personalised recipes based on what ingredients they have. As the cost of living goes up, people are coming up with new and creative ways to save money – one way is to cut back on eating out and instead get creative at home trying new recipes with groceries and other fresh produce.  

Split into small groups and write requirement statements for the following three need statements that reference the WCAG 2.2 success criterion appropriately. Pick a maximum of 4 - 5 success criteria to develop your requirement statements against. 

| **ID** | **Description** | **Importance** | **Stakeholder** | **Notes** |
| --- | --- | --- | --- | --- |
| N1 | The website is intuitive and simple to use | Essential | The company | People from all ages and backgrounds will be using this website, so the website should be easy enough for anyone to interact with |
| N2 | The website generates revenue | Highly Desirable | The company  | The website must be hosted online, which will incur a monthly or annual fee. This cost should be offset by some revenue, but this should not take away from the user experience  |
| N3 | Video instructions on how to follow the recipes | Desirable | The company | Visual and audio instructions are more inclusive ways for more people to access and use the website |


## Activity 4: Requirements for Asparagus Harvest
Asparagus harvesting is a time-consuming manual labour process and several companies around the world have considered the development of agricultural systems to automate the harvesting of asparagus.

<img width="1000" alt="Screen Shot 2023-03-10 at 11 32 22 am" src="https://user-images.githubusercontent.com/125527438/224192639-eb945de8-06b2-4967-9a77-866f8a9ee798.png">


Consider the following list of requirements determined by a design team for the development
of an asparagus harvesting machine.

Create a Requirements Breakdown Structure for the requirements. You should have no
more than 5-7 requirements at any level of the hierarchy. You may add requirements if you
feel that a layer of the hierarchy requires a high level requirement underwhich you can
capture the specific requirements that are written. 


* R1: The harvester shall operate autonomously along a row of asparagus.
* R2: The harvester shall identify spears with a length above ground of 225-275 mm
* R3: The harvester shall cut and deposit bent spears in the furrow.
* R4: The harvester shall harvest at a rate of 1.5m/s along a row of asparagus.
* R5: The harvester shall cut spears at a depth of 50 mm below the surface of the ground.
* R6: The harvester shall be operatable by a single human.
* R7: The harvester shall cut and deposit healthy erect spears in the harvest bin.
* R8: The harvester shall differentiate between healthy spears and diseased or insect ridden spears
* R9: The harvester shall not damage immature spears and emerging buds.
* R10: The harvester must operate without risk to human operators.
* R11: The harvester shall identify spears with diameter 10-18 mm
* R12: The harvester shall differentiate between erect spears and spears that are bent (>20cm curvature).
* R13: The harvester shall cut and deposit diseased or insect ridden spears in the furrow.
* R14: The harvester shall differentiate between mature erect spears and immature spears and emerging buds. 



## Learning Outcomes
1. Understand different types of requirements, constraints, and assumptions encountered during systems design
2. Gather, analyse, and communicate requirements to technical and non-technical audiences


## Additional Reading
US DoD Systems Engineering Fundamentals
* Chapter 4: Requirements Analysis (pages 35-45)

## Discussion Results
The summary of your discussions can be accessed below:
