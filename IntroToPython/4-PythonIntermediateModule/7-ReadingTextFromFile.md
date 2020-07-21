# Importing Data with Python

In many applications of Python, you will need to use data that comes from some other source. This could come in the form of reading an Excel file with data tracking the various parts of a rocket or a text file to read the rocks that a moon rover sees. In this unit we will learn how to read data from a text file using a pre-made Python function.

## Setting up Data

The first step to reading data from a file is to first get a file and save it in a location that we can tell Python to access later. First, find out where your Jupyter notebook file is saved. This may be in a Python folder or even your desktop. Next, you will need to save [this text.txt file](Media\text.txt). It is very important to save this file in the same location as your Jupyter Notebook file. This will make is very easy to tell Python where to find the data. Your folder should look similar to the one below.

:::image type="content" source="Media\SaveTextFile.png" alt-text="File Structure":::

## Getting Data in Jupyter Notebook

Now that we have our data saved, we must make a string in Python telling us what the file name is.

```python
strPath = "text.txt"
```

Next, we will use the open() function to get the file in Python. We will make a new variable called fileObject to hold the data.

```python
fileObject = open(strPath)
```

Finally, we will have Python read this `fileObject` variable to give us a list of strings that we can explore with Python functions by using the readlines() function. The readlines() function will take each line of the text file and make it an entry in a list. We will store this list in another variable so we can print it out later. It is also good practice to close out the fileObject when you are done with it. Do this by calling .close().

```python
textList = fileObject.readlines()
fileObject.close()
```

Finally, we can print the contents of the string we just read by iterating over the list.:

```python
for line in textList:
    print(line)
```

>First Astronaut on the moon  
>Neil Armstrong

The example above teaches us how to read the full data into Python. We can also read a text file and only go through certain parts of. This is called parsing in programming. To parse through the text we just imported, let's go line by line and print every line out. Since every line is an element in our list we can get the first line by looking at the first element in the list.

```python
firstLine = textList[0]
print(firstLine)
```

>First Astronaut on the moon

To read the second line from the text file just get the second item in the list.

```python
secondLine = textList[1]
print(secondLine)
```

>Neil Armstrong
