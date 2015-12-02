#Microsoft Azure Training

##John Pelak BlueMetal
* edx azure training
* sign up for certification on demand self paced
* do machine learning at stanford
  * https://www.coursera.org/learn/machine-learning
  * https://www.edx.org/course/building-cloud-apps-microsoft-azure-part-microsoft-dev202-1x-0

* mine the data network (would like to see twitter and Instagram mining)

* will be using vector calculus statistics and probability
* gradient descent
* minimize cost function from gradient point, minimum of the curve: convex functions
* used for regression models

* predict numeric value

* william sidley gossett Student’s T-Test: from small sample size to much larger population to infer effects are statistically significant
p value .05 or less, says change is just due to per chance

* principle component analysis, that computes a matrix 

* ‘Future’: Keeping Tab(let)s on Crome Data The Wall Street Journal

* Customer Patterns: Operator Insights: aggregated and correlated to provide big data warehouse harvested from millions of viewers, predictive models built to maximize advertising revenue opportunities

* mtv’s the matrix paradoy ft. will ferrell, justin time

* google algorithm unsupervised machine learning

* 15 degrees lower than normal, which will result in a larger energy consumption

* D3 and C3 are web based visualizations Webpl gpu acceleration
* calling into code and API
* Webpl: http://globe.cid.harvard.edu/

* open source version of matlab is octave

####3 Data Science and Machine Learning Essentials: Cynthia Rudin, Steve Elston Quantia Analytics
* use Kaggle.com to download data sets
* free data sets: UCSD or UC Berkley or Irvine
* A lot of preprocessing work
* Can’t trust your data (Personal Note: Why not machine learning for cleaning data sets)

* Having a string or number and vectorizing them (linear model of geographic locations)
* don’t just want a label in a row, vector to 1 or 0

* support vector machine, +/- supervised machine learning problem for classification

* cosign similarity

* recommender systems

* root means square data—how far off your actual items are from what you predict (similar to standard deviation

* Machine Learning (ML)
* when building a model, use a training set and a test set.  Results should be close to training set to build model and then use one that goes closest test set results

#####Chapter 3
* Classification: have to turn observations into numeric values—each observation is represented by a set of numbers (FEATURES) intensive analysis by a data scientist
  * input of model into rows with predictors, covaiants, explanatory variables, independent variables
  * training set (xiyi) for i=1..n can predict label y for a new x

* regression
  * fit a curve that predicts a numeric value instead of positives and negatives in classification
  * have to worry about overfitting
  * overfit = very high bias, low variance (curved line)
  * under fit = low bias, high variance (straight line)

* Occam’s Razor: Statistical Learning Theory
  * principle component analysis to limit the number
  * if it turns out two are correlated may take one variable out

* Clustering
  * unsupervised learning example
  * k-means cluster sets a few data points brings points together and rerun algorithm till you have cluster

#####Chapter 4 Regression
* sum of least squares
* slope is coefficient of the model
* optimal value: absolute value of actual income - residuals (what you predicted)
* also want squares of model to be small
* as well as continuous  form of integrals
* rules of thumb to statistical significance: watch videos on t tests

#####Ridge Regression
  * complex terms than linear
  * balance overfitting with reduction in error
  * hospital data had 700 linear regression, be careful of those types of things
  * regularization term = C term ~ penalizes the cost function for best fit, will penalize values of b

######would be interesting to see the number of tax return audits and your statical chances of being audited

#####Support Vector Machine (SVM) Regression

#####Cross-Validations
  * switch folding of validation
  * nested cross-validation

#####Learning with R
* how to subset a matrix, data frame and vector
* central limit theorem: distribution of average wingspan is still normal the bigger the sample size

* Counterintuitive, mathematically proven
  * a bimodal distribution will tend in the limit will become a normal curve

* why does central limit theorem move
  * creaturecast.org: bunnies, dragons and the ‘normal’ world

#####StatsCast: What is a t-test youtube video
* what is a t-test: checks the averages of means of two groups that are reliably different from each other
* means tells us if there is a difference, but t-test tells you the reason
* descriptive statistics: tells you what is going on in current test
* inferential statistics: tells you what you could expect in your new tests

* does the test actually work or was it just chance — this is the purpose of infrential/t-test
  * measures difference between the groups and within the groups

t = variance between groups/variance within groups

a big t value = different groups

a small t value = similar groups

#####P-Value
* how do we know if the t value ids big enough to show a difference ? = p value
* p-value tells you if difference between groups is real
* p = .05 there is no real difference / 5% difference

* larger sample size can have lower p value should have for 20/30 data points
degrees of freedom (df) = to the sample size minus one

#####3 types of test
1. independent test between 2 different groups (between samples/unpaired t test also names)
2. paired samples
3. one samples

*he uses Microsoft one drive*

#####Boston Code Camp R
* r will be available in sql server for tsql batches in 2016

* want to avoid FOR loops in R
  * much more efficient in multiplying big squares
  * r wants to do everything in memory
  * put a package up on cran

* r gives you markdown document .md
* easily rendered into html

* atomic classes or objects: character, numeric (real, Inf, NaN, NA), integer, complex, logical (True/False use this for vectors and subscripts)

  * basic object is a vector: same data class, list can contain objects of different classes
  * factors are categorical (could be useful for groups in custom attributes)
  * lm() is linear model, glm() is generalized linear model
  * will get 7 features boolean for each day of week for example

  * numeric 8 bits
  * 1 based in R

  * scoping rules: left arrow left arrow dash can send to shared

#####Azure ML
  * Windows server is under the Azure ML
  * sql server database

* can upload linux virtual machines into Azure
* experiments contain workflow, constructed of modules, transform data, compute modes, score models, evaluate models
  * create custom modules with sql, r and python

  * Microsoft virtual academy

* flow is rectangular table n columns m rows equal length columns results in a module
  * can manually upload or add from alternative servers

#####dplyr

#####python panda

* can develop and test your code in r studio and then deploy it into r studio
* r studio has good debugger that can set breakpoint
* debug your code in r studio and use your logs to check
* boilerplate code

* Boilerplate
* IDE
* Azuer = False

if Azure 

	#Load Azure ML table

else

	#Load local file

…

dataset -> execute scripte

set Azure = TRUE

converted to a data frame

dplyr runs on data frames

#####Execute R Script
myFrame <- maml.mapInputPort(1,2)

source(“src/myScript.R”)

maml.mapOutputPort(“myFrame”)

print(“Hello World”)

#####dplyr package

library(dplyr)

* bayesian, you have a population and you try to predict what the population would choose to guess the probability of what bin it came from

