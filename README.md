# Intro
Using this data set to try and predict the a person's risk of stroke given their medical and personal history. The dataset has collected the information of 5110 people ranging from ages 0 (ages less than 1 are expressed in decimals, for example a 6 month old baby would have an age of 0.5 in the dataset) to 82 and with the average age being 42.86. 
# Data Relationships
## Gender
For gender the data seems to point to females being at higher risk for a stroke than males
![image](https://user-images.githubusercontent.com/56704804/165633247-eee934b2-a81b-43b3-b919-ee9e4d8bcef2.png)
## Age
When age is plotted against the number of strokes, we can see that the older a person is the more likely they are to have a stroke.
![image](https://user-images.githubusercontent.com/56704804/165634674-c34ceded-64b9-4ceb-aad8-8922d89f6059.png)
## Average Glucose Levels
When looking at Average Glucose Levels, high average glucose levels lead to an increased risk of strokes especially when a person is older in this graph a person that had a stroke will be plotted with an orange dot and a person that has not had a stroke will be plotted in with a blue dot.
![image](https://user-images.githubusercontent.com/56704804/165602210-677a1801-6c22-4502-a1c4-abc5332b4964.png)
# Plan for prediction and Findings
Analyzing the dataset some I found some interesting relationships, firstly smoking history doesn't seem to greatly increase the chance of stroke as much as I would have initially thought, this also holds true for bmi so it seems that weight doesn't greatly impact stroke risk either. The things that do increase the risk of stroke the most are high average glucose levels, age, and gender. To predict stroke chance I'll input age, gender, average glucose levels, work type, and smoking history and see if these are enough to predict wheither or not a person could suffer from a stroke.

# Statistics and Distributions
## Target Classification: Stroke
![image](https://user-images.githubusercontent.com/56704804/165641136-faaf4fe5-536f-4d67-a72b-31c851e0f144.png)

The distribution of the stroke category is highly skewed towards subjects that have not suffered from strokes: 1 is a person that has suffered from a stroke while 0 indicates a person who has not suffered from a stroke. In total out of the 5110 subjects, 249 have suffered from a stroke with the remaining 4861 not suffering from a stroke.

## Age
![image](https://user-images.githubusercontent.com/56704804/165642360-6f4ab40a-de69-4a82-9145-1cfd2cd05a7f.png)

For age the average is 43.22 with a standard deviation of of 22.61. The minimum age is 0 and the maxium age of 82.

## Gender
![image](https://user-images.githubusercontent.com/56704804/165642985-d1223e19-efdd-44aa-b512-8fbe5f987c54.png)

The data set has more females than males with 2994 females and 2115 males.
