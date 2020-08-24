Dive Into Python Tutorial
=========================

### Pages with Further Reading links ###

- 52
- 92
- 105
- 118
- 126
- 168
- 184
- 210
- 285
- 309
- 333
- 377
- 437
- 484

Before I do anything else...

Is there a way send code from vim to a python shell?

How?

> As soon as you have a named argument, all arguments to the right of that need to be named arguments, too.

The sys.path is where python looks for libraries to import via module

    >>> sys.path
    [
    '', 
    '/Users/geoff/Documents', 
    '/Library/Frameworks/Python.framework/Versions/3.7/lib/python37.zip', 
    '/Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7', 
    '/Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/lib-dynload', 
    '/Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages'
    ]

colon + indentation = a function block

Everything in python is an object!!

> everything is an object in the sense that it can be assigned to a variable or passed as an argument to a function.

Colon `:` marks the beginning of a python code block

White space is important, and needs to be consistent. Indents don't need to be four spaces, but they to need to be *consistent*.

Python has exceptions, which are instances where you forsee possible exceptions in your code, or possible errors. You then figure out ways to deal with these exceptions, by first raising an error, then handling it in some way, with a `try...except` block for example.

```
  * - multiple
  ** - exponent
  % - modulo
  / - floating point division
  // - integer division, but not always as you expect
```

Python can do math, some results can be weird if you're not careful.
Python can do fractions.
Python can do trig.

Lists
-----

Slicing, creates a new list comprised of a subset of the old list.

```
a_list =/= a_list[:]

a_list[:] is a subset of the old list, containing every value from the old list

```

`pop()` function by default removes the last item in a list and returns the value that was removed.

A tuple is a list that cannot be changed, once it has been created... kind of like a constant, I guess.

Technically tuples are immutable. Actually, tuples have no 'methods' which allow you to perform any operation which changes the tuple.

You can observe the tuple, and slice it (because this created a new tuple).

You can also perform boolean operations on a tuple.

*A set is an **unordered** bag of **unique** values*
- a set won't 'remember' what order its componenets were added
- a set can only contain unique values (this is different from all other datatypes/frames so far, which take any number of values, and they can be the same, and they are ordered!)

There are two methods to remove values from a set.

`discard()` - removes a single value, and if the value doesn't exist it doesn't do anything
`remove()` - removes a single value, and if the value doesn't exist it returns an error, a `KeyError` to be specific.

pp 82: set operations - handy list of definitions

`Union`
`Intersection`
`Difference`
`Symmetric_difference`
`issubset`
`issuperset`

From what I can tell, any empty data 'container' passed to a boolean operation is false when empty, and true otherwise.

Dictionaries cannot contain duplicate keys, but multiple keys can have the same value.

---

Comprehensions
--------------

### Working with Files and Directories and stuff ###

Lots of interesting things you can do with filenames. How useful is it all? I suppose when you start doing real programming you find it more useful.

List comprehensions seem pretty important, but I'm too tired at this point for it to really sink in.

Seems pretty straightforward though too, and he's covering interesting syntax for for loops, if statements and other stuff.

I need to figure out how to export my command history to a text file, so that I can push that to my repo.


[master df6c818] Up to page 105
 1 file changed, 9 insertions(+), 1 deletion(-)
To https://github.com/DryLabRebel/DiveIntoPython.git
   b7dffda..df6c818  master -> master

---

A string is like a tuple of characters.

Very interesting, and different to R. in R, a string is stored into a variable, and the variable calls that string, and takes it as a single value.

in R:

```
x = "This is 1 String ¡ with some special characters"
x
# [1] "This is 1 String ¡ with some special characters"
length(x)
# [1] 1
x[1]
# [1] "This is 1 String ¡ with some special characters"
x[3]
# [1] NA
```

in python:

```
x = "This is 1 String ¡ with some special characters"
x
# 'This is 1 String ¡ with some special characters'
length(x)
# 47
x[1]
# 'h'
x[3]
# 's'
```

Compound field names is going a little over my head. It makes sense, but it's a lot to take in, and seems like the kind of thing I'll forget if I don't practise it a lot.

So the basic idea is strings are extemely versatile, and also they are objects.

You can format values (like say, from a variable) into a string.

In a way, you can do this in bash.

In bash, ['"' double quotes are like switches which turn quoting on and off](https://www.grymoire.com/Unix/Awk.html#uh-4), so you can expand variables inside of quotes, which techinally means turning the quote off, and on again on either side of the varible.

This can however, get extremely complicated, as you can do more than simply replace the field with a variable value, you can index values in a list or something else, and insert that into the field.

```
si_suffixes = humansize.SUFFIXES[1000]
'1000{0[0]} = 1{0[1]}'.format(si_suffixes)
```

It's important to understand that in the field `{0[1]}` the zero represents the first argument to the *function call*, which in this case is `format`. Since there's only one argument, it's simply calling that argument. the 1 in `{0[1]}` is calling the *second* element in the `si_suffixes` list (because the first element is indexed as `0` (zero)... Just in case you forgot.

Format Specifiers - a sophisticated mechanism for micromanaging your strings, definitely keep an eye out for this later.

```
s.lower().count('f') # This converts all the values in 's' into lowercase, then calls the count function to count the number of 'f's. Very clever.

```

Lots of interesting stuff about strings, and using bytes.

Byte arrays are cool. It would probably be useful to have a cheatsheet of ACII codes and hexadecimals for referencing.



So much to learn and read, how to build knowledge?

# ##########################
# ##########################
# Currently up to page 120 #
# ##########################
# ##########################

Functions
Modules
Classes
Subclasses
Class instances
Strings
Lists
Attributes
Methods
Exceptions

What are these things? Or, more specifically, what specifically are they in python (or R for that matter)?

Do they mean roughly what they mean in R?




