# Exercise - Import Python Libraries and Rocket Launch Data

With a goal, *Is a launch likely to be able to happen given specific weather conditions?*, and a data set containing weather data from successful and one pushed launch day, as well as the days leading up to and following each launch - you can start to actually code!

## Machine Learning in Code

While there are a number of tools and services used to solve machine learning problems, these space-themed learning paths will be using Visual Studio Code, Python, SciKit Learn, and Azure. Microsoft has a [video about downloading and configuring a similar environment](https://www.youtube.com/watch?v=5E3WMb8_T3s&list=PLlrxD0HtieHjDop2DtiCmwTTcrlwKAVHE&index=8) to the one we need. You can also see additional instructions in LP2M7.

When setting up your local programming environment, we recommend creating an Anaconda environment to ensure you have exactly what you need for that particular project. If you have another way or set of tools you prefer to use, the majority of these modules do not explicitly require Visual Studio Code or Azure.

## Local Environment Setup

Before continuing, be sure that you have:
- Visual Studio Code installed with the Python and Jupyter Notebook Extension (Link to LP1M1)
- An Anaconda environment with Pandas, NumPy, scilkit-learn, pydotplus, Azure Machine Learnign SDK
- A folder to store all of the code and data
- The data downloaded and saved to the folder
- A blank Jupyter notebook saved in the folder
- The folder open in Visual Studio Code
- The Visual Studio Code Python environment set to the Anaconda environment

### Local Setup 

To setup your local environment:
1. Install [Anaconda](https://www.anaconda.com/products/individual)
2. Open the Anaconda prompt
![Anaconda Prompt](Learn\launch-project\2-data-collection-and-manipulation\media\anaconda-prompt.jpg)
3. In the Anaconda Prompt, create a new Anaconda environment:  
```
create -n myenv python=3.7 pandas numpy jupyter seaborn scikit-learn pydotplus
```
4. In the Anaconda Prompt, activate the new environment:  
```
conda activate myenv
```
5. In the Anaconda Prompt, install AzureML-SDK:  
```
pip install --upgrade azureml-sdk
```
6. In the Anaconda Prompt, install an Excel reader:
```
pip install xlrd
```
7. With the folder open in Visual Studio Code, make sure your Python Intepreter and Jupyter Kernel are both set to your Anaconda Environment. Click on both the top right Jupyter Kernel Python version and the bottom left Python Interpreter and make sure you set them both to use the Anaconda Environment you created:  
![Visual Studio Code with Anaconda Environment](Learn\launch-project\2-data-collection-and-manipulation\media\ensure-python.jpg)

## Import Libraries

With your Visual Studio Code local environment setup, you can now import the libraries that will help us import and clean the weather data, and create and test the machine learning model..

Copy the following code into a cell and run it to import all of the needed libraries.

```Python
# Pandas library is used for handling tabular data
import pandas as pd
# Numpy is used for handling numerial series operations (addition, multiplification and ...)
import numpy as np
# Sklearn library contain all the machine learning packages we need to digest and extract patterns from the data
from sklearn import linear_model, model_selection, metrics
from sklearn.model_selection import train_test_split

# Machine learning libaries used to build a decision tree
from sklearn.tree import DecisionTreeClassifier
from sklearn import tree

# Sklearns preprocessing library is used for processing and cleaning the data 
from sklearn import preprocessing

# for vizualizing the tree
import pydotplus
from IPython.display import Image 
```

## Read Data into a Variable

Now that we have all of the libraries imported, we can use the pandas library to import our data. Use the command `pd.read_excel` to read the data and save it in a variable. Then, we will use the `.head()` function to print out the first 5 rows of the data. This will ensure that we have read everything correctly.

```Python
launch_data = pd.read_excel('RocketLaunchDataCompleted.xlsx')
launch_data.head()
```

## Begin Exploring Data

Finally, we can use the `.columns` function call to view all of the columns in our data. This will show us the different attributes the data has. You will see some common attributes like names of past rockets that have been scheduled to launch, the data they were scheduled, if they actually launched, and many more. Look at these columns and try to guess which ones will have the greatest impact of determining if a rocket will launch or not.

```Python
launch_data.columns
```
