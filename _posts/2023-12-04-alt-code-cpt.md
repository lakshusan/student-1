---
toc: false
comments: true
layout: post
title: cpt warmup - color generator
description: cpt js code opt 2
type: plans
courses: { compsci: {week: 15} }
---

<body>
    <script>
        // function to convert binary to hex color
        function binaryToHexColor(binary) {
            var decimalValue = parseInt(binary, 2);
            var hexValue = decimalValue.toString(16).toUpperCase();
            return '#' + '0'.repeat(6 - hexValue.length) + hexValue;
        }
        // display an input prompt and store the user's binary input
        var binaryInput = prompt("Enter a 24-bit binary value:");
        // checks if the input is a valid binary string (0 or 1 input for 24 characters)
        if (!/^[01]{24}$/.test(binaryInput)) {
            alert('Please enter a valid 24-bit binary value.');
        } else {
            // Convert binary input to hex color
            var hexColor = binaryToHexColor(binaryInput);
            // Display the user's input and the generated color
            var outputArea = this.element.parents('.cell').find('.output');
            var outputHTML = '<div style="color: ' + hexColor + ';">Binary Input: ' + binaryInput + '</div>';
            outputArea.append(outputHTML);
        }
        document.write("<p>Output text color</p>");
    </script>
</body>