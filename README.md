# Machine Learning Techniques on Breast Cancer Wisconsin Data Set

**Contributor**:
+ Raul Eulogio

I created this repo as a way to get better acquainted with **Python** as a language and as a tool for data analysis. 

I employed four **Machine Learning** techniques:
+ **Kth Nearest Neighbor**
+ **Decision Tree**
+ **Random Forest**
+ **Neural Networks**

If you would like to see a walk through of the analysis the **Jupyter Notebook** includes running code as well as explanations for algorithms and processes. 

For the script I employed a technique I learned from [Nathan Fritter](https://github.com/Njfritter) (thanks homie). It is outlined as such:

The **.py** script is broken into 5 sections (done by creating a function for each section) in the following order:
+ **Exploratory Analysis**
+ **Visual Exploratory Analysis**
+ **Kth Nearest Neighbors**
+ **Decision Tree**
+ **Random Forest**
+ **Neural Networks**

## Running .py Script

To run the script successfully, within the terminal you would employ this technique (Outlined starting at line 618):

I have 6 functions which are called up using these initials:
+ **Exploratory Analysis** - `EA`
+ **Visual Exploratory Analysis** - `VEA`
+ **Kth Nearest Neighbors** - `KNN`
+ **Decision Tree** - `DT`
+ **Random Forest** - `RF`
+ **Neural Networks** - `NN`

So for example you wanted to run **Exploratory Analysis** section you type this into the terminal:

	$ python breastCancerWisconsinDataSet_MachineLearning.py EA

You would do the same for all other functions with the respective initial!

**NOTE**: You can also run it by making script executable as such:

	$ chmod +x breastCancerWisconsinDataSet_MachineLearning.py


**Remember**: You must have a *shebang* for this to run i.e. this must be at the very beginning of your script:

	#!/usr/bin/env python3

then you would simply just run it (I'll use **Random Forest** as an example)

	$ ./breastCancerWisconsinDataSet_MachineLearning.py RF

## Conclusions
Once I employed all these methods I deduced that **Neural Networks** performed the best in terms of all diagnostics. But when choosing the best model since **Neural Networks** are *black box* models, we don't gain a lot of insight into our data. So in conclusion **Random Forest** was the best model in terms of performance and insight to our data. 

### Diagnostics for Data Set

| Model/Algorithm 	| Test Error Rate 	| False Negative for Test Set 	| Area under the Curve for ROC | 
|-----------------|-----------------|-------------------------------|----------------------------|
| Kth Nearest Neighbor 	| 3.509% |	2 |	0.9627 | 
| Decision Trees 	| 5.263% 	| 4 |	0.9482 | 
| Random Forest 	| 3.509% 	| 3 	| 0.9673 | 
| Neural Networks 	| 1.754% 	| 1 	| 0.981 | 

#### ROC Curves for Data Set
**NOTE**: Created on the **Jupyter Notebook** iteration. Not found in **Python** script. 
<img src="images/rocNotebook.png" style="width: 100px;"/>

#### ROC Curves zoomed in
<img src="images/rocClose.png" style="width: 100px;"/>

The ROC Curves are more telling of **Random Forest** being a better model for predicting. 

Any feedback is welcomed!

Things to do:
+ Change **Jupter Notebook** to reflect changes made to **Neural Networks** since I got better predictions 
+ Change **ROC Curves** on this **README** since **Neural Networks** performed better than last iteration
+ Change conclusions since reading documentation of real life application showed that both **Neural Networks** and **Random Forest** are useful. Its not just about picking one model. Found here: https://research.googleblog.com/2017/03/assisting-pathologists-in-detecting.html
+ Too tired to do right now 

Still a work in progress, but decided to leave both iterations to show different ways my work flow happens and emphasize that iterations make a project go from **okay** to **lit af** 