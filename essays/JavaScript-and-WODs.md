---
layout: essay
type: essay
title: JavaScript and WODs
published: false
# All dates must be YYYY-MM-DD format!
date: 2019-01-18
labels:
  - JavaScript
  - WODs
---
 
My first experiences with JavaScript began with completing basic tutorials on the FreeCodeCamp website. Coming from a C/C++ background, JavaScript was not too difficult to pick up due to similarities in the syntax. The key differences I noticed include not having to specify a variable type (i.e. int, float, char, array). Instead, JavaScript can determine automatically what datatype is being used and adjusts accordingly. The same goes for creating and calling functions. While C requires a prototype, definition, and a call from main(), JavaScript can implement a function and call it almost seamlessly. 

In C
```c
#include <stdio.h> 
void some_func(void); //prototype 
void main() { 
    some_func(); //function call 
} 
void some_func(void) { //definition 
    printf("Hello, World!\n"); 
} 
```

In JavaScript
```js
function some_func() {
  console.log("notice the blank line before this function?");
}
some_func();
```

Also, I feel that this language is much more forgiving. It is easier to get away with sloppy code or missing semicolons because the compiler would accommodate for these omissions. I am still but a novice with JavaScript but feel that with more practice exercises, I will reach proficiency. 

In ICS314, once a week we do a Workout of the Day, or WOD for short. They are best described as in-class “quizzes” that test my proficiency in understanding a problem and coding in JavaScript. These WODs are grounded on "Athletic Software Engineering" which focuses on improving the speed at which a student writes code. 
