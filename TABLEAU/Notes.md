#Data Visualization and Communication with Tableau
1. Define Context: ask questions, make hypothesis
2. Data Analysis
3. Write your Data Story
4. Tell your Data Story: Data communication, persuasion

* Craft the right questions
* Design and implement structured analysis plans
* Create important graphs in Tableau
* Transform data in Tableau and publish dashboards
* Tell data stories
* Design effective slide presentations
* Deliver compelling business presentations

#Week 1
####Tips for becoming a Data Analyst
1. Ask questions, nourish curiosity, and embrace the unknown
2. Start thinking about everything you see as a Dependent or Independent Variable
3. Start exploring the advantages of continuous vs. discrete variables
4. Listen and contribute (Data analysis projects are almost always collaborations)
5.  Train your skepticism muscles
6. Seek details
7. Cherish precision
8. Best practices do not equal most common practices
9. Expectations matter
10. Put yourself in other people’s shoes

####Asking the Right Questions
* When I recruit for BI/BA roles, it is important that the students have the following coursework/knowledge…
  1. Communication Skills
  2. SQL and Query Skills
  3. Basic Analytics
* Why do big data projects fail
  1. 75% organizations 25% technical
* Talk to and understand your stakeholders

#####The Framework
* Trying to find the right question to ask
* Asking more questions reduces the need to have all the answers
  -Donald Peterson, former CEO of Ford

#####Rock Projects
* **Define very clearly what value the data is supposed to create**

#####S.M.A.R.T. Objectives
* Need to know what business problem you/they are trying to solve
* Have a meeting with those who are funding the projects
  * What problem is this business having that you hope to solve by developing this project?
  * Can you tell me more about how this problem is affecting the business?
  * What is your ideal outcome of this project?
* SMART Statement reflect goal of analysis project - George Duran
  * Specific
  * Measurable
  * Attainable
  * Relevant
  * Time-bound
* How should my business metric change if my recommendations are put into action, and by how much?
* Specific and Measurable
  * Metric is the dependent variable
  * What independent variables would impact the dependent variable
* How far along is your company in embracing big data culture
* Show your SMART goals to stakeholders
* Elicitation Session: The process of drawing out or bringing forth, gathering information directly from people
* Goals
  1. Identify you key stakeholders
  2. Identify independent variables to test
  3. Determine whether stakeholders agree about problem to be solved
* What has been tried before and how did it turn out?
* application of issues, data governance
* analytics continuum
  1. descriptive analytics: hindsight ~ what happened, what’s happening
  2. diagnostic analytics: why things are happening ~ root cause analysis
  3. predictive analytics: trajectory ~ what is going to happen, likely scenarios
  4. prescriptive analytics: recommendations 
* 2 analytics team: trusted original and new scientific method using analytics

##### Using Structured Pyramid Analysis Plan (SPAPs) to Structure Your Thinking
* SMART goal on top with dependent variable
* independent variables middle
  * write as specific field calculation
* Specific analyses to run & graphs to make
* my mapping software: http://mindmapfree.com
* organize variables in a logical way
* layer two is categories of issues
* layer 2 is categories of behaviors
* layer 3 is marketing strategies of success
* layer 4 how to breakdown / aggregate
* layer 5 exactly what variable from what data source
  * color for know, may know, and no idea where source is

#Week 2
#####Use Data Visualization to Drive Your Analysis
* Science is knowledge which we understand so well that we can teach a computer” -Don Knuth
* Art in general consists of the truths of science, arranged in the most convenient order for practice, instead of the order which is most convenient for thought. -John Stuart Mill

#####Why Tableau?
* Ryan Mason Square: Analytics Tools and Reporting
  * Databases, MySQL, access used Hive and Vertica, wrapper for writing queries in ruby and python
  * Once we have data to work with use Tableau and Excel
  * Turn table of data into picture of what’s going on and allows interactivity
  * Manually writing sql queries is tedious
  * First load large data set into tableau play around with and then write queries on your own or in tableau
