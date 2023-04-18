# Week 7: Preliminary Design 
Relevant Lecture: Week 7: Design Criteria, Week 8 Tradeoff Analysis 

# Introduction 
Once conceptual design is complete the next phase of the systems engineering process is preliminary design.
Preliminary design is focussed on verification and optimisation of the conceptual design.
This stage of the design process involves a significant analysis and benchmarking of various designs.

The key to benchmarking and tradeoff analysis is to develop a system wide quantitative cost criteria that measures the relative merit of different options.
**Quality Function Deployment (QFD)** and the associated **House of Quality (HoQ)** is a powerful tool for system wide comparisons.
The House of Quality tool depends on the development of a set of **Technical Performance Measures (TPMs)** that capture the various requirements of the system weighted by importance.  By tracking customer requirements through to TPMs in a properly weighted matrix the customer needs are represented by properly weighted design attributes and performance measures. In this manner the ‘voice of the customer’ is reflected in the ultimate design. 

In a full design the QFD is used for system optimisation where various design parameter changes are analysed and the resulting design points optimised using the cost criteria.   Doing analysis of different design options is too difficult in a short tutorial session, so instead  we will use the House of Quality in a benchmarking study – another important use of this tool.   Here we will evaluate a range of existing products against the House of Quality and evaluate the relative scores of the different products.  This is an important first step in any preliminary design since it provides key insight into the key competitor designs and how they solved the problem.

The wattle course page has an MS Excel template that you might want to use for this process.
There is an empty template as well as a partly filled template for this workshop’s activity. 

