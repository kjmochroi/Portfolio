# Predicting Metro Interstate Traffic Volume

### By KJ MoChroi
#### May 2023  

In this project I am attempting to predict the traffic volume of an interstate highway using a multivariate time series dataset of metro interstate traffic volume in Minneapolis-St Paul, MN for westbound I-94. I am hoping to address the issue of optimal transit timing. I ended up utilizing three different models (Vector AutoRegression, AutoRegressive Integrated Moving Average, and Random Forest Regressor) because I wasn't happy with the results from the first two models.

This multivariate, sequential, time-Series dataset was found on the UC Irving database website. The traffic data was provided by the Minnesota Department of Transportation and the weather data was provided by OpenWeatherMap. The dataset has 8 training features including holiday, temperature, rain, snow, clouds, weather brief description, weather longer description and one target feature which is traffic volume on westbound I-94, with 48,204 hourly readings. The data was collected from 2012 to 2018 and has integer and real number characteristics. 

In this project I trained three different models (VAR, ARIMA, RFR) which are avaialble to see as jupyter notebook files or PDFs. I also have a white paper describing the project, and a powerpoint audio visual presentation available for viewing. Additionally, I included 10 questions from the audience as well as the answers to those questions as a pdf. Please note that I changed my name in 2023 and thus the powerpoint refers to me by my former name.
