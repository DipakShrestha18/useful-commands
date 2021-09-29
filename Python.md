`https://practical.learnpython.dev/`

source env/bin/activate - Active virtual environment

Type `python` to go to repl from virtual environment >>> and `ctrl + d` or `exit()` to exit


VSCode useful command
```
Cmd + Shift + P
```

pypi.org - for python packages
peg8.org - gives coding convention of python

Use snake_case for variable names

In python everything is object like str, int, round, boolean

There are 3 helpful method that you will be using in repl all the time.
- help() - It lets you see documentation on repl
```
>>>help(str)
```

- type() - This tells us what the type of variable is 
```
>>> num = 42
>>> type(num)
<class 'int'>
```

- dir() - shows the directory of all methods that is available for this type (int, string)
```
>>>dir(str)
>>>dir(int)
```

- print()

f-strings

There are several types of string formatting in Python, but f-strings introduced in Python 3.7 are the most modern and efficient.

f-strings start with the letter f. Variables and expressions can be inserted into the string by enclosing them in curly brackets.

```
name = "Joe"
greeting = f"Hello, {name}"
print(greeting)
```

Tuples - is a immutable list
```
tuple()
```
