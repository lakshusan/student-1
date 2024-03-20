---
toc: false
comments: true
layout: post
title: 2021 Collegeboard MC Corrections
description: Test corrections and reflection on performance and progress
type: plans
courses: { compsci: {week: 27} }
---

# 2021 Collegeboard MC Corrections

1. Q15: Use drawLine procedure to draw figure
<img src="https://cdn.discordapp.com/attachments/796087225535168512/1219726092542279710/image.png?ex=660c5971&is=65f9e471&hm=2269c0e3872cd83ca350427397c1c33306e9eb85a9dc0a71b6a6acc4764bd6cc&">

I added the length to the second x-value instead of the second y-value to produce the graph.

2. Q25 Result of iteration statements
<img src="https://cdn.discordapp.com/attachments/796087225535168512/1219726951023906836/image.png?ex=660c5a3e&is=65f9e53e&hm=40909e9e911dce872b83f8946485de92d510726cf65f2d2186348b71f0c804cb&">

I thought that since the procedure would keep repeating and the result would not be returned, that it wouldn't return anything. I didn't pay attention to the other answer that made sense and it would instead return the sum of the integers from 1 to n.

3. Q33 Efficiency of driving route algorithms
I got confused because I didn't know what the word 'heuristic' meant.

4. Q43 Keylogging example
I did not know what keylogging was (recording keys struck on a keyboard by a user unaware of the record)

5. Q48 Use of a rogue access point
I didn't know what a rogue access point was (an unauthorized individual viewing network traffick on a weak or unprotected router)

6. Q55 Move element from end of list to beginning
I chose the option with 'insert' instead of 'append' so it inserted the element at the wrong place in the list.

7. Q63 Boolean expression equivalent to table
<img src="https://cdn.discordapp.com/attachments/796087225535168512/1220092946335137913/image.png?ex=660daf1a&is=65fb3a1a&hm=c00de2431b940370c03930da9fc94455e6323fd952475f991eb77660dbfa387d&">

One of my answers was correct, but the other answer I chose is impossible, since if it was neither true nor false, the value of the expression would not match.

# Popcorn Hacks

1. Binary bit overflow

When there are 8 bits, the maximum number you can represent in binary is 255. Is one more is added to get 256, it is an overflow, so all the digits reset to zero. This is because 256 requires a 9th bit which is unavailable.

2. Making RGB standard colors

Each color in R, G, and B are represented in numbers between 0 and 255, since colors are organized with an 8-bit sequence. Each color is represented by different binary values, and they are combined to make different colors. Pure red is (255, 0, 0), pure green is (0, 255, 0), and pure blue is (0, 0, 255). I liked this subject since it is similar to my CPT warmup project, which was a random color generator.

3. Concatenation options

animal = " magic"[0:6]

animal = " not"[0:3] + animal

animal = "it's " + animal

print(animal)

output would be "it's not magic"