* Tableau server can be saved across company
* Prevailing wage
* possible for what types of salaries 
* Offered yearly wage, prevailing yearly wage, decision date, company, city, nationality, visa type, job title sub category
* number of experience required, education level req, date application received 

#####Tableau Graph
* Cards
* Shelves
* dependent variable = paid wage per year
* independent variable = job title subgroup
* Pills  
  * green are measures
    * have to tell green how we want to measure field
  * blue are measures
* Quicksort next to y axis name will sort high, low, original
* Swap will switch from vertical to horizontal chart
* To change title right click and update title, caption, summary
*can use marks card to put pills in to get details/change format of graph without having to change graph
* Std. dev use population if your population represent general population as well yes, do you care, no
* Use regular std. dev (sample) when you do not care whether your population represents the general population, but you do care.  Care that it were to apply to us
* even one outlier can mess up your average
* type of visa you make does not affect the salary you make
  * how to find outliers 
    1. Find Interquartiel, Q1, and Q2 (25 and 75 percentiles), interquartile range calculator
    2. 150% of IQR
    3. find low value = Q1 - 150IQR and high value = Q3 + 150% IGR
    4. Look for numbers that are below or above and you have the outliers

#####Understanding the Marks Card
* formatting and tooltip
* area will allow you to define the variable to use
* Shift and drag to marks card 

#####Removing Outliers Using Scatterplot and Filtering Groups
* Filter dynamically by right clicking on filter and check show quick filter
* Tableau can only use data points in the workspace
* create > group > manually create groups
  * include other so that you can count the rest as others
  * can slide subgroups up and down into order you like
  * can show quick filter on side to include exclude various fields
  * next presentation will show how to perform better ordering

#####When to use line graphs
* displaying how two continuous variables related to each other
* Continuous variables (measures)
  * Advantages: Best format for computing best fit lines, years are connected on line graphs
  * Disadvantages: Can’t see all details in a single graph
* Discrete Variables (Dimensions)
  * Advantages: easy analysis and labeling of date parts
  * Disadvantages: years are NOT connected on line graphs, some unintuitive effects when computing best fit lines
* Have data related salaries been changing over time?
* Circles views may give good view as scatter plot

#####Using Statistics
* Right click to show trend lines, edit trend
  * can edit line aggregated across all subgroups
  * can edit coorelation
* P value is how likely it is to happen, the smaller it is, the more reliable.
  * Trust trend lines .05, false positive result 5% or less
* treating dates as discrete variables (dimensions) can make statistical visualization as box and whisker plot
  * 4 quartile groups, interquartile range is 1st and 3rd quartile
* To make box plot need lots of data points, disaggregate

#Quiz 3
##### Customizing and Sharing New Data in Tableau
* Marketing and Innovation

##### Tableau Calculation Types
* Number, string, Date, Type Conversion, logical, aggregate, User
* “If i were doing this calculation in excel would I have a new number on every row in a new column (Row calculation, numbers useful at any level of detail), or would I have a single number at the bottom of my original columns (aggregation calculation)?”
* Table calculation done only at visualization level (only doing math in head)

#####How to Write Calculations
* Can replace data sources if you want, so that if you source data get’s updated you can switch over to the new one
* If you see a dimension after switching data source with a paperclip it means that it is connecting to the old data source
* right click on measures to get calculation pane
  * or go to analysis > create calculated field
* // to comment in calculated column
  * useful for nested calculations
* = sign in measure beans calculated parameter

#####Calculations that Make Filtering More Efficient
* make a logical calculation for if the state was in the group or not
* IF THEN ELSE END
  * If statement will result in creating a dimension
* if need a single quote need to double it ‘ = ‘’
* could also do CASE WHEN THEN ELSE END
* per year set default aggregation to sum

#####Identifying Companies that Pay Less than the Prevailing Wage
* Within data related jobs are their any subtypes that pay better and specific companies?
* Write out all operators in caps first

#####Blending Price Parity Data with Our Salary Data
* regional price parity of each state: sets national average cost of goods and services at 100
  * 124 would be 24% more than the national average
