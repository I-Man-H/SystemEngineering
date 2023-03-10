# Workshop 3: Requirements Analysis
Relevant lecture: L02 and L03: Stakeholder needs and Requirements Specifications

## Introduction
Requirements analysis is fundamental to the systems engineering process in that it identifies, evaluates, and translates customer needs and expectations into functional and
operational system requirements. Put simply, it is the process used for determining what the customer truly needs.

A key output of requirements analysis is a document called a System Requirements Specification (SRS). The SRS contains a set of concept-independent system-level
requirements that define explicitly what the customer needs. It is solution agnostic, which means it does not in any way assume a particular solution or concept. In many cases, it
forms a contract between developers (engineers, project managers, etc.) and the client, defining explicitly what the developers’ obligations are to the client with respect to the
delivery of a solution, as well as the client’s obligations to the developers.

Requirements expressed in the SRS should indicate whether a provision is mandatory or
non-mandatory. The specific wording of a requirement in the SRS does this.
* Use **must** to express provisions that are mandatory.
* Use **shall** to express provisions that are required to meet validation requirements of the client (requirements that must be met in order to satisfy the contract)
* Use **should** and may to express non-mandatory provisions, or requirements that are desirable but do not necessarily need to be satisfied
* Use **will** to express provisions that will be supplied by the customer.

The cost of mischaracterizing the customer’s needs can be expensive, especially if an error is discovered after conceptual design. Requirements analysis is therefore arguably one of
the most important phases in the system’s life-cycle.

## Activity 1: Good and bad requirements
Discuss what’s wrong (if anything) with the following requirements:
1. The electric vehicle (EV) must be capable of travelling faster than any other vehicle in its class.
2. The energy storage system shall store enough energy to power the EV’s motor for four hours of continuous driving.
3. The EV’s chassis shall minimise aerodynamic drag to maximise performance.
4. The EV’s user interface must be intuitive and enjoyable.
5. In the event that the EV’s auto-pilot system experiences a critical failure, the EV will immediately enter a safe state and alert the driver to resume manual control. Furthermore, if the EV’s driver monitoring system detects that the driver has fallen asleep, it will alert them to resume manual control.

In small groups - workshop good requirements (possibly including derived requirements) for the five requirements. 

## Activity 2: Writing good requirements.
What might be some of the requirements associated with an emergency alert system for seniors. Emergency alert systems are often made as a pendant and worn by seniors in order to call for help should they fall or need immediate care in their home. 

<img width="364" alt="Screen Shot 2023-03-10 at 11 30 25 am" src="https://user-images.githubusercontent.com/125527438/224192515-d5196bd1-297a-4347-9f10-3da53dec67df.png">



In the full group workshop 3-5 needs in tabular form.

| **ID** | **Description** | **Importance** | **Source** | **Validation** | **Notes** |
| --- | --- | --- | --- | --- | --- |
| N1.1 | Short Description of need | One of Desirable, Highly desirable, Essential. | Most concerned stakeholder | How would this need be validated | Any Additional Notes |

Now split into small groups write requirements for each need.

Remember that you may need to write several requirements for a single need. Sometimes, you may capture aspects of several needs in a single requirement.

Once you have done this, come back together in a group and present one of you requirement statements to the rest of the class. 

## Activity 3: National Construction Code
Mandatory standards for residential building construction in Australia are enforced through
state and territory level legislation that refers to the National Construction Code (NCC). The
NCC is developed by the Australian Building Codes Board (ABCB), a Council of Australian
Government (COAG) standards writing body.

Volume Two of the NCC deals with Class 1 (residential) and Class 10 (non-habitable)
buildings. Compliance with the NCC is achieved by satisfying the **Performance
Requirements** listed in the Code, where most of the time this is achieved through so called
**Deemed-to-Satisfy Solutions**, i.e. particular design implementations that are also listed in
the Code. A builder or architect can always choose to design their own compliant solution
which is then called a **Performance Solution**.

Download Volume Two of the NCC from the wattle course page.

Split into small groups and write requirement statements for the following two need
statements that reference the national construction code appropriately. 

| **ID** | **Description** | **Importance** | **Source** | **Validation** | **Notes** |
| --- | --- | --- | --- | --- | --- |
| N1.1 | Stairs to the first floor. | Essential | Customer, Builder | Building inspection | Must be legal |
| N1.2 | Wheelchair access to the back door | Highly Desirable | Customer | Building inspection | This will require aramp – should be possible without landings. Must be legal |

## Activity 4: Requirements for Asparagus Harvest
Asparagus havesting is a time consuming manual labour process and several companies
around the world have considered the development of agricultural systems to automate the
harvesting of asparagus.

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

## Activity 5: Verifying Requirements
During the design process the two following stair designs were obtained during the detailed
design phase. You are part of the design team that is tasked with verifying that the designs meet the requirements.

<img width="889" alt="Screen Shot 2023-03-10 at 11 33 14 am" src="https://user-images.githubusercontent.com/125527438/224192749-a62b396c-6627-4faa-a6c9-7dc468c56949.png">


* Which one of the following two design solutions for the going and riser members of a stairway satisfies the relevant NCC Performance Requirement P2.5.1? (Hint: You probably want to read Part 3.9.1 of the Code.)
* How would you go about verification of a Performance Solution for NCC Performance Requirement P2.5.1(a)? (Hint: Read Part 1.2.2 of the Code.) 

## Learning Outcomes
1. Understand different types of requirements, constraints, and assumptions encountered during systems design
2. Gather, analyse, and communicate requirements to technical and non-technical audiences


## Additional Reading
US DoD Systems Engineering Fundamentals
* Chapter 4: Requirements Analysis (pages 35-45)
