# Tensorboard-graph-problem-fixed-for-Google-Colab
# Purpose
I wanted to make a simple graph visualizing the architecture of my text classification algorithm and I came across Tensorboard graphs for Google Colab and thought I might give it a try. Sadly I kept getting an error that looks like this:<br />
<div align="left"><img src="tensorfail.JPG"</img></div>



So never fear!! I have found a solution to this issue so maybe it will help the few folks out there that use Google Colab. 

# Solution
You can go through the TensorBoard teams walkthrough to get started(https://github.com/tensorflow/tensorboard/blob/master/docs/graphs.ipynb) but where I found issue was when using the code:
``` Python
%tensorboard --logdir logs
```

So what I suggest is running everything on there that is needed i.e. tensorboard code, uploading the data, preprocessing steps to your problem, defining model(mine was already defined and I just uploaded it), and train the model. 

## Then follow these steps:

<h3> 1. Go to your files on Google Colab and download the logged file under train(seen below)</h3>
<div align="left"><img src="copyfile.JPG"</img></div><br />
<h3>2. Create a new folder called "log" and put the downloaded file in that folder. Place folder in the correct spot(you will see where in a second)</h3><br />
<h3>3. Open your command prompt and type "tensorboard --logdir=log", but make sure the folder is in the correct spot for the command prompt to find it. As you see the photo my folder was in the C drive, users, and then my name.</h3>
<div align="left"><img src="commandprompt.JPG"</img></div><br />
<h3>4. Then highlight over the local host webiste given and copy/paste that into a URL and you should get this:</h3>
<div align="left"><img src="tensorboard.JPG"</img></div><br />

# Results
Now I am a happy camper because I get to use my neural network graph! Hope this works!
<div align="left"><img src="tensorgraph.JPG"</img></div><br />
<h3>An edited version of the graph is show below:<h3/>
<div align="left"><img src="editedgraph.png"</img></div><br />
All I did was upload the original photo into Word and added color, etc, to make it come alive for my paper

# Implementation found here 
[![License: MIT](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/brianferrell787/Tensorboard-graph-problem-fixed-for-Google-Colab/blob/master/ColabTensorboardissuefixed.ipynb) 
 
