# Functions Writeup 

## Name: Stacy M.
## Period: 1
## Course: Functions
## Concept: Basic Functions, Parameters, and Return Values

---

## Context 

In this SEP course, through video lessons, classwork, DeltaMath practice, ScratchJR, and collaborating with my partner Henson on our Century Coding Challenge (js-2028-century-cc-group-19) repository in Codespaces, I learned how to structure reusable block code using functions. I learned how functions organize code to improve readability and reusability, how parameters pass input, and how return statements send data back out.  

* Wrapping block code in a named function so it can be called multiple times without repeating code (for example repeating a song chorus without writing 12 console.log lines)
  
* Parameters & Arguments: Inputs passed into functions (like year, name, or books) that make function outputs customizable!

* Return Values: Using return values to send a value back to where the function was called.

* Function Helper Calls: Calling helper functions inside other functions (such as calling `getCentury(year)` inside `printYearCentury(year)`)


## Code Examples I Practiced

Here are real code examples directly from our Century Coding Challenge group project 

```javascript

// TASK 1:
// returns the century of the year inputted
// assume input year ≥ 1
// Ex: 1 returns 1
// Ex: 99 returns 1
// Ex: 100 returns 2
// Ex: 305 returns 4
// Ex: 2020 returns 21
function getCentury(year) {
  // HINT: Math.floor() or Math.ceil()
  /* code below 👇 */
    return Math.ceil((year + 1)/100)
  /* code above 👆 */ 
  
}
// use these to make sure your function above is working properly
console.log(getCentury(1)); // 1
console.log(getCentury(99)); // 1
console.log(getCentury(100)); // 2
console.log(getCentury(305)); // 4
console.log(getCentury(2020)); // 21

// DO NOT EDIT THIS FUNCTION
// IT IS ALREADY DONE!!!
// returns the suffix of a number
// ex: 1 returns "st" (because 1st = firST)
// ex: 2 returns "nd" (because 2nd = secoND)
// ex: 3 returns "rd" (because 3rd = thiRD)
function suffix(i) {
    var j = i % 10,
        k = i % 100;
    if (j == 1 && k != 11) {
        return "st";
    }
    if (j == 2 && k != 12) {
        return "nd";
    }
    if (j == 3 && k != 13) {
        return "rd";
    }
    return "th";
}


// TASK 2:
// prints to the document "The year X is in the Y century"
// Ex: "The year 2020 is in the 21st century."
// Ex: "The year 1900 is in the 20th century."
// Ex: "The year 1 is in the 1st century."
function printYearCentury(year) {
  /* code below 👇 */
  var century = getCentury(year);
  document.write("The year"+year+"is in the" + century + "th century.");
  /* code above 👆 
  document.write("<br>");

```


## Challenges & Confusions 🧐

​Working through Task 2 during our group project was really tough at first because I struggled to understand how helper functions passed values back and forth.

​Key Technical Problems & How I Solved Them:

1. **Understanding Task 2:** When working on Task 2, I wasn't sure how getCentury(year) worked inside printYearCentury(year). I asked my partner Henson for help, but I was still confused. He asked Mr. Mueller, who explained it to us. It started making more sense, but to really lock it in, I researched extra examples on Google and checked past homework to figure it out step-by-step.

2. **Git & Collaboration Syncing:** Henson and I tried to split Task 3 evenly (50/50) with clear communication, but we ran into GitHub sync confusion regarding whether our latest changes were pushed or pulled properly. 

3. **Casual Demo Confusion:** During a casual demo led by my classmate Emmanuel, seeing different solutions made me feel confused initially. However, listening to questions asked by other classmates helped clear up my own doubts!!


## Visual Models and Videos that Helped! 🧠💡

- Scratch Jr Orange Cat: My teacher showed us a Scratch Jr example with the orange cat. Stacking a long, repetitive trail of motion blocks takes up way too much space. Wrapping those instructions into a single custom block (a function) makes the code much shorter, cleaner, and easier to read.

- Song Chorus: Instead of typing 12 console.log lines for repeated chorus lyrics, defining a chorus function once.
[Song Chorus Yt Video:](https://classroom.google.com/c/ODc4NTk4NzQ3NDMx/m/ODkyNzI2ODQ4NzM0/details)

​
## My Takeaways

**Functions Make Code Clean & Reusable:** Instead of repeating code over and over, wrapping it in functions keeps it organized and readable.  


​**Resourcefulness When Stuck:** When class explanations or casual demos don't fully click right away, combining teacher help,past code homeworks, and Google searches leads to solutions. 


​**Communication in Partner Work:** Clear communication and checking Git pushes/pulls with partners like Henson are key to making sure group tasks are completed smoothly. 


   



