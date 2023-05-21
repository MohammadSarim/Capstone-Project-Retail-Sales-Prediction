# Capstone-Project-Retail-Sales-Prediction

**The Rossman Sales Prediction** dataset contains historical sales data for a retail store chain. The data includes various information about each store, such as competitor details, holidays, the number of customers, the date of each sale transaction, and the amount of sale on each day. Our task is to **forecast the "Sales"** for the test set.

To start with, we first gathered and **cleaned the data, handling any null values and ensuring its quality**. In order to improve the results, we **merged two datasets and performed necessary typecasting to ensure the proper visualization of features**. We then conducted a comprehensive **Exploratory Data Analysis (EDA)** by analyzing the data from different perspectives, including univariate, bivariate, and multivariate analyses. This allowed us to discover meaningful insights that could aid in making future decisions regarding the machine learning model pipeline.

Next, we focused on **feature engineering and data preprocessing**. We created new features such as "PromoDuration" and "CompetitionDuration" by utilizing other features that indirectly impact sales. Additionally, we addressed **multicollinearity** among independent variables by calculating the Variance Inflation Factor (VIF) and removing highly correlated features. Outliers were also detected and treated using the **Interquartile Range (IQR) technique**. We capped the outliers of continuous features within the 25th to 75th percentile range.

Furthermore, we identified that some features were categorical in nature and not understandable by machine learning models in their original form. To address this, we encoded the categorical features into numerical values using techniques such as **One-Hot Encoding**, as these categories were unordered.

Overall, through the steps of data gathering, cleaning, EDA, feature engineering, and data preprocessing, we have prepared the dataset for the subsequent machine learning model. These steps have helped us uncover insights, handle outliers, address multicollinearity, and transform categorical features into a suitable format for the model's input.

To ensure the normal distribution of our data, we applied various transformation techniques, such as **Logarithmic, Exponential, and Square Root transformations**. We also examined the quantile-quantile plot to visually assess the deviation of our data points from the normal distribution. Additionally, we utilized the **StandardScaler** from the sklearn library to scale the data.

With our final set of features prepared, we proceeded to split the data into training and testing sets. We then selected multiple machine learning algorithms and trained them using the training data. Subsequently, we evaluated the performance of each model on the testing data to assess their ability to predict sales for real-time scenarios. Among the algorithms we employed were **Linear Regression, Decision Trees, LightGBM, and XGBoost.**

Initially, even with regularisation techniques such as **Lasso, Ridge, and Elastic Net**, the simpler model of Linear Regression yielded a satisfactory **R2 score of 0.75 and an accuracy of 93% (100 - MAPE).** However, to capture more variance and further enhance our model's performance, we explored more complex models individually.

After training the datasets using Decision Trees, LightGBM, and XGBoost, we achieved a notable R2 score of 0.94. **The best accuracy of 97% and a mean absolute percentage error of only 2% were attained using XGBoost.** Moreover, we observed that the residuals had a mean of 0.0, indicating a desirable characteristic of a good residual plot, where the residuals are normally distributed.

Based on these experiments and evaluations, we selected XGBoost as our final optimal model for deployment. It demonstrated the highest accuracy with the least error among all the five models considered.

Throughout the process of building a machine learning model on the Rossman Sales Prediction Data, we employed a combination of data processing techniques, machine learning algorithms, and model evaluation skills. This task presented its fair share of challenges, and we encountered some setbacks along the way. However, by approaching the problem with the right mindset and leveraging our knowledge and expertise, we ultimately achieved success.

Our journey involved various steps, including data cleaning, feature engineering, and data transformation techniques to ensure the quality and normal distribution of the data. We explored multiple machine learning algorithms, such as Linear Regression, Decision Trees, LightGBM, and XGBoost, to find the best model for the task. Each algorithm was trained using appropriate training sets, and we evaluated their performance using metrics like **R2 score, accuracy, and mean absolute percentage error (MAPE).**

Although we encountered some failures during the experimentation process, we persisted and learned from those experiences to refine our approach. As a result, we were able to develop a robust machine learning model that could accurately predict sales up to six weeks in advance. This achievement highlights the significance of data processing, proper algorithm selection, and effective model evaluation techniques in creating successful predictive models.

Overall, the journey to building the Rossman Sales Prediction model was challenging yet rewarding. It demonstrated the importance of perseverance, knowledge, and adaptability in overcoming obstacles and achieving accurate sales forecasts.