* data blending will take 2 source of data together when there are 2 different levels of aggregation
  * need one field that as the same data (ex: state)
* used to have to aggregate the data together 
  * Create a temporary table to store
  * small data set primary and the aggregated by your secondary
  * cant get more detailed than small table
  * Anything that’s not in the smaller table won’t be included
  * Anything that’s in the smaller but not in the larger will be included as NULL
  * The variables will be unchangeable measures (state)
  * This will be done separately each time you make a chart

#####Adjusting Data Related Salaries For Cost of Living
* Data > New Data Source
* Data > Edit Relationship
* First data set loaded tends to be primary
  * what you enter in edit relationship will not be critical
  * Primary data source the smallest, and Secondary Data source the largest
  * if no link, something didn’t work in this case it is because we set it to automatic switch to custom
* may have to go to analysis > marks > and turn off

#####Calculating which States have the Adjusted Salaries within Job Subcategories
* Why does blended row data provide no information?
  * requires a state level aggregation and there is no data for the calculation to work with
* no way to sort what is based on the visualization
  * tell it what to do with the work space through ranking related to job title subgroup
* command move aggregated measure to marks detail box > Add table calculation > Calculate the difference along is most important
  * bold will hardcode at very second (not a good thing)—never use
  * better to use variable advanced option
    * partition is grouping calculation
    * addressing is what we would apply it to
       *ex: partition: job title subgroup, address: work state
* to move new calculation it needs to be changed from a measure to a dimension > set to discrete
  * allows you to add in between partition and address columns
  * will no order according to adjusted paid wage
* Clean up
  * to clean up you can see rank below top of chart, can remove if you want > uncheck show header
  * can remove lines by right clicking > format > boarder option on left > minimize column dividers by reducing level

#####Using Parameters to Define Top States
* parameters: placeholders for string, number date, etc.
  * important because they are interactive, users can change them
  * different from filters is that they are global across worksheets
  * can be used in calculations
* use parameter 
* right click on measures pane > create parameter
* in calculated field, parameters are always in purple, measures in orange, blue for calculation
* logical calculation: TRUE or FALSE
* right click on param to show param control
* need to add logical calculation to marks > edit table calculation > compute using advanced 
  * then move updated field from marks to filters
* update calculation for in top x greater than or equal to
  * repeat process of table calculation in marks and then filters
  * now shows top 5 states in each job title sub group
* useful when you want to change visualizations across multiple worksheets (could be useful when looking at clients)

#####Calculating which Companies have the Top Adjusted Salaries within Job Subcategories
* dashboard using in one context: people coming to you with very specific request and information
* how to help you contribute to making business decisions
* dashboards have limited rows, can look at multiple graphs in one place
* can use results of one graph to filter on another graph
* useful when working on a data analytics team
  * can update a bit of what we have been doing
* steps again to get ranking
  * take calculated field > cmd + move row measure to detail mark > right click and add table calculation > Calculation Type: Rank > Running Along: advanced >  set partitioning and addressing > switch measure to dimension by right clicking > discrete > move in between fields in columns
* make parameter calculation and use in measure to create logical statement
  * move to detail marks
* edit in calculation advanced 
* drag calculation into filters

#####Designing a Dashboard to Determine Where You should Apply for Data-related Jobs
* dashboard > actions > add actions > filter/high/url
* Source sheet > select 
* Target Sheet > exclude all values
* format your filters: could do single value drop down, etc
* can change formatting on all titles, headers, axis
* how many entries are going into each one of the bars
  * would have to go back to sheet and add this (should be best practice)
* although dashboards are interactive, they are not great at giving a take home message
* no good way to control where eyes go in logical sequence
  * next piece gives better narrative

#####Visual Story Points in Tableau
* can have entire dashboard or worksheet
* want story ordered in a logical sequence to support arriving at the same conclusion
* good for when you publish on web
* can choose story size
* whatever filters in story points will not affect what happens in other story points if playing around with dashboard
  * useful for presentations
  * can click on things
  * at end you can zoom back out to data in dashboard
