Artificial Intelligence (AI) Job Roles Salary Prediction
![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white) ![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white) ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white) ![Streamlit](https://img.shields.io/badge/streamlit-%23FF4B4B.svg?&style=for-the-badge&logo=streamlit&logoColor=white)
====================================

Teams
------------
1. [Ari Adhi Hermawan](https://github.com/aridiawan)
2. [Faisal Nur Khairudin](https://github.com/fnkhairudin)

Machine Learning Project Collaboration
------------
Build a model for predicting data scienctist job salary.

How to use
------------
1. Click this [streamlit link](https://data-scientist-salary-prediction-8memihknsetmjtajyjrxns.streamlit.app/)!
2. Input your data
3. Click prediction button

Business Problem
------------
This site collects salary information anonymously from professionals all over the world in the AI, ML, Data Science space and makes it publicly available for anyone to use, share and play around with.

The primary goal is to have data that can provide better guidance in regards to what's being paid globally. So newbies, experienced pros, hiring managers, recruiters and also startup founders or people wanting to make a career switch can make better informed decisions.

Context
------------
The field of artificial intelligence (AI) encompasses a wide range of job roles, including machine learning engineers, data scientists, AI researchers, natural language processing specialists, and more. Each of these roles may command different salary levels based on factors like expertise, location, and industry. Accurate salary predictions are crucial for attracting and retaining AI talent.

Problem Statement
------------
The AI industry has been experiencing rapid expansion and transformation. New breakthroughs, applications, and technologies emerge regularly, leading to an ever-evolving landscape. As AI matures, it diversifies into specialized subfields and roles. These roles often require distinct sets of skills, expertise, and responsibilities. With the rapid growth and specialization within the AI industry, **employers and job seekers require insights into the competitive salary ranges associated with various AI job roles**. **This information is essential for recruitment, budgeting, and salary negotiations**.

Employers in the AI sector face the challenge of attracting and retaining top talent. To do so, they must be well-informed about the competitive salary ranges for various AI job roles. **Employers** need to know how much budget they should allocate for hiring AI professionals **without overpaying or underpaying**.

Job seekers in the AI field seek clarity about the compensation they can expect for their skills and expertise. Different AI job roles come with varying salary expectations, and job seekers want insights into what constitutes a fair and competitive offer. This information empowers **job seekers** to make informed decisions about job opportunities and **negotiate fair compensation** packages.

Goals
------------
With the problem above, we can determine our goals (solution) as: Provides salaries prediction by minimizing errors so that it is not too high and not too low.

Project Stakeholders
------------
**AI Job Seekers**: Individuals pursuing careers in the AI field.
**Human Resources Departement**: Personnel responsible for recruitment and compensation negotiations within AI.

Analytic Approach
------------
We will use Regression Model as method to achieve the goal.

Regression is a type of Machine learning which helps in finding the relationship between independent and dependent variable. In simple words, Regression can be defined as a Machine learning problem where we have to predict discrete values like price, rating, fees, salary, etc [Raghav Agrawal](https://www.analyticsvidhya.com/blog/2021/05/know-the-best-evaluation-metrics-for-your-regression-model/).

Metric Evaluation
------------
Evaluation metrics are quantitative measures used to assess the performance and effectiveness of a statistical or machine learning model. These metrics provide insights into how well the model is performing and help in comparing different models or algorithms (Tavish Srivastava).

Regression machine learning models have various metrics such as MAE, MAPE, and R-squared.

- **Mean Absolute Error(MAE)** is a very simple metric which calculates the absolute difference between actual and predicted values [Raghav Agrawal](https://www.analyticsvidhya.com/blog/2021/05/know-the-best-evaluation-metrics-for-your-regression-model/).
- **Mean Absolute Percentage Error (MAPE)** measures the precision of the forecasts by showing the average percent difference between forecasts and actual activities regardless of whether the individual forecasts were too high or too low. A MAPE less than 5% is considered as an indication that the forecast is acceptably accurate. A MAPE greater than 10% but less than 25% indicates low, but acceptable accuracy and MAPE greater than 25% very low accuracy, so low that the forecast is not acceptable in terms of its accuracy [Swanson, David A](https://escholarship.org/content/qt1f71t3x9/qt1f71t3x9.pdf?t=o5wul1#:~:text=A%20MAPE%20less%20than%205,in%20terms%20of%20its%20accuracy.).
- **R squared (R²)** is a popular metric for identifying model accuracy. It tells how close are the data points to the fitted line generated by a regression algorithm. A larger R squared value indicates a better fit. This helps us to find the relationship between the independent variable towards the dependent variable. R² score ranges from 0 to 1. The closest to 1 the R², the better the regression model is. If R² is equal to 0, the model is not performing better than a random model [Shweta Goyal](https://medium.com/analytics-vidhya/evaluation-metrics-for-regression-models-c91c65d73af#:~:text=R%20squared%20is%20a%20popular,variable%20towards%20the%20dependent%20variable.).

Model Limitation
------------
1. This model is for educational purposes only and demonstrate how machine learning is works. Not for production phase.
2. This dataset has been taken from 2020-2023 (Latest downloaded: September 6, 2023 at 09:58 AM). Therefore, if you use this model in 3-5+ years later to predict how much your salary will be, probably the accuracy of predicted salary is low.

Conclusion
------------
1. The best model used for salary prediction is XGBoost.
2. The prediction results can be off by approximately US$ 38897 (MAE) from the actual salary, or in percentage terms the salary prediction will be off by approximately 31.82% (MAPE) from the actual salary.
3. Experience level is the most importance feature, the higher your experience, the greater the salary is. (in this order: Entry-level / Junior (EN), Mid-level / Intermediate (MI), Senior-level / Expert (SE), Executive-level / Director (EX)).

Recommendation
------------
Things that can be done to improve model performance:
- Add some features such as:
    - `experience year`: How many years of experience in that field,
    - `education level`,
    - etc
- Collect more data
- Add more parameters when perform hyperparameter tuning to get best parameters. Try several methods/pakcage, for instance optuna.
- Try more complex model like Time Series Forecasting and/or Deep Learning
- Track your model experiment when perform benchmark modelling until hyperparameter tuning with one of this framework such as MLflow, hugging face, etc.