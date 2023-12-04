---
toc: false
comments: true
layout: post
title: cpt warmup - color generator
description: cpt js code opt 2
type: plans
courses: { compsci: {week: 15} }
---





<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Color Mixer</title>
    <style>
        #result {
            margin-top: 20px;
            width: 200px;
            height: 200px;
            border: 1px solid #000;
        }
    </style>
    <script>
        function translateColor(event) {
            event.preventDefault();
            // get input values
            var redValue = document.getElementById("redValue").value;
            var greenValue = document.getElementById("greenValue").value;
            var blueValue = document.getElementById("blueValue").value;
            // validate input values (must be between 0 and 255)
            if (!isValidInput(redValue) || !isValidInput(greenValue) || !isValidInput(blueValue)) {
                alert("Please enter valid numbers between 0 and 255.");
                return;
            }
            // convert inputs to binary
            var redBinary = decimalToBinary(redValue);
            var greenBinary = decimalToBinary(greenValue);
            var blueBinary = decimalToBinary(blueValue);
            // display binary output
            document.getElementById("result").innerHTML = `
                <p>Red: ${redBinary}</p>
                <p>Green: ${greenBinary}</p>
                <p>Blue: ${blueBinary}</p>
            `;
            // calculate the final color
            var finalColor = "rgb(" + redValue + "," + greenValue + "," + blueValue + ")";
            // display the final color
            document.getElementById("result").style.backgroundColor = finalColor;
        }
        function decimalToBinary(decimalValue) {
            return parseInt(decimalValue).toString(2);
        }
        function isValidInput(value) {
            return !isNaN(value) && parseInt(value) >= 0 && parseInt(value) <= 255;
        }
    </script>
</head>
<body>
    <form onsubmit="translateColor(event)">
        <label for="redValue">Number 0-255 for Red</label><br>
        <input type="number" id="redValue" name="redValue" required><br>
        <label for="greenValue">Number 0-255 for Green</label><br>
        <input type="number" id="greenValue" name="greenValue" required><br>
        <label for="blueValue">Number 0-255 for Blue</label><br>
        <input type="number" id="blueValue" name="blueValue" required><br>
        <input type="submit" value="Submit">
    </form>
    <div id="result"></div>

</body>
</html>
