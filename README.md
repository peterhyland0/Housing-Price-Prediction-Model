# Housing Price Prediction Model
In this project, we look at the housing data of California. The data is loaded in and manipulated using Python code.
## Process
First, the data is read from the file, now we can manipulate the contents of the file. By calling data (the name of the variable with the data) we can see all the contents of the table. When you execute data.dropna(inplace=True), it will remove rows containing missing values from the DataFrame data and update data in place, meaning that the original DataFrame data will no longer contain rows with missing values.
The next part of code is used to split a dataset into training and testing sets.
sklearn.model_selection import train_test_split
X = data.drop(["median_house_value"], axis=1)
y = data["median_house_value"]
This is an example of the data processing I has to do in this project. I then created a linear regression model and a random forest regressor.
