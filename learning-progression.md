_**TODO:**_
1. _Incorporate materials from [programming notebooks](https://github.com/CE-Curriculum-Development/mat-cpe-1040)._  
2. _Rearrange for the _study, apply, present_ structure like [CE Learning Progression 006: Flip-flops](https://github.com/ivogeorg/https://github.com/ivogeorg/ce-learning-progression-006-flip-flops)._  
---

# CPE 1040 - Spring 2020

This is the first learning progression for the Fall 2020 installment of the CPE 1040 - Intro to Computer Engineering course at MSU Denver.

Table of Contents
=================

**TODO**


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
