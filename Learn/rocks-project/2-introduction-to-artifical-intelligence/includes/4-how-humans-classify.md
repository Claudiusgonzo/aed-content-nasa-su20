# Classify Space Rocks Like a Human

Before we build an AI system to detect the rock types, lets see how we 'humans' classify things.

This is the likely process that our brain goes through to do this:

### Step 0

We have to collect as many rock images as possible. This will let us see lots of different variations of the items we are trying to classify. Fortunately, this project, there are lots of space rock pictures openly available online that you can use.

### Step 1

Our brain first tries to extract patterns from each image, patterns such as:

Color combinations  
Sharp edges  
Circular patterns  
Texture of the rock  
Size of the rock  

Our brains subconsciously do all of these without us noticing. We call these 'Features' in AI.

Below are some features that we can extract from a motorcycle. You can see there are wheels, handle-bars, throttle, ect.

<img src="../Media/features.png" width="350" align="center">  

### Step 2

Next, we try to find the relationships between the features and rock types.

In this step our brain tries to figure out what are the characteristics/features of each rock type.

As a result of this, we will come up with some rules, for example : "Lighter rocks are usually Crustals". "Basalt rocks have more dense textures", ...
We show these associations with links such as shown below:

<img src="../Media/links.png" width="350" align="center">

### Step 3

Lastly we try to use these relationships to figure out what to classify a new item as.

Given a new rock image, our brain extracts all of its characteristics we discussed above, and then uses the associations we made in the second step to decides what type of rock it is.

<img src="../Media/dl.png" width="550" align="center">