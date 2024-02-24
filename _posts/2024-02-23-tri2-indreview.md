---
toc: false
comments: true
layout: post
title: CPT Project - Individual
description: Review ticket for Trimester 2 Final, individual review on CPT feature
type: plans
courses: { compsci: {week: 24} }
---

# Overview of Project

Our game is a little spin on the existing game "Little Alchemy". The idea of the game is to combine parts to create other things, and we decided to use the theme of baking. The idea is to accumulate ingredients and combine them to create different dessert combinations.

- Sandbox - Drag and drop from inventory into 'oven' for combining
- Baking - Fetch the recipe from the backend to create a dessert, add points for each recipe found
- Shop - Ingredient organization with opportunity to buy with gained points
- Leaderboard - Orders the users with most points to least points
- Trading - Allows exchanging ingredients and recipes with friends

# Instructions

1. Users will start by registering their account to authorize access to the game
2. The user will have a set inventory of basic ingredients in the 'Baking' category
3. Drag and drop combinations of ingredients and 'bake' to see if they make a product that matches with a recipe
4. If it does not make a recipe, keep trying, and if it does, it will be added to your inventory which gives your points and sometimes allows you to create more versions of the product, like with different flavors.
5. When more points are earned, you can purchase special ingredients from the shop to use in more recipes, which expands the combination opportunities.
6. Once users have started unlocking more products and recipies, they can add friends and trade with them in the "Friends" tab.
7. Check the leaderboard for users' point value placements in order

# Requirements and Fulfillments

## Program Code

|  Requirement |   Usage    |
|-----------------|---------------------------------------------|
| Instructions for input from one of the following: the user, a device, an online datas stream, a file.          | Our project utilizes user input. It involves the user purchasing ingredients from the shop, which adds the item to the inventory.        |
| Use of at least one list (or other collection type) to represent a collection of data that is stored and used to manage program complexity and help fulfill the users purpose | Inventory list starts as empty string and ingredients are added based on user input <img src="https://cdn.discordapp.com/attachments/796087225535168512/1211173693548527736/image.png?ex=65ed3c67&is=65dac767&hm=78fb260d6ce8ffba5f45274dcda49040f365b70b20158f7b2fee73adef00e66b&"> <img src="https://cdn.discordapp.com/attachments/796087225535168512/1211211461875994685/image.png?ex=65ed5f93&is=65daea93&hm=32ebf7aac0c07226ec278532f7e1e8eecf91a63facee34cdf9a185aa1ed182fc&">             |
| At least one procedure that contributed to the program’s intended purpose where you have defined: the name, return type, one or more parameters:      | There is a put request to edit the user's 'item' data, which adds any bought ingredients to that column in the database. <img src="https://cdn.discordapp.com/attachments/796087225535168512/1211193123439644713/image.png?ex=65ed4e7f&is=65dad97f&hm=ad8b8280dbef9d391354c2c8504e797caccfefe5f9d5a2df9f828b100166b73a&">      |
| An algorithm that includes sequencing, selection, and iteration that is in the body of the selected procedure    | Sequencing (getting info): <img src="https://cdn.discordapp.com/attachments/796087225535168512/1211202852450472007/image.png?ex=65ed578f&is=65dae28f&hm=9b0b51d6265c0a2c3ad17166043ed5ddd42e17d04abeda552974551028191694&"> Selection (referencing): <img src="https://cdn.discordapp.com/attachments/796087225535168512/1211203380345708594/image.png?ex=65ed580c&is=65dae30c&hm=2adc61da7016b812a2c465448e25f4bd2af94136ee6c360d750b64013d70b885&"> Iteration (action): <img src="https://cdn.discordapp.com/attachments/796087225535168512/1211204096317726761/image.png?ex=65ed58b7&is=65dae3b7&hm=229e2ffc7cd5dccd9aabee6ea00802ca202462e2e5158fd02a3509f75301e1f2&"> |
| Calls to your student-developed prodcedure:   | Put request for 'updating' user inventory <img src="https://cdn.discordapp.com/attachments/796087225535168512/1211209171819565126/image.png?ex=65ed5d71&is=65dae871&hm=185421edfe2d879d4817167377a1355fd942aaa48ff0efd3d5d46de6d2f6c7b5&">  |
| Instructions for output (tactile, audible, visual, or ) based on input and program functionality   | Fetch from database for inventory <img src="https://cdn.discordapp.com/attachments/796087225535168512/1211210703621328936/image.png?ex=65ed5ede&is=65dae9de&hm=68c00c896bd5791716550aba01591259b75efbd1db2f7fb9f8f5bd1c0ae5c430&">        |

## Video Overview

The video covers my feature, which is the shop. The shop allows a user to buy ingredients past the default ones they start with. Each item costs a certain amount of points, which is deducted from the user's point balance when they purchase the item. The item appends to the 'items' list in the database, changing the user's inventory.

### What's Included:
- Shop feature with console view of action
- Show database change (items list, points)
- Show inventory before and after purchase
- [Link to Video](https://drive.google.com/file/d/1L2Y1-pW3vP95EL5fy9cWuA2hVlr3mTmi/view?usp=sharing)