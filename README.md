## Academic Success Rate Project

### Data Description

The dataset for this project contains information about undergraduate students from various databases in a higher education institution. It includes demographics, socioeconomic and macroeconomic status, enrollment and progress data for the first and second semesters. The data was sourced from Zenodo, and a detailed description of the columns can be found here.

### Exploratory Data Analysis

This project aims to conduct an exploratory data analysis using family background and past academic records to gain insights into why students struggle to complete their education. Factors such as younger enrollment age, scholarships, and choice of courses are found to have a significant impact on academic success rates. Multicollinearity is observed for some groups, including Curricular units 1st/2nd semestr groups, Nationality, and International, which need to be considered while building a machine learning model.

### Machine Learning Prediction

In this project, we also aim to create a machine learning algorithm that can anticipate a student's academic progress after the first semester, with a particular emphasis on forecasting whether they will successfully complete the course or withdraw. The model was deployed using Flask, and the python object was converted into a character stream using pickling to include all the information required to reconstruct the object in a different python script.

### References

https://zenodo.org/record/5777340#.ZAJvJy8w1QK
https://www.kaggle.com/code/nawazkhanpathan/end-to-end-student-s-academic-success-rate-predict
https://www.pordata.pt/en/portugal/mean+age+on+first+marriage+by+sex-421-5200
https://www.youtube.com/watch?v=xi0vhXFPegw&list=LL&index=25&t=2141s
https://medium.com/towards-data-science/how-to-easily-deploy-machine-learning-models-using-flask-b95af8fe34d4
