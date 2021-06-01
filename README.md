# Objectives
1. Gain experience using git via your CLI and Visual Studio Code (VSCode) Source Control
2. Gain experience writing and executing non-web server Node.js JavaScript code
3. Practice refactoring JavaScript code

# Technologies Used
- Terminal
- VSCode

# Part 1
Complete [Lab 2](https://pozawa1.github.io/cit281-lab2/)

# Part 2
Refractor p1-random.js from Project 1 to isolate code into functions, eliminate global variables, and make code self-documenting by variable and function name choices.
```
function getRandomInteger(min, max) {
    return Math.floor(Math.random() * (max - min) + min);
}

function getRandomString() {
    const alphabet = "abcdefghijklmnopqrstuvwxyz".split("");
    let result = "";
    for (let i = 0; i < getRandomInteger(5, 26); i++) {
        result += alphabet[getRandomInteger(1,alphabet.length-1)];
    }
    return result; 
}
console.log(getRandomString());
```

Create a new function getRandomLetter() that will return a single, random, lowercase letter.
```
function getRandomLetter() {
    const alphabet = "abcdefghijklmnopqrstuvwxyz".split(""); 
    
    for (let i = 0; i < 1; i++) {
        return alphabet[Math.floor(Math.random() * alphabet.length)]
    }
}
console.log(getRandomLetter());
```

Create a new function getRandomString(minLength, maxLength) that will return the random length string. 
```
function getRandomString() {
    const alphabet = "abcdefghijklmnopqrstuvwxyz".split("");
    let result = "";
    for (let i = 0; i < getRandomInteger(5, 26); i++) {
        result += alphabet[getRandomInteger(1,alphabet.length-1)];
    }
    return result; 
}
console.log(getRandomString());
```

Create a new function called getSortedString(string) that will return a string in ascending order.
```
function getSortedString(string) { return string.split("").sort().join(""); }
console.log(getSortedString("xpacd")); //Returns "acdpx"
```

# Part 3
Replace all of the function definitions with function expressions.

# Part 4
Create a .gitignore file to ignore .txt and .bak files.

![p2-vscode-diff](https://user-images.githubusercontent.com/83732149/120234597-338a5800-c20d-11eb-8f12-44967bbfe450.png)

[Source Code](https://github.com/pozawa1/cit281-p2/blob/main/source-code-p2)

[Return to Homepage](https://pozawa1.github.io/)
