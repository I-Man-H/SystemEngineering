# Workshop 5: Functional Analysis & Allocation 

Relevant lecture: Week 5: Conceptual Design 

## Introduction 

An essential activity in early conceptual design is the development of a functional description of the system. **Functions** refer to specific or discrete actions (or series of actions) that are necessary to achieve a particular objective. Such actions may ultimately be accomplished using equipment, software, people, facilities, data, or various combinations thereof. However, at this point in the design process, the aim is to specify the ‘whats’, and not the ‘hows’. 

**Functional Analysis** is a process used to translate system-level requirements into detailed functional architecture. It is an iterative and recursive process that responds to the ongoing activities of both the requirements and design loops, allowing the identification of functional issues to prompt the re-examination of higher-level requirements or lower-level component selection. The result of functional analysis is the generation of a function flow block diagram that is used (along with the Systems Requirements Specification) during Design Synthesis to construct and evaluate various design alternatives that satisfy the system’s requirements.    

## Activity 1: Reverse Engineering 
In groups of three, reverse engineer an automatic teller machine (ATM). 

1. Start by describing the subsystems and components for a typical ATM (hole in the wall): Cash box, keypad, screen, card slot, communications, power, database, etc.  Draw them on a page with interconnections between components that interact.  This is a simple version of a System Architecture for a typical ATM.  Keep the number of subsystems to 5-7 for the purposes of this tutorial to keep the work down.
2. Assign functions to each of the subsystems.   That is for each subsystem, consider a functional description of the role or purpose that it plays.  You may need more than one function for a given subsystem.
3. Write a function flow block diagram for an ATM.  

From the insight gained in the functional analysis, can you propose an alternative systems architecture for the functions of the ATM? 

## Activity 2: Functional Analysis 
You are part of a design team put together by a large technology firm to build an electronic voting system for the Australian Electoral Committee.  The following requirements  were developed by the team. (Note that these listed here would represent only a subset of high-level requirements for such a project.)  

**Access**
| Requirement ID | Requirement      | Description                                                  |
|----------------|------------------|--------------------------------------------------------------|
| R1.1           | Accessibility    | A Registered_Voter shall be able to vote from any Polling_Station within the nation. |
| R1.3           | Eligibility      | The system shall only allow Registered_Voters to vote.       |
| R1.4           | Uniqueness       | The system shall prevent Registered_Voters from voting more than once. |


**Voting**
| Requirement ID | Requirement       | Description                                                                  |
|----------------|-------------------|------------------------------------------------------------------------------|
| R2.1           | Verification      | A Registered_Voter shall be able to confirm and correct their vote before committing it. |
| R2.2.1         | Validity of vote  | A Registered_Voter shall receive a warning if their vote will be invalid.     |
| R2.2.2         | Invalid votes     | The system shall accept invalid votes.                                        |
| R2.3           | Convenience       | The system shall allow Registered_Voters to vote within a Reasonable_Time_Period. |

**Audit**
| Requirement ID | Requirement   | Description                                                                                   |
|----------------|---------------|-----------------------------------------------------------------------------------------------|
| R3.1           | Accuracy      | The system must count all votes correctly.                                                    |
| R3.2           | Audit         | The system shall provide reliable and demonstrably authentic records of all votes.           |
| R3.3           | Data          | The system shall provide digital records of the votes to the AEC_Tally_Room_System within 1 hour of the close of the Polling_Station. |


**Privacy and security**
| Requirement ID | Requirement      | Description                                         |
|----------------|------------------|-----------------------------------------------------|
| R4.1           | Anonymity        | The system must guarantee that the Registered_Voter identity is not associated with the vote. |
| R4.2           | Integrity        | The system shall guarantee that a Cast_Vote cannot be tampered with. |
| R4.3           | Open source      | The system shall be Open_Source. |

### Glossary:  

**Registered_Voter**: A citizen of Australia who is registered on the Australian electoral role.  

**Reasonable _Time_Period**:  A typical voter should be able to complete the voting process in a similar time to the existing process.  This is presently benchmarked at around 5-10 minutes.    Verification will be based on the median time to vote for Test_Panel performance.   Validation based on median time to vote in a local election during beta-test.  

**Test_Panel**: A group of at least 50 employees from the firm and AEC.  

**Open_Source**:  A system for which the code, the hardware, and all processes of the system are available in a public forum.  No proprietary or hidden components or code may be used in such a system.  

**Cast_Vote**:  A committed vote once the Registered_Voter has completed the voting process.  

**Polling_Station**:  A station provided by the AEC during elections to provide a physical place for voting.  Typically a hall in a local school or similar.  

**AEC_Tally_Room_System**: A central database that collates voting outcomes from different polling booths and provides aggregate tallies of votes after the election closes. 


### Exercise

1. Identify a set of functions that capture the operation of the system.
   * This is deliberately phrased as a very open question.  You can expect to spend considerable time on this question. 
2. Write up a function flow block diagram for the system. Include
   * Inputs
   * Outputs
   * Boundary

## Function Flow Block Diagram (FFBD)

![ffbd1](https://user-images.githubusercontent.com/125527438/226911328-1f57b3fd-5323-45e9-a3bd-0dd12b20f1f0.png)

## Functional Hierarchy

![ffbd2](https://user-images.githubusercontent.com/125527438/226911455-c7af7104-3d04-403f-9172-f0ad7db56265.png)


## Useful Links

To draw your diagrams (FFBD, System Architecture, Concepts etc.), you may use [this website](https://app.diagrams.net/).
 * It is completely **free**.
 * It can be shared via Google Drive, OneDrive, and DropBox for collaborations (useful for group projects).
 * It can generate PNG, SVG, PDF etc. formats with high quality (useful for assignments and group projects).


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
