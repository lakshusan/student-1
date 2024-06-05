---
toc: false
comments: true
layout: post
title: Final Project Plans
description: Adding on to the main CPT project a feature with algorithms
type: plans
courses: { compsci: {week: 32} }
---

# Purpose
- We can use the algorithms to reverse the pupose of the previous Data Structures Poject code.

Instead of converting SAT Score to a GPA, we can instead convert GPA to possible SAT Score.

We will use a different database with the RandomForestRegressor to adapt and produce predictions. We will instead have to use a float instead of integer format for the input, which is because th GPA will be entered to the nearest hundredth instead of a whole number. 

# Incorporating Lists
- We can add a mechanism that saves the predicted score to the user's attributes as a list.

For Sorting and Searching, we can add all the scores to the user's attributes and create a function that sorts through the list to find the 3 highest predicted scores.

---

# Final Project - Altered

The GPA to SAT score calculation is done with RandomForestRegressor and a different dataset compared to before (with SAT to GPA).

I did something different from the plans for my actual project. I decided to not rely on SQL for sorting and searching and instead just work with saved values in arrays.

This is what a user would see while going to the website for their score calculation.

<img src="https://i.ibb.co/hB5WJxL/image.png">


The user must add a list of GPAs separated by commas, and each GPA inputted will be one iteration of conversion to SAT Score. We defined an empty array beforehand, so that each time the program iterates, it will append the converted score to an array.

<img src="https://i.ibb.co/5rYr4bZ/image.png">

<img src="https://i.ibb.co/64Jkp7K/image.png">

After getting the values in the array, it will go through each score to figure out which is the maximum by seeing if the next score in the list is greater than the value defined by the item substring. After it finishes looping through, the maximum predicted score is saved is maxValue and is returned.

<img src="https://i.ibb.co/mXVnsR0/image.png">

By doing this, it searches through the elements in the array to find the one that is greatest, and outputs the greatest predicted score based on your GPA.

This shows the predicted scores individually in the console as it hits this breakpoint for the 4th time, displaying the 4 individual conversions.

<img src="https://i.ibb.co/X7wHsdP/image.png">

<img src="https://i.ibb.co/Q85zWzh/image.png">

To display the max value, this shows the iteration through each of the converted SAT scores, and in the end, it outputs the actual maximum value.

<img src="https://i.ibb.co/xqFVgXm/image.png">

<img src="https://i.ibb.co/DQwTwpj/image.png">

# Key Commits

- [Frontend Commit, Sorting](https://github.com/lakshusan/lmc-front2/commit/57cc27762c9b70fe126617ac0b1604fad6565823)
- [Database Update](https://github.com/lakshusan/lmc-back2/commit/6a6107f1ca416f2eebdeaf16d187ea625e5c91bd)
- [Regressor Model](https://github.com/lakshusan/lmc-back2/commit/9e9bdedf14fe6eee6e041f95b9a8fb8d1c1a4465)