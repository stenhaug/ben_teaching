Updated 11/02/2020

Instructions
============

As usual, you'll submit your do file and respond to questions as comments in the do file. If you'd like to submit a do file and a word/google document that works too.

Background
==========

The principal of Warren Early College High School, Dr. Baker, experimented with three different class sizes this past year: small, medium, and large. She is interested in if class size seems to have an effect on math and reading test scores. [The dataset scores](https://drive.google.com/open?id=0BxNjWD0-A_iaNHNPeDdnaHgwcWs) includes information on the student, the class size they were in, and their math and reading scores. The scores are reported as standard scores which at the population level have a mean of 100 and a standard deviation of 15 (similar to popular IQ tests).

Cleaning
========

One thing you'll notice is that both household income and test scores are not stored as numbers. Start by finding a way to clean the data. In particular:

1.  Remove the k from household\_income to get just the number
2.  Make a math\_test\_score and a reading\_test\_score column and store a number in there (this will make the dataset half as long)... Note this is tricky! Here are some steps that might help:

-   Convert the current test\_score column into two separate columns: test\_name (reading for example) test\_score\_numeric (102 for example)
-   Reshape the data

Explore generally
=================

Explore the scores dataset. At a minimum, be sure to answer the following questions:

1.  How many students are in the dataset?
2.  How many students are in each class size?
3.  What is the gender breakdown? Does it appear to vary by class size?
4.  What is the distribution of household incomes? Does it appear to vary by class size?
5.  What is the distribution of test scores? Do they appear to vary by class size?

Math
====

1.  Run an anova to see if math scores vary by class size. What can you conclude?

2.  Run a regression with y = math and x = class\_size. How does this compare to the anova?

3.  Now add in household\_income as an independent variable into the regression. What changes? What can you conclude?

4.  Add in gender as well. What can you conclude?

Reading
=======

1.  Run a regression to determine the effect of class size on reading. What do you find? How does it compare to math?

Prediction
==========

Make a prediction for each of the following students math and reading scores:

-   Male, household income of 50k, in a small class size
-   Male, household income of 50k, in a medium class size
-   Male, household income of 50k, in a large class size

-   Female, household income of 100k, in a small class size
-   Female, household income of 100k, in a medium class size
-   Female, household income of 100k, in a large class size

Suggestion
==========

Time to make a decision. It costs the school 4k a year to have a kid in a small class size for the year, 3k a year for a medium class size, and 2k a year for a large class size. What size classes would you suggest the school uses for their students. Why? Be sure to consider other uses of school funds.
