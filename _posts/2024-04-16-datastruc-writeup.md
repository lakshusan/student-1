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

