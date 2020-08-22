# CPE 1040 - Fall 2020

This is learning progression 001 for the Fall 2020 installment of the course CPE 1040: Introduction to Computer Engineering at MSU Denver.

Table of Contents
=================

* [CPE 1040 \- Fall 2020](#cpe-1040---fall-2020)
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

This progression will dive straight into writing a short program for the micro:bit. Along the way, we will introduce and motivate elements of the programming language JavaScript. This progression will also serve as our first follow-through of our standard assignment workflow on Microsoft MakeCode and Github Classroom. Finally, we will introduce how to write [Markdown](https://en.wikipedia.org/wiki/Markdown) files like this [one](README.md) your are reading.

### Step 1: One-line program

#### 1. Study

`[<lernact-rd>]`Before we jump into `[<cept>]`_computer programming_, we should prepare ourselves with some useful definitions. What is a `[<cept>]`_computer_? A computer is a `[<cept>]`_machine_ which manupulates `[<cept>]`_numbers_. The basic components of a computer are `[<cept>]`_processor_, `[<cept>]`_memory_, `[<cept>]`_input_, and`[<cept>]`_output_. `[<cept>]`_Data_ enter the computer through its input devices and are saved to memory. The processor accesses the data from memory to manipulate them and writes them back to memory. When a result of the manipulation is ready, the data exits the computer through its output devices. 

We use computers in a variety of different ways: to edit text, to watch movies, to design machines, to transfer money, to solve equations, etc., etc.. Despite this enormous variety, computers only work on numbers. Any data that we wish to manipulate with a computer, we first `[<cept>]`_encode_ into numbers and only then we input into the computer. At the output of the computer, we may wish to `[<decode>]` the data to enable humans to interpret the result.

`[<LERNACT-ANS>]`**Question 1.1.1:** How is text encoded in the computer?
`[<LERNACT-ANS>]`**Question 1.1.2:** How is text intput into the computer?
`[<LERNACT-ANS>]`**Question 1.1.3:** How is text output by the computer?
`[<LERNACT-ANS>]`**Question 1.1.4:** What is JPEG and what does it do?
`[<LERNACT-ANS>]`**Question 1.1.5:** What kind of data is JPEG used for?

The two types of numbers computers work on are `[<cept>]`_integers_ (aka `[<cept>]`_whole numbers_) and `[<cept>]`_real numbers_. Because of the particular format adopted for the representation of real numbers, in computing they are usually called `[<cept>]`_floating-point numbers_. The set of `[<cept>]`_operations_ a computer can perform on numeric data is not large:
1. Arithmetic: addition, subtraction, multiplication, and division.  
2. Logical: AND, OR, NOT, etc..  
3. Comparisons: greater-than, less-than, equal-to, not-equal-to, etc..  
4. Memory: load/read, store/write, move, etc..  
5. Bit-level: shift-right, shift-left, rotate-right, rotate-left, etc..
6. Branch.

Binary...



`[<LERNACT-RD>]` We start with the simplest of programs, just a single line: 
```javascript
basic.showIcon(IconNames.Heart)
```




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

```javascript
if (true) {
    basic.showIcon(IconNames.Heart)
    basic.pause(2000)
    basic.showIcon(IconNames.Butterfly)
} else {
    basic.showIcon(IconNames.Angry)
    basic.pause(2000)
    basic.showIcon(IconNames.Snake)
}
   
if (false) {
    basic.showIcon(IconNames.Heart)
    basic.pause(2000)
    basic.showIcon(IconNames.Butterfly)
} else {
    basic.showIcon(IconNames.Angry)
    basic.pause(2000)
    basic.showIcon(IconNames.Snake)
}
```

#### 1. Study

#### 2. Apply

#### 3. Present



### Step 6: Data types

```javascript
let isHeart : boolean = true

if (isHeart) {
    basic.showIcon(IconNames.Heart)
    basic.pause(2000)
    basic.showIcon(IconNames.Butterfly)
} else {
    basic.showIcon(IconNames.Angry)
    basic.pause(2000)
    basic.showIcon(IconNames.Snake)
}
```

#### 1. Study

#### 2. Apply

#### 3. Present



### Step 7: Functions

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
   
displayIcons()
```

#### 1. Study

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
