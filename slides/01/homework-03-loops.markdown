---
layout: lab
title: javascript conditionals, loops
prefix: ../../
---
# Homework

1. grade
2. fizz buzz
3. changing your number guessing game!

## Instructions

### grade

__Objective__ - practice using  boolean operators (and or or), comparison operators (less than, greater than, etc.) and conditionals (if, else if, if else if)
Write a program that converts a numeric grade into a letter grade using the following scale:

{% highlight bash %}
A: 90 - 100
B: 80 - 89
C: 70 - 79
D: 60 - 69
F: anything less than 60
{% endhighlight %}

* create a new file called __fizzbuzz.html__ 
* setup an html file, and add script tags... start writing your JavaScript between the script tags
* the program should ask for a numeric grade: "What was your score?"
* use a series of conditionals (if, if and else, if and else if) to determine if the number falls within a certain range (see [Control Flow in Eloquent JavaScript](http://eloquentjavascript.net/02_program_structure.html#h_rDxYNPd65Z))
	* the condition will likely involve one of the boolean operators that we learned: <code>and (&&)</code> or <code>or (||)</code> ... as well as comparison operators like &lt;, &gt;, etc.(see [Maya's Notes](https://github.com/mayaman26/itp-camp/blob/gh-pages/slides/01/js-complexbooleans.markdown), and [in depth at MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Comparison_Operators))
	* JavaScript will coerce types when using these comparison operators (that is, if you test a string and a number, an operator like &gt; will convert both to numbers)
* output the appropriate letter grade for the number that the user enters (for example, if the user enters 82, then the program should output B to the console)
* example interaction is below (everything after the greater than sign (&gt; is user input using the prompt function):
{% highlight bash %}
# Run 1
(prompt) What was your score?
> 82
B
# Run 2
(prompt) What was your score?
> 50
F
# Run 3
(prompt) What was your score?
> 99
A
{% endhighlight %}

### fizzbuzz

__Objective__ - practice using a for loop 

Write a program that prints out the numbers 1 to 100

* ... but for multiples of 3 print Fizz instead of the number 
* ... for multiples of 5 print Buzz
* ... for numbers which are multiples of both 3 and 5 print FizzBuzz

* hints
	* use modulo to determine if one number is divisible by another
	* be careful of ordering
	* boolean operators may be helpful

Example Output

{% highlight bash %}
1
2
Fizz
4
Buzz
Fizz
7
8
Fizz
Buzz
11
Fizz
13
14
Fizz Buzz
16
.
.
.
97
98
Fizz
Buzz
{% endhighlight %}

### guess

__Objective__ - practice using a while loop 

Using your code for your number guessing game, change your program so that it continually asks for a number _until_ the user guesses correctly (use a while loop to do this)
