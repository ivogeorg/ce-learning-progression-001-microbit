_**TODO:**_
1. _Incorporate materials from [programming notebooks](https://github.com/CE-Curriculum-Development/mat-cpe-1040)._  
2. _Rearrange for the _study, apply, present_ structure like [CE Learning Progression 006: Flip-flops](https://github.com/ivogeorg/https://github.com/ivogeorg/ce-learning-progression-006-flip-flops)._  
---

# CPE 1040 - Spring 2020

This is the first learning progression for the Fall 2020 installment of the CPE 1040 - Intro to Computer Engineering course at MSU Denver.

Table of Contents
=================

* [CPE 1040 \- Spring 2020](#cpe-1040---spring-2020)
* [Table of Contents](#table-of-contents)
  * [Learning Progression 001: micro:bit](#learning-progression-001-microbit)
    * [Step 1: One\-line program](#step-1-one-line-program)
      * [1\. Study](#1-study)
      * [2\. Apply](#2-apply)
      * [3\. Present](#3-present)
    * [Step 2: Comments](#step-2-comments)
      * [1\. Study](#1-study-1)
      * [2\. Apply](#2-apply-1)
      * [3\. Present](#3-present-1)
    * [Step 3: Sequential execution](#step-3-sequential-execution)
      * [1\. Study](#1-study-2)
      * [2\. Apply](#2-apply-2)
      * [3\. Present](#3-present-2)
    * [Step 4: Encapsulation](#step-4-encapsulation)
      * [1\. Study](#1-study-3)
      * [2\. Apply](#2-apply-3)
      * [3\. Present](#3-present-3)
    * [Step 5: Conditionals](#step-5-conditionals)
      * [1\. Study](#1-study-4)
      * [2\. Apply](#2-apply-4)
      * [3\. Present](#3-present-4)
    * [Step 6: Data types](#step-6-data-types)
      * [1\. Study](#1-study-5)
      * [2\. Apply](#2-apply-5)
      * [3\. Present](#3-present-5)
    * [Step 7: Functions](#step-7-functions)
      * [1\. Study](#1-study-6)
      * [2\. Apply](#2-apply-6)
      * [3\. Present](#3-present-6)
    * [Step 8: Loops](#step-8-loops)
      * [1\. Study](#1-study-7)
      * [2\. Apply](#2-apply-7)
      * [3\. Present](#3-present-7)
    * [Step 9: Loop function](#step-9-loop-function)
      * [1\. Study](#1-study-8)
      * [2\. Apply](#2-apply-8)
      * [3\. Present](#3-present-8)
    * [Step 10: Inside and outside of loops](#step-10-inside-and-outside-of-loops)
      * [1\. Study](#1-study-9)
      * [2\. Apply](#2-apply-9)
      * [3\. Present](#3-present-9)
    * [Step 11: Events](#step-11-events)
      * [1\. Study](#1-study-10)
      * [2\. Apply](#2-apply-10)
      * [3\. Present](#3-present-10)
    * [Step 12:  Flipping a boolean](#step-12--flipping-a-boolean)
      * [1\. Study](#1-study-11)
      * [2\. Apply](#2-apply-11)
      * [3\. Present](#3-present-11)



## Learning Progression 001: micro:bit

This progression will just familarize you with the environment we'll use: Microsoft Teams, Github Classroom, and Microsoft Makecode. All the activities will be shown and LA-ed in the lab, including submitting the assignment. Programming in JavaScript will be shown, as well as editing Markdown files, like this [README](README.md).

### Step 1: One-line program

```javascript
basic.showIcon(IconNames.Heart)
```

#### 1. Study

#### 2. Apply

#### 3. Present



### Step 2: Comments

```javascript
basic.showIcon(IconNames.Heart)       // this text ignored
```

#### 1. Study

#### 2. Apply

#### 3. Present



### Step 3: Sequential execution

```javascript
basic.showIcon(IconNames.Heart)
basic.pause(2000)
basic.showIcon(IconNames.Butterfly)
```

#### 1. Study

#### 2. Apply

#### 3. Present



### Step 4: Encapsulation

```javascript
{
    basic.showIcon(IconNames.Heart)
    basic.pause(2000)
    basic.showIcon(IconNames.Butterfly
}
```

#### 1. Study

#### 2. Apply

#### 3. Present



### Step 5: Conditionals

#### 1. Study

In the English language, a statement that begins with "if" is followed by a condition. If the condition is met, the next statement follows as a logical consequence. For example, in the sentence "If it starts to rain, then I will get wet." The condition is that "it starts to rain." When the condition becomes true, the second part of the sentence - "I will get wet" - also becomes true.

In javascript, we use statements that begin with `if` in the same way. Take a look at the following code:

```javascript
if (true) { //This condition is always true, so the code in this block will run.
    basic.showIcon(IconNames.Heart)
    basic.pause(2000)
    basic.showIcon(IconNames.Butterfly)
} else { //Everything in this block is ignored because the first "if" statement was true.
    basic.showIcon(IconNames.Angry)
    basic.pause(2000)
    basic.showIcon(IconNames.Snake)
}
```

In the above example, the statement begins with `if`, and the condition written within the parentheses is `true`. Therefore, the statements inside the first block of code are run. The `else` block can be thought of as an alternative to the `if` statement - it will only run if the condition for `if` is not met. Therefore, in this version of our code it will be ignored.

_In javascript, words like `true` and `false` are special keywords reserved by the language. These keywords can only be used to represent a specific boolean value. More on booleans in the next step._

Conversely, if the condition provided within the parentheses is `false`, then the statements in the first block of code will be skipped. Instead, the code in the block following `else` will be run.

```javascript
if (false) { //This block will be ignored.
    basic.showIcon(IconNames.Heart)
    basic.pause(2000)
    basic.showIcon(IconNames.Butterfly)
} else { //The only condition for this block of code to run, is that the above block did not run.
    basic.showIcon(IconNames.Angry)
    basic.pause(2000)
    basic.showIcon(IconNames.Snake)
}
```

Code written as "`if`-`else`" statements is always executed in an either-or fashion. This means that only one of the two blocks will run. So the program will split and only one of the two possible outcomes will be executed, this is known as a conditional "branch" in programming. 

#### 2. Apply

1. Write a program that shows a heart icon if the condition is true and a butterfly if the condition is false.  
2. See what happens when you replace `true` or `false` with a mathematical relationship that will be evaluated as either true or false.
For example, a relationship in which one number is greater than (`>`) or less than (`<`) another.  

   Note that if you are trying to express equality, you will need two equals signs: `==`.

#### 3. Present

In the [Lab Notebook](README.md), include:
1. A short narrative about the experiment.
2. Short video of the operation of your code in 2.2.2.

In the repository [programs folder](./programs), include:
1. File `microbit-program-2-2-2.js` with the code you used in task 2.2.2.

### Step 6: Data types

#### 1. Study

To start thinking about the most basic type of data we can store, it is helpful to use the analogy of a light switch. When the switch is set to the higher power state, it is on, which can be interpretted to mean true or 1. When the switch is flipped to the lower power state, it is off, false, or 0. In this analogy, we can see that the same piece of data (the light switch being on or off) can be used to represent different kinds of information. 

One of the most rudimentary types of data in javascript is a "Boolean," which has two possible values: `true` and `false`. We can apply this in the example that we used in the previous step to switch which block of code in the "`if`-`else`" statement is run.

A variable is a symbol that is used to represent information. In a computer program, a variable can store information that is intended for use later on. The information stored in the variable can change as the program runs. For example, we may create a boolean with the value of `true`, and change it to `false` if a particular condition is met.

In the previous step, we used the boolean literals `true` and `false` to change the outcome of our program. A boolean is also a [data type](https://makecode.microbit.org/javascript/types) for a variable. So, when a variable is declared, we can use the keyword `boolean` to indicate that it will store one of two possible boolean values.

```javascript
let myVar : boolean
```

Above is an example of how to declare a new variable in javascript. The keyword `let` indicates that the line that follows will be to declare a variable. The word after `let`, in this case `myVar`, will be interpretted as the name of this new variable. After the variable name, a colon must be placed before giving the new variable a type, in this case `boolean`.

With this code, we have declared our variable and given it a type, however it has not been assigned any value. Since it has been declared as a `boolean`, its value can be either `true` or `false`. To assign this variable a value or change the value it currently holds, we would enter `myVar = true` or `myvar = false`.

Javascript also allows us to declare our variable and assign it an initial value in one line. To declare `myVar` as a `boolean` and give it an initial value of `true`, we would enter `let mVar : boolean = true`.

```javascript
let isHeart : boolean = true //Declares isHeart as a boolean and assigns it the initial value `true`.

if (isHeart) { //Since `isHeart` is true, the code in the first block will run.
    basic.showIcon(IconNames.Heart)
    basic.pause(2000)
    basic.showIcon(IconNames.Butterfly)
} else { //The "else" block will be ignored.
    basic.showIcon(IconNames.Angry)
    basic.pause(2000)
    basic.showIcon(IconNames.Snake)
}
```

#### 2. Apply

#### 3. Present



### Step 7: Functions

#### 1. Study

In programming, a function is a block of code that can be written once and used repeatedly. As such, a function allows us to reuse code that we or someone else has written. We have been using built-in functions since step one, `basic.showIcon(IconNames.Heart)` 

```javascript
function displayIcons(isHeart : boolean) {
    if (isHeart) {
        basic.showIcon(IconNames.Heart)
        basic.pause(2000)
        basic.showIcon(IconNames.Butterfly)
    } else {
        basic.showIcon(IconNames.Angry)
        basic.pause(2000)
        basic.showIcon(IconNames.Snake)
    }
}
   
displayIcons(true)
```

#### 2. Apply

#### 3. Present



### Step 8: Loops

```javascript

while (true) {
    basic.showIcon(IconNames.Heart)
    basic.pause(2000)
    basic.clearScreen()
})
```

#### 1. Study

#### 2. Apply

#### 3. Present



### Step 9: Loop function

```javascript

basic.forever(function () {
    basic.showIcon(IconNames.Heart)
    basic.pause(2000)
    basic.clearScreen()
})
```

#### 1. Study

#### 2. Apply

#### 3. Present



### Step 10: Inside and outside of loops

```javascript
let isHeart : boolean = true

basic.forever(function () {
    if (isHeart) {
        basic.showIcon(IconNames.Heart)
    } else {
        basic.showIcon(IconNames.Butterfly)
    }
    basic.pause(2000)
    basic.clearScreen()
})
```

#### 1. Study

#### 2. Apply

#### 3. Present



### Step 11: Events

```javascript
let isHeart : boolean = true

input.onButtonPressed(Button.A, function () {
    if (isHeart) {
        isHeart = false
    } else {
        isHeart = true
    }
})

basic.forever(function () {
    if (isHeart) {
       basic.showIcon(IconNames.Heart)
    } else {
       basic.showIcon(IconNames.Butterfly)
    }
    basic.pause(2000)
    basic.clearScreen()
})
```

#### 1. Study

#### 2. Apply

#### 3. Present



### Step 12:  Flipping a boolean

```javascript
let isHeart : boolean = true

input.onButtonPressed(Button.A, function () {
    uprightHeart = !uprightHeart
})

basic.forever(function () {
    if (isHeart) {
        basic.showIcon(IconNames.Heart)
    } else {
        basic.showIcon(IconNames.Butterfly)
    }
    basic.pause(2000)
    basic.clearScreen()
})
```

#### 1. Study

#### 2. Apply

#### 3. Present