Click [**here**]([Week7/HoQ - Bicycle Suspension.xlsx](https://github.com/I-Man-H/SystemEngineering/blob/main/Week%207/HoQ%20-%20Bicycle%20Suspension.xlsx)) to download the Excel template for this example.

# Activity 1: Select a Bicycle Suspension
In this activity you will compare six different bicycle suspensions and decide which of them best addresses you client’s needs (see Figure 1).

![image](https://user-images.githubusercontent.com/125527438/232694026-3ad5ccb1-9e40-481d-9458-72e194fac28e.png)

Figure 1: Stakeholder requirements and importance. (Ulrich and Eppinger)


  * Add the “Importance” scores to the customer needs section of the HoQ using the data provided by the stakeholder needs study.
  * Determine your overall **design strategy** by filling in the “Benchmark solution” and “Planned design” columns of the HoQ. Together they determine the (planned) “Improvement ratio”. This ratio multiplies the “Importance” score of a need to yield the final “Absolute weight” (sums to an arbitrary value across all needs) resp. the normalized “Relative weight” (sums to one across all needs). This means that a ratio of more than one emphasizes a need while a score of less than one de-emphasizes the need compared to the customer’s opinion. 

Enter numbers in a range 1-5 into these columns, where 5 means “addresses the need very well”, 4 means “addresses the need well”, 3 means “addresses the need partly”, 2 means “addresses the need poorly”, and 1 means “does not address the need

In the absence of a real benchmarking study, a reasonable assumption is that there are existing solutions that address all needs well. This corresponds to entering “4” into all rows of the “Benchmark solution” column. Do this, and agree in your team which needs you wish to carry through unchanged, which ones you wish to emphasize and which ones you wish to de-emphasize. Enter corresponding numbers into the “Planned design” column. 

The spreadsheet will compute the “Relative weight” column accordingly. 

  * Fill in the requirements correlation matrix in the middle of the HoQ diagram. An entry of 9 means “strong relation”, 3 means “moderate relation”, 1 means “weak relation”. A blank entry means “no relation”. You can take the information on which attribute relates to which need from Figure 2, but you will need to determine the strength of the relation.  These corelations were shown in the Lecture slides for this week as well. Take care to enter the numbers into the correct fields.  


![image](https://user-images.githubusercontent.com/125527438/232689753-45451c10-3327-48a4-990c-4c9aba07e8d4.png)

Figure 2: Requirements correlations (Ulrich and Eppinger)


The spreadsheet will now compute the “Absolute importance” (sums to an arbitrary value across all design attributes/TPMs) resp. the normalized “Relative importance” (sums to one across all design attributes/TPMs) rows at the bottom of the HoQ.


# Activity 2: Evaluate Concept Designs 

Consider the 5 concepts drawn from benchmark data: ST Tritrack, Mainray 2, Rox Tahx Quadra, Rox Tahx T1 21, Tonka Pro, Gunhill Head Shox

You will see that in the metric space below the relative importance the metric and benchmark information has been entered.   Your goal is to generate Technical Performance Metrics (TPMs) for each design criteria and to evaluate the 5 concepts. 

First, you need to go along the TPM metric column and fill in a target or target range for every metric.  Do this based on your desire to improve certain aspects of the design or not.  You can see which requirements corelate to which design criteria, and those where you want to improve the design, the targets should be set to push the design.  In other design criteria, meeting the industry benchmark should be sufficient.

A Technical Performance Metric can be generated for each of the Design Criteria by setting control points for an associated graph.  The TPM is a function that assigns a value between zero and one to the measurement of the design criteria.


The standard TPM uses the min, max and provides a range in which the design scores the maximum value of 1. 


![image](https://user-images.githubusercontent.com/125527438/232690303-6b9b45a0-e616-48d1-8bfe-262a1b773a56.png)


It is common that there is a target but that there is no range around the target.   In this case you can set control 2 and control 3 equal.  


![image](https://user-images.githubusercontent.com/125527438/232690349-436334d3-629c-4d82-8692-5f46d34a5e5b.png)

Another common situation is that there is no maximum value.  In this case the right hand side of the graph goes to infinity at value 1.  In my excel code, this is difficult to implement and so I suggest you just double the target value for controls 3 and 4.  

![image](https://user-images.githubusercontent.com/125527438/232690418-7e0ac693-8b9a-489b-be8f-300919df2f25.png)

For the reverse case where there is no minimum – usually, this is associated with a measure that cannot go negative anyway.  In this case we set control 1 and control 2 to zero.

![image](https://user-images.githubusercontent.com/125527438/232690480-305609ff-b60f-4f90-8455-091f5f434fb2.png)


If there is negative data then you need to do a similar trick to the no maximum case but in the negative axis. 

In the MS excel spreadsheet provided there is a second worksheet that has the control points for a single TPM set up and a simple graph that you can use to visualise a TPM when designing it. 

Note that in all cases the TPM is piecewise linear.  This is good enough to capture design tradeoffs in real systems.  There are lots of situations where the design may meet targets and the TPM is 1.  This is the expected, once you have met design targets it is not necessary to continue to optimise the design.  Indeed, a typical design will end up with many targets met and just a few TPM active on the sloped sections where the tradeoffs in the design are active. 

The last case to be discussed is where the values of the design criteria are drawn from a finite set.  For example the design criteria 11 considers the headset size and lists them against each design.  A TPM for this design criteria is to simply an assignment of a value between 0 and 1 to each of the finite possibilities.

| **Metric 11 from bicycle design** | **TPM** |
| -- | -- |
| (1, 1.125) | 0.5 |
| (1, 1.125, 1.250) | 1 |
| N/A | 0 |

The only tricky part is to fit this idea into the spreadsheet format.  Of course, you could just hand enter the appropriate TPM and overwrite the spreadsheet function – there is no requirement to use the control point mapping.  But if you want to use the spreadsheet function, this can be done by mapping the finite set of options into a number.  For example assign the number of headset sizes to each category.  

| **Metric** | **Number of standard headset sizes** | **TPM** |
| -- | -- | -- |
| N/A | 0 | 0 |
|  | 1 | 0.25 |
| (1, 1.125) | 2 | 0.75 |
| (1, 1.125, 1.250) | 3 | 1 |


Again – I am assigning a TPM to each category – however, this time I am deliberately choosing values that allow a simple linear interpolation.  Choosing the control points as follows instantiates this TPM.


![image](https://user-images.githubusercontent.com/125527438/232691309-20bd85d1-5efa-49e2-b44d-c2444c751798.png)

Although this is a bit of a hack it works quite well.  One of the very common cases is if the design criteria is a Boolean parameter (taking only two possibilities) map those options to {0,1} and use

![image](https://user-images.githubusercontent.com/125527438/232691391-2164ab7b-688c-4a29-b1c4-6d0fe47c4c89.png)


Now you can go ahead and score the various concepts by entering the values of the metrics into the columns.  The QFD score is in the blue box on the left of the score. Figure 3 contains the performance of six different bicycle suspension designs against the TPMs. Use this data to score the concepts against every TPM. 


![image](https://user-images.githubusercontent.com/125527438/232692995-8d83ef84-6c57-4036-8e16-385c27ba76cc.png)

![image](https://user-images.githubusercontent.com/125527438/232693048-98c8dc67-d9d0-4ed3-ad73-a49f68632210.png)

Figure 3: Design criteria (Ulrich and Eppinger) 


# Activity 3: Interpreting the outcomes

In your small groups discuss what you can learn from the House of Quality.

  * Consider the final scores obtained from the House of Quality.
  * Are there **significant** differences between the various products?
  * What would you do with this information in a design process? 



# Learning Outcomes

1. Identify, analyse and objectively resolve design trade-offs
2. Understand different types of requirements, constraints, and assumptions encountered during systems design 


# Additional Reading

  * NASA Systems Engineering Handbook 
    * Chapter 5: Product Realization (pages 71-81)
  * US DoD Systems Engineering Fundamentals 
    * Chapter 6: Design Synthesis (pages 57-63) 
    * Chapter 7: Verification (pages 65-72)
  * Ulrich & Eppinger, Product Design and Development 
    * Chapter 5: Product Specifications (first 13 pages of chapter) 
