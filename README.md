# Intro
Using this data set to try and predict the a person's risk of stroke given their medical and personal history. The dataset has collected the information of 5110 people (though the data is cut down to 4014 as some rows included incomplete data was dropped from the dataframe) ranging from ages 19 to 82 and with the average age being 50.36. 
# Data Relationships
## Gender
For gender it the data seems to point to females being at higher risk for a stroke than males
![image](https://user-images.githubusercontent.com/56704804/165182522-dca1212e-277c-4f51-a734-8544f69327f4.png)
## Age
When age is plotted against the number of strokes the likelihood of strokes increases as a person ages
![download](https://user-images.githubusercontent.com/56704804/165183231-403e1746-3e82-48b8-8d22-55b11e065ab4.png)
## Average Glucose Levels
When looking at Average Glucose Levels high average glucose levels lead to an increased risk of strokes especially when a person is older in this graph a person that had a stroke will be plotted with an orange dot and a person that has not had a stroke will be plotted in with a blue dot
![download](https://user-images.githubusercontent.com/56704804/165183872-3473434c-1497-4fad-8129-2287a10db4fd.png)

# Plan for prediction and Findings
Analyzing the dataset some I found some interesting relationships, firstly smoking history doesn't seem to greatly increase the chance of stroke as much as I would have initially thought, this also holds true for bmi so it seems that weight doesn't greatly impact stroke risk either. The things that do increase the risk of stroke the most are high average glucose levels, age, and gender. To predict stroke chance I'll input age, gender, average glucose levels, work type, and smoking history and see if these are enough to predict wheither or not a person could suffer from a stroke.
