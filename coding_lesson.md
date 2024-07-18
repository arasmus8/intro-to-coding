# Intro to Coding

## Resources and More Info

These are some great resources you can use to learn more about coding:

- [code.org](https://code.org/): lessons and projects for all ages, including hands-on, offline activities
- [Coding a Lego Maze](https://researchparent.com/coding-a-lego-maze/): Practice coding with paper and Legos
- [Hour of Code](https://hourofcode.com/us): Fun activities and videos to learn computer science
- [Scratch](https://scratch.mit.edu/): Learn to code with visual blocks
- [Khan Academy](https://www.khanacademy.org/computing/computer-programming)

## Instructions

Instructions are how we tell the computer to do something. All coding is made
up of instructions, and the computer will follow the instructions, one-by-one
in order. [^1]

Here are some examples of instructions:

`5 + 5` _do some math_

`print('Hello!')` _call a **function**_

`x = 5` _assign to a **variable**_

`if (x > 3)` _check a condition_


[^1]: Computers don't actually run things one-by-one in order, but they are build
in a way to make it look like they do.

## Variables

Think of a variable like a box or a folder - it has a name (like the label on the
box), and a value (the contents of the box).

```
# assign the variable 'x' to have the value 10
x = 10
```

You can change the contents.

```
# assign the variable 'x' to have the value 10
x = 10

# change the value of x to 20
x = 20
```

You can also add more labels on the box - every label will still be on the same box, and
will have the same contents.

```
x = 10 # Set x to 10
y = x  # y is the same as x
z = y  # what will z be?

x = 20 # now what will z be?
```

Variables are useful, because you can pass them around and use them in other instructions.

## Functions

A function is a set of instructions that can be called from somewhere else. It can pass
the results of those instructions back to the code that called it.

```
function doSomething () {
    return 5 + 5
}

x = doSomething() # What value does x hold?
```

Functions can be given _parameters_ that they can use in the instructions they follow.

```
function addOne (x) {
    return x + 1
}

y = addOne(1) # What value does y hold?

function add (a, b) {
    return a + b
}

x = 6
y = 3

z = add (x, y) # What value does z hold?
```
Functions can call other functions.

```
function sayHello (name) {
    print('Hello ', name, '!')
}

function greetEveryone () {
    everyone = ['Alice', 'Bob', 'Candace', 'David']
    everyone.forEach(sayHello)
}

greetEveryone() # What happens?
```

## Loops

When you need to do something similar over and over, you can use a loop.

```
x = 10
while (x > 0) {
    print(x, '...')
    x = subtractOne(x)
}
# What will this print out?
```

## Conditions

Sometimes, you want to do something or not based on the value of a variable.
For these situations, you can use a conditional.

```
function pluralizer (name, howMany) {
    if (howMany == 1) {
        print('one ', name)
    } else if (howMany == 0) {
        print('no ', name, 's')
    } else {
        print(howMany, ' ', name, 's')
    }
}

pluralizer('apple', 3)     # What gets printed?
pluralizer('banana', 0)
pluralizer('candybar', 1)
```
