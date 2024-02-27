# Workshop 2: Customer Needs/Standards and Regulations
Relevant lectures: L02: Customer Needs / Standards and Regulations

# Introduction
The initial phase of requirements analysis involves three steps
1. Crafting a scope document
2. Identifying Stakeholders
3. Generating a Stakeholders' needs list.

These three steps are all associated with acquiring information on the system and building an understanding in the design team of what the problem space is.

Standards and Regulations are a core tool in developing the formal System Requirements Specification (SRS) and a good understanding of how to use standards is critical to a profession
engineer.

# Part I: Customer Needs
Consider a scenario where ANU board of directors decides to introduce campus wide public transport. The high level project statement from the Vice Chancellor is to build a transport system that connects the student accommodations, the core teaching and learning hubs of the
campus, union square, through to the civic transport hub.
The project should be innovative, exciting and not too expensive to implement. Your design team is employed to develop the project design.

## Activity 1: Project Scope
Split into small groups and consider fleshing out the project scope document. You may use the vision statement of the Vice Chancellor as the high level project vision.
A transport system that connects the student accommodations, the core teaching and learning hubs of the campus, union square, through to the civic transport hub.

Start by drawing a context diagram for the system.
Once you have a first draft of the context diagram – try running a journey map for a student living in a residence, who needs to go to a lecture, then go to civic to buy groceries, and then
return to their residence.
Try running a second journey map for a staff member who is coming in to work from a Canberra suburb.
Hint: When you do a journey map you will naturally think of certain technology that would solve part of the journey.
For example, the staff member takes a bus to the civic transport hub, and then takes a smaller autonomous bus to the campus.
When you do this, try replacing the technology specific choice by something else – for example, ANU branded electric scooters from
civic to campus.
Look for opportunities to challenge your own technology assumptions. 

## Activity 2: Stakeholder list
From the context diagram and journey maps that you undertook in Activity 1, write up a list of stakeholders.
Initially, just get as many stakeholders as you can all in a list.
Now, go down the list of stakeholders and rank their importance against the five criteria Legitimacy, Power, Influence, Immediacy, Vested interest.
A simple three level ranking high, average, low in each separate category is usually sufficient to capture a basic understanding of
the stakeholder importance. You should end up with a table similar to the following:

| **Stakeholder** | **Legitimacy** | **Power** | **Influence** | **Immediacy** | **Vested Interest** |
|---|---|---|---|---|---|
| Vice Chancellor | Average | High | High | Average | Average|
| Student | Average | Low | Low | High | High |
| Police | High | Low | High | Low | Average |
| etc | | | | | |


## Activity 3: Stakeholder needs list
The final stage of customer needs is to compile a stakeholder needs list. Compiling a full stakeholder needs list would take far too long for a short tutorial exercise, and we will only try
and get a few needs written down to learn the approach.
You should try and get at least two needs each from at least three stakeholders written down.
Choose one stakeholder from the list above. It is a good idea to choose a stakeholder with a good number of high categories so that you have something to work with. Brainstorm with your
group what needs this stakeholder may have.
Each need must be given a short description, an importance, the stakeholder associated with that need should be listed and any notes provided. The levels of importance that are used are Essential, Highly Desirable, Desirable, Preferable. Note that essential means that that particular stakeholder sees the need as essential to have the project succeed, not that it is actually essential, or that the stakeholder would not still use the project if the essential need is not met.
When you are discussing stakeholder needs you will come across examples of needs that are more than essential – they are constraints.
That is they can not be compromised at all. Such needs must be of the form – if this need is not met, they project cannot be built. For example,
if the transport technology does not meet Australian road rules, then use of the facility would be illegal and the project would not be built. This “need” would be encoded as a constraint:
“Compliance with Australian Road laws”.
There are some needs that are less about the structure that the system will have, and more about the environment that the system will be part of. For example, it is clear from context that
the system is not intended to provide transport to and from the Australia National Telescope Facility in the ANU Siding Springs Observatory campus near Coonabarabran in western NSW.
This “need” could be ncoded as an assumption: “The system will be designed to service the ACTON campus area”.
At the end of the exercise you should have a list of stakeholder needs similar to that below, along with a list of dot point assumptions and constraints.

| **ID** | **Short Description** | **Importance** | **Stakeholder** | **Notes** |
| --- | --- | --- | --- | --- |
| N1.1 | Highly utilized by students | Highly desirable | Vice Chancellor | The project must be seen to be being used extensive to be perceived as a success. |
| N2.1 | Low Cost | Essential | Student | Students cannot afford expensive transport options. |

The final step is to assign tracking numbers to the stakeholder needs. This is done by grouping similar needs together, regardless of which stakeholder the need came from. And assigning
groups of similar needs the same group number, and then numbering each need separately within each group.
Subgroups can be formed to help structure the needs list. A good rule of thumb is to keep the number of elements at any level of the hierarchy to around 7 entries maximum.

# Part II: Standards and Regulations
Standards and regulations exist to ensure that products are safe, reliable, compatible, and consistent.
Standards are often employed by engineers to simplify product design and development. Regulations are mandatory standards that are maintained and enforced by a regulatory agency or governing body.

## Activity 4: CO2 emission standards
Suppose that you are an automotive engineer at BMW who is responsible for designing the BMW
X1 series. The following table lists some of the specifications of four representative models in this series.

Table 1: Vehicle details for BMW X1 F48 series, from October 2015

| **Class Description** | **Transmission/Gearbox** | **Engine Capacity (cm^3)** | **Fuel Type** | **Co2 Emissions (g/km)** |
| --- | --- | --- | --- | --- |
| X1 sDrive18d - 17'' & 18'' wheels | M6 | 1995 | Diesel | **109** |
| X1 sDrive18d - 19'' wheels | M6 | 1995 | Diesel | **114** |
| X1 xDrive18d - 17'' & 18'' wheels | M6 | 1995 | Diesel | **124** |
| X1 xDrive20d - 17'' & 18'' wheels | M6 | 1995 | Diesel | **127** |

Reference: Climate Change Authority (2014), International Implementation of Vehicle Emissions Standards.

Your manager has tasked you with identifying the impact of longer term regulation changes (listed in the table below) in several of your key target markets on the ongoing viability of the
series. Keep in mind that regulatory emission targets are set for **fleet averages**.
What do you propose that BMW do?

Table 2: Global comparison of standards for passenger vehicles

| **Jurisdiction and first compliance year** | **Basis** | **Future Target Years** | **CO2 Target (g/km)** | **Fuel Economy Target (L/100km)** |
| --- | --- | --- | --- | --- |
| EU 2009 | CO2 Emissions | 2021 | **95** | 3.6 |
| United States 1975 | Fuel Economy & GHG | 2020 | **121** | 4.6 |
| China 2004 | Fuel Economy | 2020 | **117** | 4.4 |
| India 2016 | CO2 Emissions | 2021 | **113** | 4.3 |


# Learning Outcomes
1. Understand the difference between standards and regulations, and how they apply in the real-world
2. Represent requirements using formal contract language
3. Identify, analyse and objectively resolve design trade-offs

# Additional Reading
NASA Systems Engineering Handbook
* Chapter 2: Fundamentals of Systems Engineering (pages 3-16)

US DoD Systems Engineering Fundamentals
* Chapter 1: Introduction to Systems Engineering Management (pages 3-10)

International Electrotechnical Commission (IEC)
* http://www.iec.ch/
* Explore the website for the International Electrotechnical Commission (IEC)

National Construction Code, Building Code of Australia, Volume two
* https://ncc.abcb.gov.au/




