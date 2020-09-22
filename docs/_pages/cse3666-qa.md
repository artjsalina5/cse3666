---
title: FAQs
layout: default
description: Some commonly asked questions from students in CSE 3666, Introduction to Computer Architecture.
---

# Frequently Asked Questions

## Why do I have to learn assembly language?

Well, processors only understand instructions. If you want to understand how
they work, you would need to learn and program with instructions. So we learn
assembly language in this course.

Here is Youtube video ["Why should I learn assembly language in
2020?"](https://www.youtube.com/watch?v=iYRl50gtprA).

## Why do computers use 2's complement numbers?

There are many explanations on the Internet. One of the reasons is we can use
the same method to do additon of unsigned and signed numbers. We just need to
build one adder in hardware to perform add/sub for unsigned binary nnumbers and
for 2's complement numbers.  

## How does the processor do additions on hexadecimal or decimal number?

The processors only deal with bits. They add bits. No matter what format we use
in the source code to specify numbers, they all are represented by bits in
computers. For example, you can write the following in your programs.

```
int x = 0xA0; 
int y = 160; 
```

Both ```x``` and ```y``` have the same value, represented by the same bits.

## Can you give me an example of MIPS code?  

There are many examples in textbook and slides. Here is a sample example. 

The problem is `Set register $s0 to 0.`. 

You could give an answer like 

```
	sub 	$s0, $s0, $s0
```

or 


```
	add 	$s0, $0, $0
```

You do not need to write an assembly program that can be assembled.

## How do I find out what an instruction does?

Read the reference manual! The information in slides is minimum to get you
started. Textbook has more details. Many MIPS pages may provide even more
details. An example is
[here](http://www.mrc.uidaho.edu/mrc/people/jff/digital/MIPSir.html), which
lists a subset of MIPS instructions, but with encoding.

You could go to [the MIPS32 manuals on the official site](https://www.mips.com/products/architectures/mips32-2/).
