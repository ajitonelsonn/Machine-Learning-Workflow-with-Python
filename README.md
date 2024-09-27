# 1- Introduction
This is a **comprehensive ML techniques with python** , that I have spent for more than 6 months to complete it.

I think it is a great opportunity for who want to learn machine learning workflow with python completely.
I have covered most of the methods that are implemented for iris until **2018**, you can start to learn and review your knowledge about ML with a simple dataset and try to learn and memorize the workflow for your journey in Data science world.

I am open to getting your feedback for improving this
<a id="2"></a> <br>
# 2- Machine Learning Workflow
Field of 	study 	that 	gives	computers	the	ability 	to	learn 	without 	being
explicitly 	programmed.

Arthur	Samuel, 1959

If you have already read some [machine learning books](https://towardsdatascience.com/list-of-free-must-read-machine-learning-books-89576749d2ff). You have noticed that there are different ways to stream data into machine learning.

most of these books share the following steps (checklist):
*   Define the Problem(Look at the big picture)
*   Specify Inputs & Outputs
*   Data Collection
*   Exploratory data analysis
*   Data Preprocessing
*   Model Design, Training, and Offline Evaluation
*   Model Deployment, Online Evaluation, and Monitoring
*   Model Maintenance, Diagnosis, and Retraining

**You can see my workflow in the below image** :
 <img src="http://s9.picofile.com/file/8338227634/workflow.png" />

**you should	feel free	to	adapt 	this	checklist 	to	your needs**
## 2-1 Real world Application Vs Competitions
<img src="http://s9.picofile.com/file/8339956300/reallife.png" height="400" width="300" />
<a id="3"></a> <br>
## 3- Problem Definition
I think one of the important things when you start a new machine learning project is Defining your problem. that means you should understand business problem.( **Problem Formalization**)

Problem Definition has four steps that have illustrated in the picture below:
<img src="http://s8.picofile.com/file/8344103134/Problem_Definition2.png" width=400 height=400>
## 3-1 Problem Feature
The sinking of the Titanic is one of the most infamous shipwrecks in history. **On April 15, 1912**, during her maiden voyage, the Titanic sank after colliding with an iceberg, killing **1502 out of 2224** passengers and crew. That's why the name DieTanic. This is a very unforgetable disaster that no one in the world can forget.

It took about $7.5 million to build the Titanic and it sunk under the ocean due to collision. The Titanic Dataset is a very good dataset for begineers to start a journey in data science and participate in competitions in Kaggle.

ٌWe will use the classic titanic data set. This dataset contains information about **11 different variables**:
<img src="http://s9.picofile.com/file/8340453092/Titanic_feature.png" height="500" width="500">

1. Survival
1. Pclass
1. Name
1. Sex
1. Age
1. SibSp
1. Parch
1. Ticket
1. Fare
1. Cabin
1. Embarked

> <font color="red"><b>Note :</b></font>
You must answer the following question:
How does your company expact to use and benfit from your model.
### 3-2 Aim
It is your job to predict if a **passenger** survived the sinking of the Titanic or not.  For each PassengerId in the test set, you must predict a 0 or 1 value for the Survived variable.
<a id="6"></a> <br>
### 3-3 Variables

1. **Age** :
    1. Age is fractional if less than 1. If the age is estimated, is it in the form of xx.5

1. **Sibsp** :
    1. The dataset defines family relations in this way...

        a. Sibling = brother, sister, stepbrother, stepsister

        b. Spouse = husband, wife (mistresses and fiancés were ignored)

1. **Parch**:
    1. The dataset defines family relations in this way...

        a. Parent = mother, father

        b. Child = daughter, son, stepdaughter, stepson

        c. Some children travelled only with a nanny, therefore parch=0 for them.

1. **Pclass** :
    *  A proxy for socio-economic status (SES)
        * 1st = Upper
        * 2nd = Middle
        * 3rd = Lower
1. **Embarked** :
     * nominal datatype 
1. **Name**: 
    * nominal datatype . It could be used in feature engineering to derive the gender from title
1. **Sex**: 
   * nominal datatype 
1. **Ticket**:
    * that have no impact on the outcome variable. Thus, they will be excluded from analysis
1. **Cabin**: 
    * is a nominal datatype that can be used in feature engineering
1.  **Fare**:
    * Indicating the fare
1. **PassengerID**:
    * have no impact on the outcome variable. Thus, it will be excluded from analysis
1. **Survival**:
    * **[dependent variable](http://www.dailysmarty.com/posts/difference-between-independent-and-dependent-variables-in-machine-learning)** , 0 or 1
## 4- Inputs & Outputs
<a id="41"></a> <br>
### 4-1 Inputs
What's our input for this problem:
    1. train.csv
    1. test.csv
<a id="42"></a> <br>
### 4-2 Outputs
1. Your score is the percentage of passengers you correctly predict. This is known simply as "**accuracy**”.


The Outputs should have exactly **2 columns**:

    1. PassengerId (sorted in any order)
    1. Survived (contains your binary predictions: 1 for survived, 0 for deceased)
## 5- Loading Packages
In this kernel we are using the following packages:
 <img src="http://s8.picofile.com/file/8338227868/packages.png" width=400  height=400>
# 6- Exploratory Data Analysis(EDA)
 In this section, you'll learn how to use graphical and numerical techniques to begin uncovering the structure of your data. 
 
* Which variables suggest interesting relationships?
* Which observations are unusual?
* Analysis of the features!

By the end of the section, you'll be able to answer these questions and more, while generating graphics that are both **insightful** and **beautiful**.  then We will review analytical and statistical operations:

*   5-1 Data Collection
*   5-2 Visualization
*   5-3 Data Preprocessing
*   5-4 Data Cleaning
<img src="http://s9.picofile.com/file/8338476134/EDA.png">

 ><font color="red"><b>Note:</b></font>
 You can change the order of the above steps.
## 6-1 Data Collection
**Data collection** is the process of gathering and measuring data, information or any variables of interest in a standardized and established manner that enables the collector to answer or test hypothesis and evaluate outcomes of the particular collection.[techopedia]
<br>
I start Collection Data by the training and testing datasets into Pandas DataFrames
## 6-2 Visualization
**Data visualization**  is the presentation of data in a pictorial or graphical format. It enables decision makers to see analytics presented visually, so they can grasp difficult concepts or identify new patterns.

With interactive visualization, you can take the concept a step further by using technology to drill down into charts and graphs for more detail, interactively changing what data you see and how it’s processed.[SAS]

 In this section I show you  **11 plots** with **matplotlib** and **seaborn** that is listed in the blew picture:
 <img src="http://s8.picofile.com/file/8338475500/visualization.jpg" />
# Help

I hope you have enjoyed reading my python notebook.

If you have any problem to run notebook please open an issue here in github.

for most of the my notebook you need **dataset** as input.

To use the **correct data**, please **download** the dat set from  the **Kaggle** site and put it in your notebook folder.

**Mj Bhamnai**

mohamadjavad.bahmani@gmail.com

 **Have Fun!**
 
you can follow me on:
> ###### [ GitHub](https://github.com/ajitonelsonn)
> ###### [LinkedIn](https://www.linkedin.com/in/ajitonelson/)

 
 ## Please Fork the Repository to continue...
