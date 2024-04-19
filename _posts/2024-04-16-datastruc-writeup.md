---
toc: false
comments: true
layout: post
title: Data Structures Project Writeup
description: Based on integrated ML projects between triangles
type: tangibles
courses: { compsci: {week: 30} }
---

## Collections

This is out SQLite database with initiating the users, and users.py showing the users and their respective schema details, expressed in the database. 

<img src="https://cdn.discordapp.com/attachments/796087225535168512/1230551541367439522/image.png?ex=6633bb6e&is=6621466e&hm=10fb05e0e39b0f343ed370a942b0561985ef7b73965a6db0280859ff38c5b371&">

<img src="https://cdn.discordapp.com/attachments/796087225535168512/1230551830572961842/image.png?ex=6633bbb2&is=662146b2&hm=183bd38a1adc7c8151faf74f921a00424869abd08d76a48cb10b4ae74974d75d&">


## Lists and Dictionaries

This is the GET function which retrieves the user information with the prompt on user login, using the username and password. It will return user data like their point balance, their inventory, and more.

<img src="https://cdn.discordapp.com/attachments/796087225535168512/1230552981091651624/image.png?ex=6633bcc5&is=662147c5&hm=11202b1b227ba7a74f29a576871f045a8eaa0e1ca503394bfaf6746ee96a493d&">

## API and JSON

These are the CRUD functions in the API that use JSON input to get a certain output.

### POST

Adds user to database

<img src="https://cdn.discordapp.com/attachments/796087225535168512/1230554361369722940/image.png?ex=6633be0e&is=6621490e&hm=b12fc93dd1067bc8d9dd4ada4e81ba5286b40cb82a83768ad3f331799c8f5333&">

### GET

Retrieves user information from the database, output in JSON

<img src="https://cdn.discordapp.com/attachments/796087225535168512/1230552981091651624/image.png?ex=6633bcc5&is=662147c5&hm=11202b1b227ba7a74f29a576871f045a8eaa0e1ca503394bfaf6746ee96a493d&">

### PUT

Edits the user information ex. change username

<img src="https://cdn.discordapp.com/attachments/796087225535168512/1230554721035751575/image.png?ex=6633be64&is=66214964&hm=fafe50445d0f3af1cc8813dc35749f00dcf6a5772ddf11a63f971827ddc208f9&">

### DELETE

Deletes user (admin only) and removes frmo database

<img src="https://cdn.discordapp.com/attachments/796087225535168512/1230555176100954215/image.png?ex=6633bed0&is=662149d0&hm=ea3547c0b59bfe5407523e7e25dcb0acf76fd01c2dd509e6a58e273f8460b30e&">

## Postman

### POST

<img src="https://cdn.discordapp.com/attachments/796087225535168512/1230555967507271733/image.png?ex=6633bf8d&is=66214a8d&hm=25db3969aad1a52fb547e62eea23104468e96e6957f742775f7f89ed24ee8366&">

### GET

<img src="https://cdn.discordapp.com/attachments/796087225535168512/1230556142833504326/image.png?ex=6633bfb7&is=66214ab7&hm=d508c3fb7bbd7fb91a7f6dcdd8faf672fc3527193bc792f36cebf8c6843d135b&">

### PUT

<img src="https://cdn.discordapp.com/attachments/796087225535168512/1230558795038589118/image.png?ex=6633c22f&is=66214d2f&hm=c68f069ca9dc18e5e908a87496a6e0a409ebba38203407bfc3719254e95ef09c&">

### 400 POST

<img src="https://cdn.discordapp.com/attachments/796087225535168512/1230557838208663652/image.png?ex=6633c14b&is=66214c4b&hm=370f9c16dcb69d167f279a386da21dfa1df7a14727e1648c4dac5be886f5fe8e&">

### 404 PUT

<img src="https://cdn.discordapp.com/attachments/796087225535168512/1230559006758801438/image.png?ex=6633c261&is=66214d61&hm=8b2ec8ea0b8d563401d7928d8611d72c2697055f8f2b56760a7fdfcb0e54cc02&">

## Frontend

GET, UPDATE, and POST with JSON responses

<img src="https://cdn.discordapp.com/attachments/796087225535168512/1230880307906084895/image.png?ex=6634ed9e&is=6622789e&hm=949a4af988a30c0159f5f190277a5d2dd69cc57ee92b5b4afb8147fe228242a8&">

<img src="https://cdn.discordapp.com/attachments/796087225535168512/1230880478303621120/image.png?ex=6634edc6&is=662278c6&hm=68d62e3cf5169235b46e19c5dd1f875cff5fba158696926a8cc4656590fc7530&">

GET with formatted data

<img src="https://cdn.discordapp.com/attachments/796087225535168512/1230883590536040478/image.png?ex=6634f0ac&is=66227bac&hm=46aefde22a7dde5bf7d21ac130234c016500383ed6b5956a58329408b1bc268d&">

Fetch and Iteration

<img src="https://cdn.discordapp.com/attachments/796087225535168512/1230885357801963573/image.png?ex=6623ced2&is=66227d52&hm=ee908c2ae75833f818d189f2dc099955686519e3aa8660ced7ad4d0458b9b51e&">

<img src="https://cdn.discordapp.com/attachments/796087225535168512/1230884790115373126/image.png?ex=6634f1ca&is=66227cca&hm=c8d1a72cab957e69e74dad748c7ca9837afe342b659614643531d664373bd883&">

POST Demo Success and Failure

<img src="https://cdn.discordapp.com/attachments/796087225535168512/1230885908270682202/image.png?ex=6623cf55&is=66227dd5&hm=c481ec597825bc6b7d4d8c317f1f58fe013bc5bbc5e1edf355fa8c5d2a7321e9&">

<img src="https://cdn.discordapp.com/attachments/796087225535168512/1230885958044356670/image.png?ex=6634f2e1&is=66227de1&hm=1a5d072819f0d53f83d776ce7f765d1ce0e3ef5e2d16f48017c4149b6667b25d&">

<img src="https://cdn.discordapp.com/attachments/796087225535168512/1230887050602090558/image.png?ex=6634f3e5&is=66227ee5&hm=a04ec0219ef3f8142de95f073a41c415c6c6bfdf8b3e8d2d6a8de58194f8ce17&">

## Algorithm Analysis

<img src="https://cdn.discordapp.com/attachments/796087225535168512/1230889058138587147/image.png?ex=6623d244&is=662280c4&hm=153e382e938781b48d087da5d95021d01d62baa3dc3f85349cdfc1d9e7600dd0&">