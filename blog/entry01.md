# Process Writeup 

## Name: Stacy M.
## Period: 1
## Course: Arrays
### Concept: Nested Arrays & Array Methods (`.push()`, `.pop()`, `.shift()`, `.unshift()`)

---

## Context

In this SEP course, with the help of freeCodeCamp lessons, classwork, and collaborating with my partner Emmanuel on our **Grocery List Coding Challenge** repository on our codespaces, I learned a lot on how to work with more advanced array structures, including nesting one array within another. I also learned how to manipulate array data using fundamental methods.

* Nested Arrays: Putting arrays inside other arrays to store structured data together.
* `push()`: Appends one or more items to the end of an array.
* `pop()`: Removes the last item from an array and returns it.
* `shift()`: Removes the first item from the beginning of an array.
* `unshift()`: Adds one or more items to the beginning of an array.
* `if` Statements: Used to check conditions (like ensuring an item exists before running an alert or updating a specific index).

### Code Examples I Practiced 👩🏻‍💻💡

Here are code examples directly from our grocery list project, Taylor Swift inspired code, amd`if` statements:

```javascript
// 1. Nesting one array within another 
const favoriteEras = [["Taylor Swift", 13], ["Folklore", 2]];

// 2. Using .push() to add an item
var newItem = prompt("Type an item you would like to add");
groceryList.push(newItem);

// 3. Using .pop() and an `if` statement to delete the last item
var removedItem = groceryList.pop();
if (removedItem) {
  alert("Removing: " + removedItem);
}

// 4. Using `if` with logical operators (`&&`) to change a specific item
var changeItem = prompt("Which item do you want to change?");
var newItem = prompt("What would you like to change it to?");
if (changeItem && newItem) {
  groceryList[changeItem - 1] = newItem;
}

```
## Challenges & Confusions 🤔

Missing almost a week of class made this topic really challenging because I missed the core basics, which led to a tough initial quiz score of a 4/10. Trying to wrap my head around nested arrays and keeping track of what push(), pop(), shift(), and unshift() did felt completely overwhelming. However, to lock those methods into my memory,

I created my own visual mental tricks: 🧠📚⚡

​1.Push: Pushing someone to the back of a grocery line (adds to the end). ⤷ 🛒

​2.Pop: Popping a balloon at the end of something (removes from the end). 🎈📍
 
3.Shift / Unshift: Working strictly with the front (beginning) of the list. ⫶☰

Me and my partner also ran into technical hurdles during our group project. When Emmanuel and I tried to push and pull our code changes on GitHub or check our work on the HTTP server, nothing was showing up. We first tried to solve the problems ourselves, however we later realized it was better if we asked Mr. Mueller for help. To the naked eye, we couldn't spot any errors at first, and even Mr. Mueller didn't see anything wrong right away. He initially thought we might have accidentally modified code in the the protected "do not change" section or missed placed a parenthesis. To get to the bottom of it, Mr. Mueller ended up running our code through an external site, it just turned out to be a small syntax mistake. Proving how much small details matter in coding. Additionally, when we hit Task 2 and Task 3, I had to figure out if statements although I had never been formally taught in class; and just learned a little on Slack!

## Helpful tips and tricks I used to turn my grade around!‧₊˚⏱٠࣪⋆💻₊💯˚

​To turn my grade around, I studied hard using flashcards on the subject on Quizlet, reviewed my notes carefully, and put in serious extra time, including waking up two hours early before school to study for the quiz to run through practice questions on FFCC.

## Takeaways 𓂃✍︎

​1.Determination Pays Off: Even though missing a week dropped my first quiz score to a 4/10, staying determined, waking up early, and studying hard helped me drastically improve my performance.

2.Memory Hacks Help: Creating real-world visual associations makes technical methods like push and pop much easier to recall during tests and fun.

​3.Resourcefulness & Collaboration: Working closely with my partner Emmanuel, asking Mr. Muller for debugging help when we need it, using Slack when stuck, and practicing with flashcards are essential tools for overcoming obstacles. There is always help and answers through resources.

​4.Details Matter A LOT: Debugging server and syntax issues taught me to pay close attention to small things like parentheses. It is crucial to keep an eye, as an error can be hidden in plain sight!



​

