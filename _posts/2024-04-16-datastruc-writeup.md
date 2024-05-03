---
toc: false
comments: true
layout: post
title: Data Structures Project Writeup
description: Based on integrated ML projects between triangles
type: tangibles
courses: { compsci: {week: 30} }
---

# Introdution

I used my CPT project, "Let 'Em Cook" to demonstrate different functions using Lists and Dictionaries, API and JSON, and different CRUD commands. The overview of our project is based on the existing game, "Little Alchemy", which uses combinations of parts to create new objects. We took the same idea and used it with the theme of baking; adding different ingredients to create a recipe, making a baked good product. You can buy ingredients with points, which you can earn by making new baked items. You can exchange ingredients with your friends and can check your leaderboard status based on point balance.

My ML project is based on Eun's project, which is a college information site. The project adds a GPA predictor with the input of a user's SAT score. This shows different academic standards and howtheir correlate with each other, both of which are used in college applications.

## Collections

This is out SQLite database with initiating the users, and users.py showing the users and their respective schema details, expressed in the database. We include schema such as name, user id, password, inventory, date of birth, favorite food, points, and role. The user's information in these columns change along with their actions in the game.

<img src="https://i.ibb.co/kgmspfr/image.webp">

<img src="https://i.ibb.co/hY8vNg3/image.webp">


## Lists and Dictionaries

This is the GET function which retrieves the user information with the prompt on user login, using the username and password. It will return user data like their point balance, their inventory, and more.

<img src="https://i.ibb.co/VLYShTK/image.webp">

This is running a post function in the debugger, and I keep going until I get to the user information, where it is shown in the sidebar. The first capture shows the user 'flay' and the information connected to it. The second one shows the number of users that have a login with the game.

<img  src="https://i.ibb.co/YNb9s54/image.webp">

<img src="https://i.ibb.co/ZgczFQc/image.webp">

## API and JSON

These are the CRUD functions in the API that use JSON input to get a certain output.

### POST

Adds user to database, increases 'len' for number of users and adds basic information (including basic ingredients and starting point value)

<img src="https://i.ibb.co/GtQYdCN/image.webp">

### GET

Retrieves user information from the database, output in JSON

<img src="https://i.ibb.co/VLYShTK/image.webp">

### PUT

Edits the user information ex. change username.

<img src="https://i.ibb.co/Sm52sqD/image.webp">

### DELETE

Deletes user (admin only) and removes from database

<img src="https://i.ibb.co/C0Ny9FH/image.webp">

## Postman

### POST

This creates a user called 'test' appends it to the database user list.

<img src="https://i.ibb.co/qWKSRbx/image.webp">

### GET

This outputs all the user information that is listed in the database, specific to the user requested.

<img src="https://i.ibb.co/PQvr15B/image.webp">

### PUT

This example edits the user info to change the point value in the database.

<img src="https://i.ibb.co/ZM6zNT2/image.webp">

### 400 POST

<img src="https://i.ibb.co/S5tvgFp/image.webp">

### 404 PUT

<img src="https://i.ibb.co/D5Cvc28/image.webp">

## Frontend

GET, UPDATE, and POST with JSON responses

This shows the inventory and the changes with the shop. If a button in the shop is clicked, it sends the request to the backend, and if you have enough points, it will append the item to the end of your inventory and tell you the item you bought.

<img src="https://i.ibb.co/ph57cD2/image.webp">

<img src="https://i.ibb.co/Fb4703r/image.png">

GET with formatted data

This is the leaderboard, where you can compete with other users to gain the most number of points by making baked goods. The more items you make, the more points you earn, and the higher you get on the leaderboard.

<img src="https://i.ibb.co/0J721s1/image.webp">

Fetch and Iteration

This fetches to out 8028 backend port with all the data and gets the information from the element it requests.

<img src="https://i.ibb.co/KLh48WM/image.webp">

<img src="https://i.ibb.co/3SznKyn/image.webp">

POST Demo Success and Failure

Recipe for a cookie added into sandbox/oven

If the recipe matches one listed in the backend 'bakings' database, then the baking function will go through and show you the baked good you made.

<img src="https://i.ibb.co/0XK1SQN/image.webp">

Results in oven shaking and "You made a cookie!" 

This particular recipe matched with that of a cookie, so the cookie will be added to the user's inventory.

<img src="https://i.ibb.co/ZcSVpwv/image.webp">

When a recipe does not exist in the database, there is an alert and a log in the console that says "failed: recipe does not exist"

<img src="https://i.ibb.co/jb07z8H/image.webp">

## ML Project

We defined 'predict' in the SATtoGPA model
We used predict in the api, which is what the frontend fetches to. The model is referenced in the API, which uses the .csv dataset to output the correct prediction, converting it to a JSON string. The JSON string the frontend sends is with 'satscore' and uses 'prediction' to output the GPA. 

This uses the RandomForestRegressor to predict the scores based on a given dataset. The dataset does not include all the values, so the algorithm allows the program to provide an accurate prediction. It takes different branches from 2 sides of the input, and gives a prediction that branches in from the other values.

<img src="https://i.ibb.co/bdqDr9s/image.webp">

<img src="https://i.ibb.co/sVWJtYc/image.webp">