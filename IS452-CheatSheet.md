# Cheat Sheet for IS452

This is the first time through for this document, so expect it to change a bit as we go.

# Data Types

## Numbers

You type in numbers without anything special.  A number just hanging out on its own will be considered as a numerical data type.

### Integers or `int`

There are whole numbers that may be negative.  Examples:  `-5`, `0`' `1000000`

All the normal math operators work on these.

### Floating point numbers or `float`

These are numbers with a decimal value.  This value may be `.0` because you have a whole number, but it will still be a float.  Examples:  `-194.02380`, `0.38940`, and `9.0`

## Strings

These are collections of charecter content.  I'm not using letters here because you can mave much more than just letters.  White space, punctuation, numbers, or anything else that could be considered part of text.  Think of these as "things that can be typed in on a kepboard".  You may have to search around to find them, but they could be typed in or copy/pasted.

You use quotes to state that content is a string.  You can use either single (`'`) or double (`"`) quotes for this.  It doesn't matter which one, so long as they match on either side.

Example:  `print("Hello!")` and `print('Hello!')` will produce the same output:  `Hello!`

You may also see triple quote (`"""`) strings, which are multi-line strings.  These allow you to have hard retuns (new lines) in your text.  You can use either `'''` or `"""`, but they have to match on either side.  You can use `/n` in any string to indicate a newline character, but triple quote strings allow you type them in or copy/paste text with the rendered newlines inside your script. 

Example:

``` python
text = """I am
on many
lines of text
"""
print(text)
```
Output:
``` text
I am
on many
lines of text
```

# For loops

## Do something an arbitrary number of times.

Relevant week:  2

You will use a for loop with range for this.

``` python
for i in range(number_of times):
  do your stuff here
```

Example that will print `"Hello!"` 5 times.

``` python
for i in range(5):
  print("Hello!") 
```

Output:

``` text
Hello!
Hello!
Hello!
Hello!
Hello!
```
You will change the number in `range()` to be however many times you want it to repeat.


## Unpack something and loop over those elements, however many there are.

General syntax:

``` python
for iterable_variable in sequence:
    do stuff
```

Example that will print out the individual characters within `"Hello!"`:

``` python
for character in "Hello!": 
    print(character)
```

Output:

``` text
H
e
l
l
o
!
```


Example that will print out a message for each character inside of `"Hello!"`

``` python
for character in "Hello!":
    print("I see a character!")
```

Output:

``` text
I see a character!
I see a character!
I see a character!
I see a character!
I see a character!
I see a character!
```

Important points:

* You don't always have to use the content of the `iterable_variable`, but it's there if you want.  
* You can name your iterable variable name any valid variable name, but you should try to use a new variable name. Do not repeat a variable name already in your program!
* the iterable variable will be created in the first loop through.  It will not exist before the for loop runs, but the variable will continue to exist with the final value after the for loop completes.
* Python knows how to unpack different kinds of things, so the data type of the iterable variable will be whatever the data type of that element is.
    * strings will unpack into the individual characters inside
    * numbers won't work. You need to use `range(n)` to generate a series of numbers
    * lists will unpack to the individual elements inside, which means you may have different data types for the iterable variable, if you have a list with multiple data types within it.

# Strings

## Slicing

Index positions will always start at 0.  When you want to slice a string, you'll be yanking out chunks of the text. Empty strings are represented by `""` with a length of 0, but will not have any index positions.

You can: 

* get a single character out:
  * `string[stop]`
* get a subset of adjacent characters:
  `string[start:stop]`
* get a subset of characters, skipping some (the step):
  * `string[start:stop:step]`

* Start: always inclusive
* Stop:  always exclusive
* Step:  count how many steps you want to go each time

## Looping

Strings will unpack character by character.  Each of these characters will be another string.

## Essential methods

String methods will always return back a new string for you.

* `string.split()` when left empty will get rid of all white space inside of the string and give you back a list of non-space characters
* `string.strip()` removes all the white space on the left and right sides.  Related are `rstrip()` and `lstrip()`.
* `string.lower()` lower case the string
* `string.join(sequence)` will join the elements of a sequence into a new string
* `string.replace(current_character, new_character)` will replace the current character with the new character.

# Lists

## Slicing

## Looping

## Essential methods
