## Academic Success Rate Project

* Developed a predictive tool that can forecast whether students will complete their course or drop out after first semester. The results of this analysis can offer valuable insights into the reasons why students struggle to finish their education. By using this tool, institutions can devise effective strategies to prevent failure and dropout.
* Selected and optimized a machine learning model using GridSearchCV to achieve the optimal performance.
* Built a client facing API using flask.

### Code and Resources Used:
Python Version: 3.9.13 <br/>
Packages: pandas, numpy, matplotlib, seaborn, plotly, sklearn, xgboost, imblearn, flask, pickle, tqdm

### Data Description:
The dataset for this project contains information about students from various databases in a higher education institution. It includes demographics, socioeconomic and macroeconomic status, enrollment and progress data for the first and second semesters. The data was sourced from Zenodo, and a detailed description of the columns can be found here.

### Exploratory Data Analysis:
This project aims to conduct an exploratory data analysis using family background and past academic records to gain insights into why students struggle to complete their education. Factors such as younger enrollment age, scholarships, and choice of courses are found to have a significant impact on academic success rates. 
![alt text](https://github.com/vvalmispild/Academic_Success_Rate_project/blob/main/marital_status_average_age.png)

### Machine Learning Prediction:
In this project, we also aim to create a machine learning algorithm that can anticipate a student's academic progress after the first semester, with a particular emphasis on forecasting whether they will successfully complete the course or withdraw. 

#### Model Building and performance:
I tried different models: <br/>
<sup>
Metrics | Logistc Regression |	Random Forest | Balanced Random Forest | KNN | SVM | XGBOOST |
|----------|:---------:|------:|----------|:---------:|------:|------:|
accuracy |	0.860606	| 0.846281	|  0.841873	| 0.831680	 | 0.841598 | 0.851240 |
precision |	0.858474	| 0.854389	 | 0.873773	| 0.831427	 | 0.824737 | 0.858500 |
recall	|  0.923704	| 0.910246 |	0.868328	| 0.907213	 | 0.939163 | 0.904835 |
f1_micro |	0.860606	| 0.848485	 | 0.841047	| 0.831680	 | 0.841598 | 0.851240 |
f1_macro |	0.849770	| 0.838368 |	0.832926	| 0.817776	 | 0.825529 | 0.841179 |
</sup>
Logistic regression is chosen as the optimal model. <br/>
Next, the model was tuned with optimal hyperparameters.

### Productionization:
To productionize the project, I created a Flask API endpoint that runs on a local web server by following the tutorial provided in the reference section. The endpoint receives input variables from a web application request and generates a forecasting estimate, which is then returned as output. To launch the web application, the command "$ python app.py" is executed, and the resulting GUI can be accessed by opening http://127.0.0.1:5000/ in a web browser. The GUI should resemble the one shown below.

### References:
<sup>
1) https://zenodo.org/record/5777340#.ZAJvJy8w1QK <br/>
2) https://www.pordata.pt/en/portugal/mean+age+on+first+marriage+by+sex-421-5200 <br/>
3) https://medium.com/towards-data-science/how-to-easily-deploy-machine-learning-models-using-flask-b95af8fe34d4 
</sup>
