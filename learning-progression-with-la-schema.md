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
[[toc](#table-of-contents)]

#### 1. Study
[[toc](#table-of-contents)]

`[<lernact-rd>]`Before we jump into `[<cept>]`_computer programming_, we should prepare ourselves with some useful definitions. What is a `[<cept>]`_computer_? A computer is a `[<cept>]`_machine_ which manupulates `[<cept>]`_numbers_. The basic components of a computer are `[<cept>]`_processor_, `[<cept>]`_memory_, `[<cept>]`_input_, and`[<cept>]`_output_. For example, the two buttons of the micro:bit are input devices and the 5x5 matrix of red `[<cep>]`_LEDs_ is an output device. `[<cept>]`_Data_ enter the computer through its input devices and are saved to memory. The processor accesses the data from memory to manipulate them and writes them back to memory. When a result of the manipulation is ready, the data exits the computer through its output devices. 

We use computers in a variety of different ways: to edit text, to watch movies, to design machines, to transfer money, to solve equations, etc., etc.. Despite this enormous variety, computers only work on numbers. Any data that we wish to manipulate with a computer, we first `[<cept>]`_encode_ into numbers and only then we input into the computer. At the output of the computer, we may wish to `[<decode>]` the data to enable humans to interpret the result.

`[<lernact-ans>]`**Question 1.1.1:** How is text encoded in the computer?  
`[<lernact-ans>]`**Question 1.1.2:** How is text intput into the computer?  
`[<lernact-ans>]`**Question 1.1.3:** How is text output by the computer?  
`[<lernact-ans>]`**Question 1.1.4:** What is JPEG and what does it do?  
`[<lernact-ans>]`**Question 1.1.5:** What kind of data is JPEG used for?  

The two types of numbers computers work on are `[<cept>]`_integers_ (aka `[<cept>]`_whole numbers_) and `[<cept>]`_real numbers_. Because of the particular format adopted for the representation of real numbers, in computing they are usually called `[<cept>]`_floating-point numbers_. The set of `[<cept>]`_operations_ a computer can perform on numeric data is not large:
1. `[<cept>]`_Arithmetic_: `[<cept>]`_addition_, `[<cept>]`_subtraction_, `[<cept>]`_multiplication_, and `[<cept>]`_division_. These operations create new data from already existing data by applying _arithmetic functions_ to pairs of numbers.    
2. `[<cept>]`_Logical_: `[<cept>]`_AND_, `[<cept>]`_OR_, `[<cept>]`_NOT_, etc.. These operations create new data from already existing data by applying _logical function_ to single numbers or pairs of numbers.   
3. `[<cept>]`_Comparisons_: `[<cept>]`_greater-than_, `[<cept>]`_less-than_, `[<cept>]`_equal-to_, `[<cept>]`_not-equal-to_, etc.. These operations compare pairs of numbers.    
4. Memory: `[<cept>]`_load/read_, `[<cept>]`_store/write_, `[<cept>]`_move_, etc.. These operations move data around between different `[<cept>]`_locations in memory_.    
5. `[<cept>]`_Bit-level_: `[<cept>]`_shift-right_, `[<cept>]`_shift-left_, `[<cept>]`_rotate-right_, `[<cept>]`_rotate-left_, etc.. These operations create new data from existing data by manipulating single numbers on the bit level.  
6. `[<cept>]`_Branch_. These operations cause the processor to jump from one place in a program to another, providing the funcamental mechanism for `[<cept>]`_functions_, `[<cept>]`_conditional execution_, and `[<cept>]`_loops_.  
For example, this is the [summary](https://developer.arm.com/documentation/ddi0432/c/programmers-model/instruction-set-summary) of the `[<cept>]`_instruction set_ of the processor of the micro:bit (that is, the operations it can perform).  

All data in a computer is represented in the `[<cept>]`_binary number system_, which has only two symbols, 0 and 1. These are called `[<cept>]`_bits_. All numbers are represented as sequences of 0s and 1s (aka bit patterns). The lengths of these sequences are always `[<cept>]`_powers_ of 2: 8, 16, 32, 64, 128.

`[<lernact-ans>]`**Question 1.1.6:** If the 8-bit pattern `00001011` represents 11<sub>10</sub>, what number in `[<cept>]`_decimal_ does the bit pattern represent if it is _shifted one bit to the left_? _Note: Shifting to the left is performed by dropping the leftmost bit and filling on the right with 0s._    
`[<lernact-ans>]`**Question 1.1.7:** If the 8-bit pattern `00001011` represents 11<sub>10</sub>, what number in `[<cept>]`_decimal_ does the bit pattern represent if it is _shifted one bit to the right_? _Note: Shifting to the right is performed analogously to shifting to the left._    

`[<lernact-rd>]` Now we are ready to jump into programming. We start with the simplest of programs, just a single line: 
```javascript
basic.showIcon(IconNames.Heart)
```
We will explain everything about this line of `[<cept>]`_code_ (meaning: line(s) of a programming language), but first let's say what it does when `[<cept>]`_compiled_ and written to the program memory of the micro:bit: a representation of a heart is lit up on the LEDs and remains lit until the micro:bit is reprogrammed or it's '[<cept>]`_power supply_ is disconnected.

This single line introduces us to several important computer programming concepts:
1. A line of code is compiled (meaning: translated) into a sequence of processor instructions (aka machine instructions) which the processor `[<cept>]`_executes_ (meaning: performs).  
2. `showIcon` is the name of a function, which is an `[<cept>]`_encapsulation_ of several lines of code. The lines can made to be executed by only specifying the function name. The function is said to be `[<cept>]`_called_. More on functions [below](#step-7-functions).  
3. A function may or may not have `[<cept>]`_arguments_, which are data that are `[<cept>]`_passed_ (meaning: given) to the function, which needs them to execute its code. The arguments, if any, are specified between the _parentheses_ after the function name. Every function call, wether it has arguments or not, **requires** the two parentheses `()`. Otherwise, this line of code will not be interpreted as a function call.  
4. The argument of the function `showIcon` is `IconNames.Heart`. This is a name of an icon, which is a pattern of lit and dark LEDs for the 5x5 LED matrix of the mcirobit. The named icons are already defined and stored in the memory of the microbit when used. The collection of predefined icons is represented by an [`enum`](https://www.typescriptlang.org/docs/handbook/basic-types.html#enum) data type, called `IconNames`. More on data types [below](#step-6-data-types).   
5. Finally, `basic` is the name of a `[<cept>]`_package_ of functions (aka `[<cept>]`_library_). Functions are always packaged together according to their purpose. For example, in the [MakeCode editor](https://makecode.microbit.org/#editor) the packages are listed in a column bar on the left of the code area (`basic`, `input`, `radio`, `led`, etc.) and clicking on any of the package names opens the list of available package functions with documentation.  

#### 2. Apply
[[toc](#table-of-contents)]


#### 3. Present
[[toc](#table-of-contents)]



### Step 2: Comments
[[toc](#table-of-contents)]

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
