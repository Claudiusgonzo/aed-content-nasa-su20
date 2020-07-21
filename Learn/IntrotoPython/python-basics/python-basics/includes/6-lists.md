# Lists

Lists are ways that you can store a lot of data in Python (similar to variables). They are a collection of values stored in the form of a list. Lists are very useful in Python because a lot of times you will need more than one piece of data. In data science, lists play a huge role because the goal of data science is to take large amounts of related data and analyze it. That's why the popular data science Python packages like Pandas and NumPy have additional data structures like dataframes and arrays, which are essentially lists with additional features.

## How to make a list

Defining lists in Python is very similar to creating variables. You must start by making a name for your list and then set it equal to a value. However, lists can hold multiple values. For example:

```python
# Create a list of common moon rocks
rockTypes = ["basalt", "highland", "breccia"]
rockTypes
```

>['basalt', 'highland', 'breccia']

As you can see, you must include square brackets and then include the values you want separated by commas.

Lists can have values that come in all forms (int, float, string) and can even mix and match different types. For example:

```python
# A list with rock names and the number of that rock found
rockTypeAndCount = ["basalt", 1, "highland", 2.5, "breccia", 5]
rockTypeAndCount
```

>['basalt', 1, 'highland', 2.5, 'breccia', 5]

## List Functions

There are many pre-made functions, included in Python which we can use to modify a list.

For example, we can add items to a list by calling the .append() function followed by the data that we want to add in parenthesis. This will add an item to the end of a list. Let's add a rock type to our original list.

```python
rockTypes.append("soil")
rockTypes
```

>['basalt', 'highland', 'breccia', 'soil']

We can also delete items from the end of a list by calling the .pop() function. We will now delete soil from the rock types list.

```python
rockTypes.pop()
rockTypes
```

>['basalt', 'highland', 'breccia']

Finally, we can look at and change the value from anywhere within the list. To see what value is at a certain point in the list, use square brackets after the list name to look at that specific value. Everything in Python is zero-indexed, meaning that counting begins at 0, not 1. So if we were to look at the value in the first position in a list, we would use:  `listName[0]`.  
In our rock type example, use the following code to look at the value in the second position in the list:

```python
rockTypes[1]
```

>'highland'

We can also change a specific value in the list at a specific point by coding:
listName[position in list to change value] = newValue.  
In our rock type example, if we wanted to change the value in the third position of the list to be "soil", we could do so by:

```python
rockTypes[2] = "soil"
rockTypes
```

>['basalt', 'highland', 'soil']

This will change the current value at this position in the list, so the previous value will be gone.
