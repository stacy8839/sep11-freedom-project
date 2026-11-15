## Name: Stacy M.
## Period: 1
## Course: Conditionals and JavaScript 
## Concept: Conditionals, Functions,`Math.floor()`, and my Git Collaboration with Jasmine!
---
## Context 

In this SEP course, I collaborated with my partner Jasmine on our **Guess the Color** JavaScript project (`js-2028-jsproject-group-26`),In this project I learned how to combine conditionals, user input, functions, and arrays to build an interactive guess the color game! Although I missed the day the project was announced, Jasmine and I teamed up to create a game that tested all the concepts we have been learning in class.

To keep things fair, we split the tasks 50/50 and I built a detailed `plan.md` file with a clear timeline adjusted to both our schedules and flexibility:

* **Conditionals (`if` / `else if` / `else`):** Creates user responses (like `"yes"` or `"no"`) and compares the player's color guess to our secret color.
  
* **User Input & Output (`prompt()`, `alert()`, `document.write()`):** This welcomes our player, taking their name and color guess, and shows the results on the page.
  
* **Random Selection (`Math.random()` & `Math.floor()`):** This helped pick a random secret color from an array so every round is different and fun to play around.
  
* **Our Project Planning (`plan.md`):** We broke the project into 5 clear steps with real code examples and a Tuesday through Friday schedule so we stayed on track, we even finished ahead of time which is a bonus!

---

## Some Code Examples I Practiced 

Here are code examples directly from our **Guess the Color** project, including user input, conditionals, and our random color function!:

```javascript
// 1. Welcoming the player, saving input, and fixing the color list prompt
alert("Welcome to the Color Guessing Game!!");
var playerName = prompt("What is your name?");
let colors = ["red", "blue", "green", "yellow", "purple"];
let guess = prompt("Guess a color from this list: red, blue, green, yellow, purple");

// 2. Using conditionals and .toLowerCase() to check if the player is ready
let ready = prompt("Are you ready to guess a color?");

if (ready.toLowerCase() === "yes") {
  alert("YAY:D Let's have fun together!");
} else if (ready.toLowerCase() === "no") {
  alert("Aw man :C that's okay");
}

// 3. Random Color Function using Math.floor() and Math.random()
function getRandomColor(colorArray) {
  var randomIndex = Math.floor(Math.random() * colorArray.length);
  return colorArray[randomIndex];
}

// 4. Win or Loss conditional rules and TAYLOR SWIFT!!!
var secretColor = getRandomColor(colors);

if (guess === secretColor) {
  alert("OMG" + playerName + "! You guess it right! Yippe! Taylor Swift would be proud! :)");
} else {
  alert("Sorry you lost, " + playerName + "... the secret color was " + secretColor + ". Better luck next time!");
}




[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)
