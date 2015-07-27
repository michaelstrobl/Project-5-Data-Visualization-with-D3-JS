Project 5: Data Visualization with D3.js

Survivors of the Titanic

by: Michael Strobl, Nanodegree Data Analyst November Cohort


1. Dataset

The used Dataset: http://biostat.mc.vanderbilt.edu/wiki/pub/Main/DataSets/titanic3.xls

Description of the Dataset: http://biostat.mc.vanderbilt.edu/wiki/pub/Main/DataSets/titanic3info.txt

First, the Dataset is converted to a CSV file with Excel. Second, the Dataset is converted to a new one with only the relevant Variables.

Used Python Code for Conversion: “Datasets/titanic_csv_changer.py”

Now the Dataset is reduced to:

Total Data Points: 1309

Variables:
- Passenger Class: Class of the Titanic Passengers. Possible Classes: 1,2,3. 1 is the most expensive, 3 is the cheapest.
- Status: Status of the Passenger: Survived or Perished
- Sex: female or male
- Age: <14, 14-30, 31-50, >51
- Embarked: Port of Embarkation (C = Cherbourg; Q = Queenstown; S = Southampton)

2. Summary

The Titanic was the biggest passenger liner in the world and it sunk during its first ride where 1500 of 2200 passengers died. In the Data Visualization, you can see that certain parameters gave the passengers better chances of survival.
More People in Class 1 or Class 2 have survived than in Class 3 and people who embarked in Southampton than in the other two harbors. Additionally, women and children (below age of 14) survived rather than men and older people.

3. Design

I used stacked Bar Charts for this Data Visualization. It allows to represent different groups on top of each other and it’s good for comparison. Additionally, I added the Data Labels inside each of the stacked bars. For example, the values of 123 and 200 inside the first bar of Chart 1: It means that 123 people of Class 1 survived while 200 people of Class 1 died.

Survivors are shown in a light blue, while perished people get a light red color. With two different colors, the stacked bars are easier to perceive, differ and understand. A low value of saturation is more natural and gentle for the human’s eye.

When you hover over a stacked bar, you get also the related information.

In the top right of each graph, you can see the legend which indicates the survival status of a group.

4. Feedback

4.1 R Plots

Used Code: 'R Plots/plots.R'
Visible in: 'R Plots/R Plots.pdf'

Colors are too bright
  -> will be changed later
Nice Overview
No Title or Y-Axis labelled
  -> will be changed later

4.2 index1.html

Embarked NA values in Plot 4should be removed
	->  new CSV File (‘titanic_full.csv’) created where the two Embarked NA are 		removed manually
Colors: Survived people are red, while perished ones are blue. Makes no sense.
	-> New Colors where survived people are lightblue and perished ones are lightred
X-Axis in Plot 2 should be sorted
	-> X-Axis sorted in Plot 2
Data Labels in the Stacked Bar would be nicer for overview
	-> Data Labels included



5. Resources

http://www.perceptualedge.com/articles/visual_business_intelligence/rules_for_using_color.pdf

http://www.encyclopedia-titanica.org/children-on-titanic/

http://dimplejs.org/advanced_examples_viewer.html?id=advanced_bar_labels

http://stackoverflow.com/questions/18558045/dimple-js-add-data-labels-to-each-bar-of-the-bar-chart

https://en.wikipedia.org/wiki/Bar_chart

https://en.wikipedia.org/wiki/RMS_Titanic
