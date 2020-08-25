_**TODO:**_
1. _Incorporate materials from [programming notebooks](https://github.com/CE-Curriculum-Development/mat-cpe-1040)._  
2. _Rearrange for the _study, apply, present_ structure like [CE Learning Progression 006: Flip-flops](https://github.com/ivogeorg/https://github.com/ivogeorg/ce-learning-progression-006-flip-flops)._  
---

# CPE 1040 - Fall 2020

This is the first learning progression for the Fall 2020 installment of the CPE 1040 - Intro to Computer Engineering course at MSU Denver.

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

This progression will dive right into writing a short program for the micro:bit. Along the way, we will introduce and motivate elements of the programming language JavaScript. This progression will also serve as our first follow-through of our standard assignment workflow on Microsoft MakeCode and Github Classroom. Finally, we will introduce how to write [Markdown](https://en.wikipedia.org/wiki/Markdown) files  like this [README](README.md).

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

_In javascript, words like `true` and `false` are special keywords reserved by the language. The keywords `true` and `false` can only be used to represent a specific boolean value. More on booleans in the next step. Other examples of keywords that we have been using in our code include `boolean`, `if`, and `else`._

Conversely, if the condition provided within the parentheses is `false`, then the statements in the first block of code will be skipped. Instead, the code in the block after `else` will be run.

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

Code written as "`if`-`else`" statements is always executed in an either-or fashion. This means that only one of the two blocks will run. So the program will split and only one of the two blocks will be executed, this is known as a conditional "branch" in programming. 

#### 2. Apply

1. Create a new project in [makecode](https://makecode.microbit.org/) and delete the starter code.
1. Write a program that shows a heart icon if the condition is `true` and a butterfly if the condition is `false`.  
2. See what happens when you replace `true` or `false` with a mathematical relationship that will be evaluated as either true or false.
For example, a relationship in which one number is greater than (`>`) or less than (`<`) another.  

   If you are trying to express equality, you will need two equals signs: `==`. In programming languages, the double equals sign is used as a comparison operator. This means that it can only be used for the comparison of two values. A single equals sign (`=`) is used as an assignment operator. This means that it can only be used in the context of assigning a value to a variable. This concept is covered in more detail in the next step.
   
   Other comparison operators in javascript include `!=` for "not equal to", `>=` for "greater than or equal to", and `<=` for "less than or equal to." 

#### 3. Present

In the [Lab Notebook](README.md), include:
1. A short narrative about the experiment.  
2. Short video of your code from 5.2.2 running on your microbit.

In the repository [programs folder](./programs), include:
1. File `microbit-program-5-2-2.js` with the code you completed in task 5.2.2.

### Step 6: Data types

#### 1. Study

The files on a computer are distinguished from each other (eg, video files, audio files, photos, etc.) so that the computer knows how they will be used. In the same way, data that we store and use while programming needs to be distinguished so that the programming language understands how we want to use this data.

In a computer program, a variable is a symbol used to store data that is intended for use later on. To tell the programming language how we intend for our data to be used, we must give it [type](https://makecode.microbit.org/javascript/types). The types that come built into our programming language are known as "primitive types." One of these types is the "boolean," which has two possible states: `true` and `false`. Other common data types in javascript are numbers and strings.

The data stored in the variable can change as the program runs. For example, we may create a boolean with the value of `true`, and change it to `false` if a particular condition is met.

_In the program written in step 5, we used the keywords `true` and `false` to change the outcome of our program. These keywords are also known as "[literals](https://en.wikipedia.org/wiki/Literal_(computer_programming))," or more specifically "boolean literals." In contrast to a variable, the value of literal never changes._

```javascript
let myVar : boolean
```
Above is an example of how to declare a new variable in javascript. The keyword `let` indicates that the line that follows will be to declare a variable. The word after `let`, in this case `myVar`, will be interpretted as the name of this new variable. After the variable name, a colon must be placed before specifying the type of the new variable, in this case `boolean`.

With this code, we have declared our variable of a specific type. However, it has not been assigned any value. Since it has been declared as a `boolean`, its value can be either `true` or `false`. To assign this variable a value or change the value it currently holds, we would enter `myVar = true` or `myvar = false`.

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

1. Create a new project in [makecode](https://makecode.microbit.org/) and delete the starter code.
2. Start by declaring three variables: a `boolean`, a `number`, and a `string`. Ideally, variables should be given a descriptive name, however for this exercise names such as `bool1`, `num1`, and `string1` will suffice.  
   Assign each of the three variables a value. As in the example above, the variable declaration and assignment of an initial value can be done on the same line for each of these types.
   When declaring a number, simply change the type specification in the `boolean` example to `number`. After the equals sign, instead of `true` or `false`, enter a number of your choosing. For the [string](https://makecode.microbit.org/types/string) do the same, but remember to place your string inside of double quotation marks, e.g. `"Hello, World!"`.
3. Create an `if`-`else` statement with your `boolean`'s name as the conditonal. In the first block, make the microbit show your number with the line `basic.showNumber( num1 )`. In the second block, make the microbit show your string with the line `basic.showString( string1 )`. Be sure to change `num1` and `string1` if you created your variables with different names.
4. Run your code in the simulator, with the `boolean` set as `true`, then again with the `boolean` set to `false`.

#### 3. Present

In the [Lab Notebook](README.md), include:
1. A short narrative about the experiment.  
2. Short video of your code from 6.2.4 running on your microbit.

In the repository [programs folder](./programs), include:
1. File `microbit-program-6-2-4.js` with the code you completed in task 6.2.4.

### Step 7: Functions

#### 1. Study

In programming, a [function](https://makecode.microbit.org/javascript/functions) is a named block of code that can be written once and used repeatedly. As such, a function allows us to reuse code that we or someone else has written. We have been using built-in functions since step one. The line `basic.showIcon(IconNames.Heart)` uses the "showIcon" function.

The following program encapsulates our `if`-`else` blocks from step 6 in a function then calls that function:

```javascript
//Declares our named function with 1 argument of the type `boolean`.
function displayIcons(isHeart : boolean) { //This curly bracket is the opening delimiter, indicating the start of the code encapsulated in this function.
    if (isHeart) {
        basic.showIcon(IconNames.Heart)
        basic.pause(2000)
        basic.showIcon(IconNames.Butterfly)
    } else {
        basic.showIcon(IconNames.Angry)
        basic.pause(2000)
        basic.showIcon(IconNames.Snake)
    }
} //This curly bracket is the closing delimiter, indicating that everything afterward is not contained in this function.

displayIcons(true) //Calls our function.
```

The first line is called a signature. It contains the keyword `function` followed by the name of our function, in this case `displayIcons`. Inside the parentheses we place arguments. Arguments are local variables, meaning that the function is going to use them in its block of code. Like any other variable, arguments have types. Note that functions can also be declared with no arguments or many arguments.  

 Under the signature is the function's code block. Like all code blocks, it is composed of a series of statements.
 
The function's code block defines what we want our function to do. However, it does not actually execute the code in the function. For this we need to [call the function](https://makecode.microbit.org/javascript/call), or to tell javascript that we want to execute this function. The function call must include any arguments defined by the function's signature with the appropriate types. In our case, we can use boolean literals (`true` and `false`) or a boolean variable that has been assigned a value. 

#### 2. Apply

1. Create a new project in [makecode](https://makecode.microbit.org/) and delete the starter code.
1. Write a function called `addSubtract` that accepts three arguments: one boolean and two numbers. Each argument in your function signature will need to be separated by commas. You can use this code get you started: `function addSubtract (sign : boolean, ... ) {`. Replace the [ellipsis](https://en.wikipedia.org/wiki/Ellipsis) with the names and types of your other two variables.  
2. Inside the function write an `if`-`else` statement that adds the numbers if `sign` is `true` and subtracts the numbers otherwise. Store the result in a variable named `result`.  
3. Enter the line `basic.showNumber(result)` to show the result.  

   _Hint: This line only needs to be written once._
4. Call your function. Be sure to include all three arguments in your function call, and that their order matches the order in your function signature.

#### 3. Present

In the [Lab Notebook](README.md), include:
1. A short narrative about the experiment.  
2. Short video of your code from 7.2.4 running on your microbit.

In the repository [programs folder](./programs), include:
1. File `microbit-program-7-2-4.js` with the code you completed in task 7.2.4.

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
    basic.pause(2000)
})
```

#### 1. Study
It is common to repeat code that is already writen. This is done with loops. One of the ways that this is done is with the [forever loops.](https://makecode.microbit.org/reference/basic/forever)
The encapsulation of code within the function is repeated unless a button action has taken over the processor.
basic.forever(function()
{
// repeated code
}
)
is equvalent to  
while(true)
{
// repeated code
}
The only differnce is the function is taken in as a variable.
This makes basic.forever a first class function.

There are three ways to display the 5x5 led matrix expicity. 
 One of which is [Show LEDs](https://makecode.microbit.org/reference/basic/show-leds)
    This one alows one show the LEDs that one wants in a 5X5. 
 Another is [Show icon](https://makecode.microbit.org/reference/basic/show-icon)
     This displays a pre programed image which one could choose to display.
 Last is [clear screen](https://makecode.microbit.org/reference/basic/clear-screen)
      This clears the 5x5 LED matix.   

#### 2. Apply
 Write a program that uses a forever loop that displays a image on the 5x5 led matrix on the micro:bit for 2 seconds then is blank for 2 seconds.


#### 3. Present
Save your program in the programs folder as placeholder.js
Also record with of your working program[Yuja]{https://msudenver.yuja.com/} 



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
In the event a [button]{https://makecode.microbit.org/reference/input} a pressed all code is stopped and the code within the button press or pin number is executed. 
We call this an interput. 

#### 2. Apply
Use a button press to change the behaveior of a function that is already running. 



#### 3. Present
Save the program in the programs folder as placeholder.js
and make a video on yuja.


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
