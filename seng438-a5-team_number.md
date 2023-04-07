**SENG 438- Software Testing, Reliability, and Quality**

**Lab. Report \#5 – Software Reliability Assessment**

| Group \#:       | 6  |
|-----------------|---|
| Student Names:  | Maarya Ahmed  |
|                 | Hannah Son  |
|                 | Jinsu Kwak  |
|                 | Jack Li  |

# Introduction

This assignment's main objective was to conduct an analysis integration test data using relaibility assessment tools. The two ways to assess failure data is by reliability growth testing and reliability assessment using Reliability Demonstration Chart (RDC). The team learned the importance of fialure data testing and how to use the various software that was to be used. In this lab, C-SFRAT was mainly used to test the failure data. This report encompasses all the necessary figures and explanations about the testing done to the failure data. 

# Assessment Using Reliability Growth Testing 

The input data that we used was from Failure Report 4, and it was converted into an excel sheet in order to be used with C-SFRAT.

From using C-SFRAT, we were able to get the models and their comparison. The columns 'Critic (Mean)' and 'Critic (Median)' were used to rank the models. The models that had Critic (Mean) and Critic (Median) closest to 1.000 were determined to be the models that provided the best fit for the data.

![Screenshot 2023-04-01 130141](https://user-images.githubusercontent.com/77519521/229309483-faf6aeda-40d4-40f7-b0bd-08da877a04eb.jpg)
*Figure 1. C-SFRAT Model Comparison*

So, the models with the best fit were IFRGSB (E), S (None), S(E), DW2 (None), DW2 (F), DW2 (E), DW2 (F, E), DW3 (F), NB2 (F), NB2 (E), TL (None), TL (F), TL (E), and TL (F, E)

To find the range of useful input data, we used Laplace Tests. As seen in Figure 2, the Laplace Test yielded 0 for all data points except for Failure Count 1. Since values between -2 and +2 indicate stable reliability, Failure Counts 2-15 is the range of useful data.

![Screenshot 2023-04-01 125849](https://user-images.githubusercontent.com/77519521/229309374-7a761e3d-bf0f-4251-9e6d-5b5f4ca89ff2.jpg)
*Figure 2. The input data from Failure Report 4 and the results of the Laplace Test*

We then were able to get the MVF graph (Figure 3) and Intensity graph (Figure 4)
![Screenshot 2023-04-01 130811](https://user-images.githubusercontent.com/77519521/229309698-e44513aa-96b7-4ebb-8897-bdfff780d2f6.jpg)
*Figure 3. MVF graph with models with the best fit*

![Screenshot 2023-04-01 131643](https://user-images.githubusercontent.com/77519521/229310049-0d37267c-7f1f-4bdc-96e2-d8b62f84e578.jpg)
*Figure 4. Intensity graph with models with the best fit*

## Advantages and Disadvantages of Reliability Growth Analysis

__Advantages:__

- Predicts the growth or improvement of reliability of a system throughout testing
- Generated graphs provide insight into any time dependent trends and facilitate examining changes at specific points in time
- Therefore it guides the testing process
          

__Disadvantages:__

- Creating reliability growth analysis graphs can be tedious and time-consuming
- Different prediction models can produce varying results, making it challenging to compare and make informed decisions
- Doesn't tell us how to improve the reliability of a system

# Assessment Using Reliability Demonstration Chart 
## __MTTFmin:__
> **MTTFmin:**
> MTTF that results in the first failure point occurring in the Accept region and the previous failure point located in the Continue Test region

          MTTFmin: 1/6 = 0.166

![image](https://user-images.githubusercontent.com/81532489/230562282-52f34a9f-dff8-49b1-ab74-d3c2f941c220.png)

## __Half MTTFmin:__
> **We have decreased the acceptable number of failures, 
>  the reject region in the half MTTF plot should contain more data points for our failures.**

          MTTF: 0.5/6 = 0.0833

![image](https://user-images.githubusercontent.com/81532489/230563771-20027eca-d2f1-40a4-983d-c759bac75e3a.png)


## __Twice MTTFmin:__
> **We have increased the acceptable number of failures, 
>  the accept region in the twice MTTF plot should contain more data points for our failures.**

          MTTF: 2/6 = 0.33

![image](https://user-images.githubusercontent.com/81532489/230563510-f0cc2202-441e-4aef-a762-4ce2e851a242.png)


## __Explain your evaluation and justification of how you decide the MTTFmin:__


# Advantages and Disadvantages of RDC
__Advantages:__

- Provides a simple and straightforward way to assess a system's reliability
- Generating plots and analyzing data using RDC is quick and easy
- RDC is a low-cost method of determining system reliability
- Can help identify trends in system reliability over time, making it useful in identifying potential issues early on and making necessary improvements
- Can be used to compare the reliability of different systems, making it a useful tool in system design and selection

__Disadvantages:__

- Unable to provide a quantitative number for system reliability, which is crucial for decision-making
- MTTF calculation with RDC involves a lot of guesswork, which can be tedious and time-consuming
- Relies heavily on the accuracy of the data being collected. If the data is not accurate or is incomplete, the resulting analysis may be misleading
- Not suitable for complex systems where there are many failure modes and multiple components contributing to overall system reliability

Overall, RDC can be a useful tool in assessing system reliability, but it should be used in conjunction with other methods to ensure a comprehensive analysis. It is important to consider the limitations of RDC and use other methods when needed to supplement its analysis


# Comparison of Results

# Discussion on Similarity and Differences of the Two Techniques
__Similarities:__

- Both techniques collect and analyze data to identify trends in system reliability
- Both techniques are do not require the system to be taken offline
- Both techniques help to make informed decisions about system reliability

__Differences:__
- RDC is a low cost and straightforward, Reliability Growth Analysis is more complex and requires more resources
- RDC may miss certain types of failures, Reliability growth Analysis can account for a wider range of failure factors
- RDC is better suited for simple systems, Reliability growth Analysis is better suited for complex systems
# How the team work/effort was divided and managed

Since the assignment contained two parts and we are a group of 4, we decided that it was best that we divide the parts so that each part has two people working on it. For part 1, Maarya Ahmed and Hannah Son was responsible for getting this part done. For part 2, Jinsu Kwak and Jack Li was responsible for getting this part done. 

# Difficulties encountered, challenges overcome, and lessons learned

Some difficulties we encountered was first getting the required software to download on various different operating systems . One person had difficulty in getting the software to download on their Mac. The instructions that were made to download the software were very unclear and most of us were confused for the majority of the time. It was also difficult to understand what exactly we had to do with the failure reports and how to format them differently so that the C-SFRAT software can read the files properly. But after talking around with other peers, we figured out how to convert the word document to be compatible with the software. Another difficulty we encountered was that the report we converted for the software did not work on some people's laptops but it also worked on my other peer's laptops. This created some problems because then we would have to use the other persons laptop and try to get everything done quickly. 

We overcame these challenges by testing all the software and finding one that worked for majority of the group and used their operating systems. By communicating with other peers, we learned quite alot about the software's requirements.


# Comments/feedback on the lab itself

This assignment provided an importance of analyzing integration test data using reliability assessment tools. Some comments about this lab is that the instructions about which software to use could have been better since we all did not know what to do and which software is compatible with which operating systems. Another comment is that there could be more instructions on how to use C-SFRAT to generate the graphs that were required. There were also some confusion revolving around how to reformat the word documents given so if there were some instructions on that, that would be great. 
