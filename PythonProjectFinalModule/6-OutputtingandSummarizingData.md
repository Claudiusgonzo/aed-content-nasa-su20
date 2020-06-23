# Analyzing summary data

Let's start by printing the number of each type of rock we found. For example, to do this for Basalt rocks, paste in the following code:

```python
print("Number of Basalt: ", Basalt)
```

As you can see, we first output a string telling the user what they are going to be seeing and then we concatenate on the variable name which includes the number of how many Basalt rocks we found.

Try this for the other four types of rock variables we created.

Next, let's provide some more general data like the type of rock that was the most and least common. To do this, we will use the max() and min() functions that we learned about before.

Try to figure this out and if you get stuck, read below for the answer:

```python
print("The rock that was found the most was: ", max(basalt, ))
print("The rock that was found the least was: ", min(basalt, ))
```

Congratulations, you have now successfully programmed Artemis to give a summary about the different types of rock data that it found.