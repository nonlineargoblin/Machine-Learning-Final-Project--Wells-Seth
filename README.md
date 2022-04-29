# Intro
I'll be using this data set to try and predict the a person's risk of stroke given their medical and personal history. The dataset has collected the information of 5109 people ranging from ages 0 (ages less than 1 are expressed in decimals, for example a 6 month old baby would have an age of 0.5 in the dataset) to 82 and with the average age being 42.86.
# Data Relationships
## Gender
For gender the data seems to point to females being at higher risk for a stroke than males
![image](https://user-images.githubusercontent.com/56704804/166066282-d02e1eab-674e-4801-8004-a834d1a063be.png)
## Age
When age is plotted against the number of strokes, we can see that the older a person is the more likely they are to have a stroke. This graph was created using a dataset of 400+ of the patients where the first 200 non-stroke patient's data was concatinated to the 249 stroke patient's data. This was done to better show the correlation betweeen age and stroke risk.
![image](https://user-images.githubusercontent.com/56704804/165634674-c34ceded-64b9-4ceb-aad8-8922d89f6059.png)
## Average Glucose Levels
When looking at Average Glucose Levels, high average glucose levels lead to an increased risk of strokes especially when a person is older in this graph a person that had a stroke will be plotted with an orange dot and a person that has not had a stroke will be plotted in with a blue dot. This graph was created using a data set of 400+ patients in order to make a more readable scatterplot.
![image](https://user-images.githubusercontent.com/56704804/165602210-677a1801-6c22-4502-a1c4-abc5332b4964.png)
# Plan for prediction and Findings
Analyzing the dataset some I found some interesting relationships, firstly smoking history doesn't seem to greatly increase the chance of stroke as much as I would have initially thought, this also holds true for bmi so it seems that weight doesn't greatly impact stroke risk either. The things that do increase the risk of stroke the most are high average glucose levels, age, and gender. To predict stroke chance I'll input age, gender, average glucose levels, work type, hypertension, and smoking history and see if these are enough to predict wheither or not a person could suffer from a stroke.

# Statistics and Distributions
## Target Classification: Stroke
![image](https://user-images.githubusercontent.com/56704804/165641136-faaf4fe5-536f-4d67-a72b-31c851e0f144.png)

The distribution of the stroke category is highly skewed towards subjects that have not suffered from strokes: 1 is a person that has suffered from a stroke while 0 indicates a person who has not suffered from a stroke. In total out of the 5109 subjects, 249 have suffered from a stroke with the remaining 4860 not suffering from a stroke.

## Age
![image](https://user-images.githubusercontent.com/56704804/165642360-6f4ab40a-de69-4a82-9145-1cfd2cd05a7f.png)

For age the average is 43.22 with a standard deviation of of 22.61. The minimum age is 0 and the maxium age of 82.

## Gender
![image](https://user-images.githubusercontent.com/56704804/166066199-499ed34c-47f0-40fd-814b-2af65e4f2af1.png)

The data set has more females than males with 2994 females and 2115 males.

## Average Glucose Levels
![image](https://user-images.githubusercontent.com/56704804/166061342-b1a798f2-4193-4862-964e-5cf51d517166.png)

Average glucose levels is the measure of glucose in the patients blood.; The mean average glucose leve is 106.14 with a standard deviation of 45.285. The max level was recorded at 271 and the minimum of level of 55.12

# Encoding and Data Dropping
## Encoding
To encode my dataset I chose to encode the columns gender,work_type,ever_married, and smoking status using one-hot encoding (the encoding itself was done with the pandas.getdummies()). This was chosen as all of my categorical columns were non-ordinal and also they each had a small number of sub-categories(e.g male or female for gender) with work_type being the largest category with 5 sub-categories. The columns hypertension and heart disease were already encoded in the raw data set with 0 denoting no history of hypertension or heart diesease and 1 denoting a history of hypertension or heart diesease, therefore these columns were not encoded.
## Data Dropping
The only column That was removed in its entirety was the id column as ids were arbitrary and unique. I did remove a single row which had the patient's gender recorded as 'other', since it was the only entry in the dataset with that gender it didn't seem to be of much use and it also added an extra row when gender was encoded.
