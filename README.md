# Intro
Using this data set to try and predict the a person's risk of stroke given their medical and personal history. The dataset has collected the information of 5110 people ranging from ages 0 (ages less than 1 are expressed in decimals, for example a 6 month old baby would have an age of 0.5 in the dataset) to 82 and with the average age being 50.36. 
# Data Relationships
## Gender
For gender the data seems to point to females being at higher risk for a stroke than males
![image](https://user-images.githubusercontent.com/56704804/165182522-dca1212e-277c-4f51-a734-8544f69327f4.png)
## Age
When age is plotted against the number of strokes, we can see that the older a person is the more likely they are to have a stroke.
![image](https://user-images.githubusercontent.com/56704804/165613906-2ee3ddcb-51c9-4bd0-acf6-4d99204e3fb8.png)
## Average Glucose Levels
When looking at Average Glucose Levels, high average glucose levels lead to an increased risk of strokes especially when a person is older in this graph a person that had a stroke will be plotted with an orange dot and a person that has not had a stroke will be plotted in with a blue dot.
![image](https://user-images.githubusercontent.com/56704804/165602210-677a1801-6c22-4502-a1c4-abc5332b4964.png)
# Plan for prediction and Findings
Analyzing the dataset some I found some interesting relationships, firstly smoking history doesn't seem to greatly increase the chance of stroke as much as I would have initially thought, this also holds true for bmi so it seems that weight doesn't greatly impact stroke risk either. The things that do increase the risk of stroke the most are high average glucose levels, age, and gender. To predict stroke chance I'll input age, gender, average glucose levels, work type, and smoking history and see if these are enough to predict wheither or not a person could suffer from a stroke.
