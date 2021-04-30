# Notice

Welcome to Step Through Code. The following documents in the folder have titles of the format A.B; Chapters represented by A, and sections represented by B.

If there are any errors, please kindly raise an issue on GitHub.

Thank you!
# Preface

Step through code is for regular people who are looking to get into coding. This tutorial will start from low-level programming to higher-level programming because of the importance of learning the basics of programming before doing higher-level projects like web development, machine learning, and other cool things.
# Glossary

## 1 - Low-level concepts

1.  [Computers](#computers)
2.  [Binary Numbers](#binary-numbers)
3.  [Arithmetic](#arithmetic)
4.  [Logic Gates](#logic-gates)
5.  [Machine Code](#machine-code)

## 2 - Low-level machines

1.  [Turing Machines]()
2.  [State Machines]()
3.  [Stack Memory]()
4.  [Stack Machines]()

## 3 - Low-level data structures

1.  [Boolean Values]()

2.  [Unsigned Integers]()
3.  [Signed Integers]()
4.  [Floating Points]()
5.  [Arrays]()
6.  [Pointers]()

## 4 - Low-level data structures

1.  [Heap Memory]()
2.  [Linked Lists]()
3.  [Hashing]()
4.  [Hash Maps]()
5.  [Better Hash Maps]()
6.  [Trees]()
# Computers

## What is a computer?

A computer is a machine capable of storing data and performing calculations with it. In other words, your digital watch, the calculator of yours you use in your math class, and many other things around you are computers.

## How do modern computers work?

All modern computers use electricity and magnetism to store information and perform calculations on it. I will not go into details because this is beyond my field of knowledge.

# Binary Numbers

## The human counting system
Humans use a counting system of base-10. It means that we have ten digits.
```
0 1 2 3 4 5 6 7 8 9
```

From a mathematical standpoint, the following will represent the number 7473.

<img src="https://render.githubusercontent.com/render/math?math=7*10^3 %2b 4*10^2 %2b 7*10^1 %2b 3*10^0 = 7473">

The above is not easy to read and very hard to write. We will use programming math grammar.

```
7 * 10**3 + 
4 * 10**2 + 
7 * 10**1 +
3 * 10**0 = 7473

7 * 1000 + 
4 * 100 + 
7 * 10 +
3 * 1 = 7473

7000 + 400 + 70 + 3 = 7473

So base-10 7473 in base-10 is 7473
```

> `*` is the multiplication operator
> `**` is the power operator. 

## The nowadays computer counting system
Computers use a counting of base-2 because electricity can only represent two different states: open and closed circuits.

Open is zero, and closed is one.

This counting system is called binary.

> Little confused?
> In your electricity and magnetism class, you learned that there is no current when the circuit is open, and a current can pass if it is closed. 

Here is the math behind the base-2 counting system. In this example, we are trying to write the base-10 number 13 in base-2.
```
1 * 2**3 + 
1 * 2**2 +
0 * 2**1 +
1 * 2**0 = 13

1 * 8 + 
1 * 4 +
0 * 2 +
1 * 1 = 13

8 + 4 + 0 + 1 = 13

So base-10 13 in base-2 is 1101
```

> Notice that the value of the first character of every line separated by empty lines is the values used in the writing of the base-x formatted number.
# Arithmetic

## If you can do regular arithmetic, you can do it in binary.

Additions
```
Sum of base-2 10 and base-2 01

  10
+ 01
= 11

# This is a comment
# bx will be the abbreviation of base-x, so b2 is base-2

Sum of b2 101 and b2 001

  101
+ 001
= 110

Sum of b2 011 and b2 011

  011
+ 011
= 110
```

You got it, right? It really is the same.# Logic Gates

## What are they?

Logic gates are the basic building blocks for everything that has to do with logic in a computer.

## What do they do?

They take one or two boolean values as input and output one boolean value.

> A boolean value is a true or a false. It is often respectively represented with 1 and 0.

```
true = 1
false = 0
```

## AND gate

The AND gate takes two inputs and outputs one only if both inputs are ones.

```
# & is the AND gate operator

1 & 1 = 1
0 & 1 = 0
1 & 0 = 0
0 & 0 = 0
```

## OR gate

The OR gate takes two inputs and outputs one if either of the inputs is one.

```
# | is the OR gate operator

1 | 1 = 1
0 | 1 = 1
1 | 0 = 1
0 | 0 = 0
```

## XOR gate

The XOR gate (exclusive OR gate) takes two inputs and outputs one only if one of its inputs is one.

```
# ^ is the OR gate operator

1 ^ 1 = 0
0 ^ 1 = 1
1 ^ 0 = 1
0 ^ 0 = 0
```

## NOT gate

The NOT gate takes a single input and outputs one when the input value is zero. Otherwise, it outputs one.

```
# ~ is the OR gate operator

~1 = 0
~0 = 1
```

> The AND, OR, and XOR gates are binary operators, meaning they take two inputs. NOT is a unary operator because it only takes one input value.

Great, you now understand all the logic gates in a computer. Think about them and see how you can create a summation logic gate circuit with them.# Machine Code

## What is code?

A code is a language where things are not explicitly defined.
In other words, I would call it:

> Language for machines where things are not explicitly defined for humans because they do not understand it.

## Our machine code

```
let x and y be 0

machine code A: set y to 1
machine code B: increase x by y
machine code C: jump back to the previous instruction
```

## Our program with our machine code

```
A
B
C
```

This program will loop forever and never stop.

-   We set the variable y to one.
-   The variable x will increase by y each time we execute instruction B.
-   Once running instruction C, we will jump back to the previous instruction, which is instruction B.

This program will increase x forever.
