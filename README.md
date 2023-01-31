# Conditionals

## Learning Goals

- Define conditionals.
- Explain statements.
- Use the `if` statement.
- Use the `if-else` statement.
- use the `if-elif-else` statement.

## Introduction

We make decisions based on conditions all the time. For example, if it’s raining
outside we would wear a raincoat. And if it’s sunny we would wear sunscreen.

Python allows us to make decisions based on conditionals using `if`, `if-else`,
and `if-elif-else` statements.

## What are Statements?

A statement is an instruction to the computer to do something. As we’ve learned
previously, “expressions” produce a value. Statements don’t produce a value.

Let’s look at an example:

```python
current_name = 2023
```

A variable declaration is a statement because it doesn’t produce a value.
Statements can have expression slots. In this example, `2023` is an expression.
Here’s the general structure for a variable declaration:

```python
variable_name = expression_slot
```

One way to check if a piece of code is an expression or a statement is to
`print` it. The `print` function can display expressions but statements will
raise an error.

```python
print(5 * 3) # 15
print(name = 'Al') # raises an error
```

Output:

```python
15
Traceback (most recent call last):
  File "main.py", line 2, in <module>
    print(name = 'Al') # raises an error
TypeError: 'name' is an invalid keyword argument for print()
```

## The `if` Statement

The `if` statement can be used to instruct the computer to execute a piece of
code only if a certain condition is met. Here’s the general structure:

```python
if (expression that evaluates to a boolean):
	# do something only if the expression produces True
```

And here’s an example:

```python
temperature = 80
if (temperature > 60):
  print("It's hot outside!")
```

The `print` statement is only executed when the condition `temperature > 60`
evaluates to `True`. Try changing the temperature to `60` or below and see what
happens.

### A Note on Whitespace

Python uses whitespaces as part of its syntax. Notice that the body of the `if`
statement is indented (4 spaces; you can use the “tab” key in the code editor).
If you try to run the code without proper indentation, it will raise an error.

You can read the
[official guidelines on indentation](https://peps.python.org/pep-0008/#indentation)
for more information.

## The `if-else` Statement

We can use this statement if we want to run a piece of code when the expression
of the `if` statement evaluates to `False`.

```python
num = 100

if (num > 100):
	print("The number is greater than 100")
else:
	print("The number is less than 100")
```

## The `if-elif-else` Statement

We can use this statement if we want to make a decision based on multiple
conditions:

```python
age = 20;

if (age < 16):
  print("You're too young to drive")
elif (age < 18):
  print("You're old enough to get a learner's permit")
else:
  print("You're old enough to get a full license")
```

## Conclusion

The conditional statements allow us to make programs that can react to a user’s
decision. Any complex program we develop will require us to decide things based
on certain conditions.