* story points can also just be useful for presentations or providing data to your boss
* can change story title, font color, etc.
* can add description to each story point (enters a text box)
* can present and interact with still seeing the data
* good way for figuring out what order would be useful for communicating your decision
* can make data story and publish online
* storyboards tend to have a lot of text
* The History of the Dow 30 tableau public
* pretty hard to get full take home message
* next week will help create a clear take home message

##Week 4

#####Using Visualization Science to Influence Business Decisions
* “If computer programming is to become an important part of computer research and development, a transition of programming from an art to a disciplined science must be effected.”
* Birth of Visualization Science
* Tableau has automated best practices
* Where people look is tightly aligned with what people decide
  * Will affect practical and abstract judgements
  * Want to affect, influence where to look
  * Physically guide their eyes
* Default formatting or Visually busy slides
  * Leaving decisions to chance
* Visual contracts best way to influence decisions

#####The Storyboarding Hourglass
* Structure of a Business Presentation
* Hour glass analogy
  * Heavy big picture
    1. Why? So what? the business problem you will solve less than a minute to frame emotional business problem—motivate audience emotions
    2. SMART: Specific, Measurable, Attainable, Relevant, and Time Bound—state specific recommendations within first minutes
    3. What I am going to show—agenda slide could go here
  * Skinny on the details
    1. Supporting evidence
  * Heavy on big picture
    1. Link evidence to smart rec.
    2. What you could gain
    3. Why? So what use story elements some that pair up with story elements in the beginning—strong positive emotion

  * Surround data you show with motivating details

* Be prepared to address pitfalls in appendix out of the main presentation or in Q & A
* Provided Technical Details White Paper
* Hand out after presentation is over
  * Before will reduce ability to maintain solutions

#####Making Your Data Story Come Alive
* Want to be able to solve business problem, affecting a company and as a consequence impacting their lives
  * Visual, sound, physical feeling, create an experience
  * Characters, location/setting, conflict, resolution
  * Make it feel like a story
  * Picture person or place in their mind
* Other devices could use imagery, this picture illustrates something we all know
*Jana’s Tips and Tricks
  1. Try starting in the middle of a story
  2. Use details
  3. Stick to positive emotions, negative tend to linger
  4. Use large, high-quality pictures (looking at someone’s face or point of view images)
  5. Think about what got you excited, worried, motivated to determine what emotional context to use in the presentation

#####Storyboarding your presentation
* Reasons for storyboard
  1. Clarifies your logic
  2. Highlights gaps in your logic
  3. Facilitates communication
  4. Streamlines slide-making
  5. Companies are starting to ask for storyboards instead of traditional dashboards
* Steps similar to smart goal pyramid
* brainstorm and write down each insight’s index card, should be a story point, should be summarized into one sentence, widdle down critical story points
  * 3 story points and 3 story sub points
* What they should do, not what you did
* When your recommendation is not controversial
  * First story point = most compelling story point
* When your recommendation is controversial
  * First story point = Least controversial story point
* Show relevant data, don’t show them how you got there
* draw a quick visualization example that your audience would like / details
  * Details can be in a hand out
* stress test your story

#####The Best Stress-Testers are Teams
* Lindsay Pettingill Data Scientist, AirBnb 
* Elena Grewal Data Scientist Manager, Airbnb
* Culture of bringing forward any errors
* Take a class on Logic and Reasoning, construct bullet proof arguements

###Common Errors to Avoid

#####Overgeneralization and Sample Bias
* For data related jobs, bias because only showing what is being offered to non us citezens
* Many more visas for men than women
* Large sample sizes can’t always be best when considering mobile big data
  * Data shadows lower socio economic data
* Smartphones, Big Data Help Fix Boston’s Potholes 
* How to catch mistakes
  * Not analytic mistakes
  * Data does not behave the way you assumed it to behave
  * Realize it is a subset of listings
  * Single minded paranoid 
  * Something is not quite right
  * Get familiar with data you are looking at
