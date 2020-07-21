Dive Into Python Tutorial
=========================

### Pages with Further Reading links ###

- 52
- 92
- 105
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

# #########################
# #########################
# Currently up to page 94 #
# #########################
# #########################

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




