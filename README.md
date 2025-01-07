# Uncommon HTML Error: Incorrect getElementById Usage
This repository demonstrates a common yet subtle error in JavaScript when interacting with HTML elements using `getElementById`. The error arises from including the '#' symbol when selecting elements using `getElementById`. The '#' symbol is used as a selector in CSS and various other JavaScript methods, but it's not required with `getElementById`.

## Bug Description
The bug occurs in the `bug.html` file. The JavaScript code attempts to select the element with the ID "myDiv" using `document.getElementById('#myDiv')`. However, this is an incorrect usage. The '#' should be omitted.

## Solution
The `bugSolution.html` file demonstrates the correct way of selecting the element. It correctly uses `document.getElementById('myDiv')` to select the element, allowing successful modification.

## How to reproduce
1. Clone this repository.
2. Open `bug.html` in your browser. You will see an error in the console and text not changing.
3. Open `bugSolution.html`. You will see the text changed.