* Take rows out of your data, sometimes the missing data you remove could be systematically bias
* Tips and Tricks
  1. Ask questions about collection methods, look for ways to test data
  2. Always check number of data points
  3. Test subsets of data for consistency, see if consistent with whole or if subset should track down and analyze
  4. Look for common characteristics of outliers and missing data

#####Misinterpretations Due to Lack of Controls (Conclusions without controls)
* Need to look at sales of competitor (p-value? rose more to competitors)
* All about impact, can shape direction of company with data that you bring to the table


#####Correlation Does Not Equal Causation
* tylervigen.com
* Correlation: noun the degree to which two measures vary together
* Causation: noun the act of one thing being the result, or effect, of another thing
* Coincidence: noun a striking occurrence of two or more events at one time apparently by mere chance
* Spurious Relationship: noun correlations due to chance or unmeasured variables, but not direct causal relationships
  * both related to the unmeasured variable of summertime
* Data analysis > Inspires > Your  recommended Business Process change > Causes > Improved Business Metrics
 * Graphs should should Causation, not just correlation
* How do you support a causal relationship? Next video will help make decisions that are less risky for correlation

#####How Correlations Impact Business Decisions
* Benefits if relationship is causal > Cost of a poor decision
  * Make a business recommendations assuming the correlation is causal
* Benefits if relationship is causal < Cost of a poor decision
  * Get more information
* Small scale pilot phases to see the change early 
  * Want stepwise strategy
* Use scientific method and see whether cause and effect challenge to keep things constant, but this is the point of A/B Test
* A correlates with E, start to look for if there are other variables and whether they are a better measure of the correlation, multiple data sets
* Likelihood that you will get into trouble inferring causation from correlation y & complexity of data set x
  * doesn’t matter when you are trying to measure a phenomenon or predict
* http://dx.doi.org/10.1038/nature07634
* design to implement tests, need  to keep tabs on whether the correlation is stable

#####Choosing Visualizations for Story Points
* Don’t use 3-D charts, use flat file.
  * Use beveling or shadow instead of 3-D
* Tips Use:
  * Bar charts for comparing categories
  * Line charts for changes over time or an ordered category
  * Pie charts for 4 or fewer categories that add up to 100
* Don’t use scatter plots unless technical or 3 d plots ever

#####The Neuroscience of Visual Perception Can Make or Break Your Visualization
* Visual Perception: What people are aware of what they are seeing
* http://extremepresentation.typepad.com/blog/2006/09/choosing_a_good.html

#####Misinterpretations Caused by Color bars
* Do not use color to: convey detailed quantitative differences in the values of continuous variables
* Do use color to: the illustrate general patters

#####Visual Contrast Directs Where Your Audience Looks
* google docs survey
* Salient: adjective standing out conspicuously; very noticeable
* colors could show this is important, this is not important for grey and orange and white

######Formatting Slides to Communicate Data Stories
* Maximize data ink ratio: ink that represents the actual data, leave everything out
* Likely giving up some of your power to influence decision-making
  * Don’t be afraid of white or empty space
* Understanding at a glance
* Times New Roman, Bodoni, Garamond Sara font
  * need high resolution in screen of view
* Use sans serif fonts: Helvetica, Calibri, and Arial: text in back of room
* 30 point font
* Divide oldest investors age and divide by 2
* Reduce size to 66% to see if you can still read
* Slide titles optional: take home message of slide

#####Formatting Presentations to communicate Data Stories
* Consistent formatting throughout presentation 
* Max learning experience is 10 minutes
  * Build soft breaks
    * Summarize, or activities for user, just keep it smooth
* Rule of thirds, people will consistently look at the 4 corners of the center box
  * but within visual compartment or in line
  * Don’t use rule of thirds to data slides
  * Only use for transition slides
* Presentation formatting
  1. Check for typos then check again
  2. Bold is more readable than italics or underlining
  3. No distorted or fuzzy pictures
  4. Use 2-3 colors (but others can be used for highlighting)

#####Delivering Your Data Story
* What you will say 
* Add a question or ask people to raise their hand get audience to participate
* Use verbal transitions
  * How you will say them
