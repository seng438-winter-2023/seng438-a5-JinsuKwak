**SENG 438- Software Testing, Reliability, and Quality**

**Lab. Report \#5 – Software Reliability Assessment**

| Group \#:       | 6  |
|-----------------|---|
| Student Names:  | Maarya Ahmed  |
|                 | Hannah Son  |
|                 | Jinsu Kwak  |
|                 | Jack Li  |

# Introduction

# 

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

Advantages

      -Predicts the growth or improvement of reliability of a system throughout testing
      -

Disadvantages

      -

# Assessment Using Reliability Demonstration Chart 

## Advantages and Disadvantages of RDC

# Comparison of Results

# Discussion on Similarity and Differences of the Two Techniques

# How the team work/effort was divided and managed

# 

# Difficulties encountered, challenges overcome, and lessons learned

# Comments/feedback on the lab itself
