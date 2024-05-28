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

There will be an additional column on the user's information that saves the predicted score output in a column titled "scores".