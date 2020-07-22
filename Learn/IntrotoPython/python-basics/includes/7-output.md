# Exercise - View Results of Variables and Expressions in Python Notebooks

Now that we have created some variables and have given them values, we can learn how to view the values beyond running a notebook cell. To do this, we will use a function called print(). Notebooks are useful because each cell will output the value of the final command without the need to do use the print() function. However, it might be useful to print values or messages in between larger code blocks for debugging, logging, or informational purposes. Without the print() function, the cell will only print the last value:

```python
2 + 2
5 + 3
```

>8

The print() function, like the functions we have called earlier when using strings, is code written by others that we can use. The print() function will make the computer write the values within the values you pass in as a parameter.

Try to print some values to the console by using the code below:

```python
print(6)
print("Hello World")
```

>6  
>Hello World

Along with only values, we can use the code below to print the value of a variable:

```python
numRocks = 15
print(numRocks)
```

>15

We can combine variables and strings by putting a comma in between them:

```python
numBasalt = 4
print("The number of Basalt rocks found:", numBasalt)
```

>The number of Basalt rocks found: 4

```python
date = "February 26"
numRocks = 15
print("On", date, "number of rocks found:", numRocks)
```

>On February 26 number of rocks found: 15

The print function is very helpful because the people using our programs won't always be able see our code or not know how to read our code. The print function allows us to only show them the values we want them to see.
