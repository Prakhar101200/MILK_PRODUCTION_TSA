Milk Production Forecasting Project

#Overview
This projects aims to perform a time series analysis over the dataset of milk production.

#Dataset
The dataset is provided in both excel and csv format nameing '/content/monthly-milk-production-pounds-p.csv'. This dataset is provided by the Eduonix learing center. This dataset contains 2 columns: 'Months' and 'Milk production per cow in pounds'.

#Approach #Exploratory Data Analysis (EDA):

Visualize the time series data to identify patterns, trends, and seasonality. Calculate summary statistics and explore the distribution of female birth counts. Identify outliers or missing values that need to be addressed.
Also, check for the stationarity of the data and perfore sstatiscal analysis steps to make it stationary.

#Model Selection
After checking the the data and making it stationary, we went with the model creation and model training. For the firstt choice we went ARIMA, but, due to multiple trials and errors faced we took the decision to not go with this model. 
Therefore, we went with the SARIMAX model. In this model, we first checked for the best combinations of the pdq for both the production of the milk column and the seasonal first difference column which we calculated to make our data stationary.

After finding the best combinations for both the columns we trained the model. This model gave us promising results.

#Model Evaluation
For checking the effectiveness of the model we predicted data through our model and checked them over the graph to see if the model is giving right predictions over the testing part of the data.
The  plotting gave us a good precise predictions on the dataset.
Hence, we forecasted few more future dates and used them to predict our milk production for the future. 
This gave us high accuracy on the future prediction.

#Hardships
There were two issues faced while working.
1. while creating our model our first choice was the ARIMA model for training but the errors couldn't let us train the data with the ARIMA. This was the error which I faced [LinAlgError: LU decomposition error.]. So we removed the code part of the ARIMA from here and went with the SARIMAX.

2. Another issue we went through was in the SARIMAX model. The problem we faced was with the parameters. So, to solve it we went through several articles on the web and found the solution.

#Future_Scope
As there will always be a scope for improvement in the future. Therefore, with more data and more experimentaion we can surely create more accurate model.

#Contributors
Prakhar Raj Gupta

#Acknowledgements
.I would like to acknowledge the numerous sources available over the internet that helped me throughout this project hardships.

.Along with this, I would like to acknowledge "Miss Suchisita Mondal" for teaching me this concept in the class.

.I would also like to appreciate 'Eduonix' for creating this Data Science Certification Module that enabled me to explore the world of Data Science and make myself more knowledgable in the concepts. .Lastly, I would like to appreciate myself for not giving up and fighting all obstacles on daily basis, whether its in coding or any other theoritical concepts or in life.

#Code Structure main.ipynb: Google Colab containing the main code for data loading, EDA, model training, and evaluation. README.md: README file providing an overview of the project, dataset, approach, and code structure.
