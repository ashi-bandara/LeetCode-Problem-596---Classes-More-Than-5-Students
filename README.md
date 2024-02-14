
# LeetCode Challenge D53
## Achievements
[![image.png](https://i.postimg.cc/vmrbW5xX/image.png)](https://postimg.cc/Nyj3t94r)

This solution outperformed 89.69% of Java users on LeetCode according to runtime metrics.


## Overview

Welcome to my LeetCode solution repository! This project addresses the coding challenge presented by [596. Classes More Than 5 Students](https://leetcode.com/problems/classes-more-than-5-students/). Below, you'll find details about the problem, my approach to solving it, and the implemented solution.

## Problem Statement
Write a solution to find all the classes that have  **at least five students**.

Return the result table in  **any order**.

The result format is in the following example.

**Example**
>**Input:**
> 
| student | class | 
| :---: | :---: |
| A     | Math |
| B     | English |
| C     | Math |
| D     | Biology |
| E     | Math | 
| F     | Computer |
| G     | Math |
| H     | Math |
| I     | Math |

>**Output:**

| class   |
| :---: |
| Math    |

**Language Used**
> Java

**Difficulty**
> Easy

## Solution Overview
The SQL query begins by selecting the distinct classes from the Courses table. It then joins this result with another derived table that calculates the count of students for each class. The derived table uses the GROUP BY clause to group the data by class and the COUNT function to count the number of students. The main query then filters the result using the HAVING clause to include only those classes where the count of students is greater than or equal to five. Finally, the result is returned, displaying the classes with at least five students.
