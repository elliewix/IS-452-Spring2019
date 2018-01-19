# Cheat Sheet for IS452

This is the first time through for this document, so expect it to change a bit as we go.

# Data Types

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

## Looping

## Essential methods

# Lists

## Slicing

## Looping

## Essential methods
