# Exercise - Create a Jupyter Notebook File in Visual Studio Code and Run a Simple Program

Now that we have installed everything that we need, we can create our own Jupyter Notebook file and begin coding.

## Creating a Jupyter Notebook File

To start, you should make a folder to easily organize all of the Jupyter files you will create. Pick a location on your computer that is easily accessible (documents or desktop are good choices) and create a folder named something like `Jupyter Files` or `Python`.

To create a Jupyter Notebook file that will run our Python code, first go to Visual Studio Code and locate the "file" tab at the top left of the screen. Click on this to view a drop down menu and click on "new file". You will then be taken to a blank file. Now we are going to save this as a Jupyter file: click file and then save or `ctrl-s`.

Name your file anything you want, choose the save location to be the folder you just created, and then change the file type to "Jupyter" from the drop down menu. Alternatively, you can add the file extension `.ipynb`, which will automatically change the file type to "Jupyter".

You will know that it worked if in the top left of the screen you see the name you gave to the file followed by ".ipynb" and if your file reloads inside of Visual Studio Code to have cells instead of one solid editor view.

:::image type="content" source="..\Media\MakeJupyter.png" alt-text="Set Python environment":::

## Configuring Python Environment

Once the file changes to Jupyter Notebook, on the bottom left of the window, you will need to choose which Python environment you are using. After you installed Python, Visual Studio Code might already recognize Python, but if it does not, simply click the box on the bottom left of the screen and select the version of Python that you installed.

:::image type="content" source="..\Media\JupyterEnvironment.png" alt-text="Set Python environment":::

Next, you will need to add Jupyter Notebooks to your path. To do this, type "2+2" into the first line of the editor and click the green play button. At the bottom right of the screen you will see a pop-up asking you to install Jupyter Notebooks, click install and the installation will begin. This may take up to 5 minutes, so you may have to wait a little.

:::image type="content" source="..\Media\InstallJupyter.png" alt-text="Set Python environment":::

Now, Jupyter Notebooks should be installed on your computer. Before continuing, make sure that the Jupyter Notebook Kernel is also running with the version of Python that you expect. You can see this in the top right of Visual Studio Code where it says "Jupyter Server: local" followed by the instance of Python.

## Information about Jupyter Notebooks

The [Visual Studio Code Jupyter Notebooks docs](https://code.visualstudio.com/docs/python/jupyter-support) have good documentation on how to this environment. Basically, in Jupyter notebooks there are cells where you write code. The plus button to the left of a cell will create a new cell below the current cell, when you click on it. The garbage can to the right of it will delete the selected cell and the arrow buttons will move the cell up or down in relation to the cells around it.

Additionally, the green play button in each cell will run that cell. After you run a cell, a number will appear surrounded by square brackets. This helps you keep track of what cells you just ran. This is important because, as you remember, you can re-run cells within a Jupyter Notebook which might change variables or program state.

Looking at the top of the file, you can choose to run all cells above or below the current cell with the play button. Finally, you can click the red pause button to force stop the program at any time.

## Writing and Running Simple Program

Now you will test your setup by writing a simple "Hello World" program. In the the first line of the editor type the following code and then click the green play button.

```python
"Hello World"
```

:::image type="content" source="..\Media\RunJupyter.png" alt-text="Run Jupyter":::

Below the cell that you have just ran, there should be an output saying Hello World.

Congratulations! You just programmed a computer to output text. Next step: ~~hacking the mainframe~~ ... or maybe we will start by learning more about Python fundamentals!
