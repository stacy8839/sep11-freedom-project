## Name: Stacy M.
## Period: 1
## Course: Conditionals and JavaScript 
## Concept: Conditionals, Functions,`Math.floor()`, and my Git Collaboration with Jasmine!
---
## Context 🖳‧₊˚

In this SEP course, I collaborated with my partner Jasmine on our **Guess the Color** JavaScript project (`js-2028-jsproject-group-26`),In this project I learned how to combine conditionals, user input, functions, and arrays to build an interactive guess the color game! Although I missed the day the project was announced, Jasmine and I teamed up to create a game that tested all the concepts we have been learning in class.

To keep things fair, we split the tasks 50/50 and I built a detailed `plan.md` file with a clear timeline adjusted to both our schedules and flexibility:

* **Conditionals ❌✅ (`if` / `else if` / `else`):** Creates user responses (like `"yes` or `"no"`) and it also compares the player's color guess to our secret color.
  
* **User Input & Output 🟥🟦🟩🟨🟪(`prompt()`, `alert()`, `document.write()`):** This welcomes our player, taking their name and color guess, and shows the results on the page.
  
* **Random Selection ⛶ (`Math.random()` and `Math.floor()`):** This helped pick a random secret color from an array so every round is different and fun to play around.
  
* **Our Project Planning ⏰👥 (`plan.md`):** We broke the project into 5 clear steps with real code examples and a Tuesday through Friday schedule so we stayed on track, we even finished ahead of time which is a bonus!

---

## Some Code Examples I Practiced 👩🏻‍💻💡

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

// 4. Win or Loss conditional rules and TAYLOR SWIFT PRAISE!!!
var secretColor = getRandomColor(colors);

if (guess === secretColor) {
  alert("OMG" + playerName + "! You guess it right! Yippe! Taylor Swift would be proud! :)");
} else {
  alert("Sorry you lost, " + playerName + "... the secret color was " + secretColor + ". Better luck next time!");
}
```

## Challenges and Confusions 🤔❓

​I missed the project announcement day which meant I had to catch up fast, and collaborating on GitHub brought a lot of stress at first. Since our tasks depended on each other, I did Step 1, Jasmine did Step 2, and I needed her code before doing Step 3, we had to constantly git push and git pull our updates and message each other to not encounter a git merge. However, I did ran into one git merge issue and I got really nervous, especially when my code got overwritten or deleted after pulling Jasmine's changes, forcing me to rewrite and debug parts of her and my work.

​We also ran into a bug where the prompt asked the player to "Guess a color from the list" without actually showing the list of colors anywhere on the screen. Once I spotted that players were guessing blind, I updated line 10 to display all five colors inside the prompt message and pushed the fix and made sure Jasmine knew about the update I did on her code and for her to pull.

​Another tricky part was figuring out how to pick a random color. I ended up finding Math.random() and Math.floor() on Google and TikTok because we hadn't covered how Math works in JavaScript yet. I understood just enough to get it working in our function, and when Nile used Math during a casual demo and Mr. Mueller broke down how it works, everything clicked and felt completely grounded in my head. 

---

​## Helpful Tips and Tricks I Used ⫶☰

​In order for me to stay organized and avoid any last-minute work, I rewrote our plan.md twice! I turned a very broad and detail lacking first draft into a detailed plan with actual bracket examples like (["red", "blue", "green", "yellow", "purple"]) so Jasmine knew exactly what to build. I kept plan.md open in a tab right next to my Codespaces editor the entire time as my core reference. Because we followed our timeline and communicated nonstop over text whenever one of us pushed or pulled code, we finished everything including bug fixes by Thursday night.


​My Takeaways 🧠💪🏻

​*  A detailed plan.md is the core of a project: Taking extra time to rewrite our plan with specific steps and code examples gave me and Jasmine an easy understanding of what to do from start to finish. 

​* Communication helps build successful group projects: Texting back and forth before every git push and git pull helped us avoid merge conflicts and keep our 50/50 partnership.

​* Think like our intended audience/player: Testing our game really did help me catch that players couldn't see the color options, proving how important small user experience details are. As much as I trusted my partner in doing a good job, I am very glad that I double checked.

​* Always pay attention to class demos: Searching Google and seeing TikTok videos to solve a problem like for (Math.random() / Math.floor()) and paying attention during class demos helped turn a confusing concept I had into something I understand now and can use in the future!

[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)
