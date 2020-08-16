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

In the English language, a statement that begins with "if" is followed by a condition. If the condition is met, the next statement follows as a logical consequence. For example, in the sentence "If it starts to rain, then I will get wet." When it starts to rain the condition is met, so the latter part of the sentence necessarily follows.

A conditional statement in programming works in the same way. In the following example, the statement begins with "if," and the condition written within the parentheses is "true." Therefore, the statements inside the first block of code are run. The "else" statement can be thought of as an alternative to the "if" statement - it will only run if the condition for "if" is not met. Therefore, in this version of our code it will be ignored.

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

Conversely, if the condition provided within the parentheses is "false," then the statements in the first block of code will be skipped. Instead, the code in the block following "else" will be run.

```javascript
if (false) { //This block will be ignored
    basic.showIcon(IconNames.Heart)
    basic.pause(2000)
    basic.showIcon(IconNames.Butterfly)
} else { //This block will run since its only (implicit) condition is that the above block did not run.
    basic.showIcon(IconNames.Angry)
    basic.pause(2000)
    basic.showIcon(IconNames.Snake)
}
```

#### 2. Apply

#### 3. Present



### Step 6: Data types

#### 1. Study

The basic functions of a computer are to store and process electrical signals which represent binary numbers, 1's and 0's. These numbers are used to represent all of the information in our computers, from a simple text document to an HD movie.

To start thinking about the most basic type of data we can store, it is helpful to use the analogy of a light switch. When the switch is set to the higher power state it is on, which can be interpretted to mean true or 1. When the switch is flipped to the lower power state it is off, false, or 0. In this analogy, we can see that the same piece of data (the light switch being on or off) can be used to represent different kinds of information. 

As such, one of the most rudimentary types of data in javascript is a "Boolean," which can has two possible states: "true" and "false." We can apply this in the example that we used in the previous step to allow us to more easily switch which block of code in the "if-else" statement is run.

To declare a variable with a type (such as boolean) in javascript, the following template can be used: "let _name_ : _type_". The keyword "let" indicates that the line that follows will be to declare a variable. The "_name_" can be replaced with any name that is valid for the variable. And the "_type_" indicates how the stored data will be interpretted. For example, if we want to say that we have a variable called "isHeart," which will store a boolean, we would enter "let isHeart : boolean". With this code, we have declared our variable and given it a type, however it is not holding value. Since it has been declared as a boolean, we can either assign it a value of "true" or "false." To assign this variable a value or change the value it currently holds, we could enter "isHeart = true" or "isHeart = false".

Additionally, javascript allows us to declare our variable and assign it an initial value in one line by typing "let _name_ : _type_ = _value_". In our example, to declare "isHeart" as a boolean and assign it an initial value "true," we would type "let isHeart : boolean = true".

```javascript
let isHeart : boolean = true //Declares isHeart as a boolean and assigns it the initial value "true."

if (isHeart) { //Since "isHeart" is true, the code in the first block will run.
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

In programming, a function is a piece of code that can be written once and used repeatedly.

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
