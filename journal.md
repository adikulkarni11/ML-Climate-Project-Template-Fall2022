# ML and Climate Project Journal


### 10/4/22

Earlier this year, I pondered upon an [web article](https://sustainabilitymag.com/esg/how-nvidia-fighting-climate-change-omniverse) article about US gaming and computer graphics how they were tackling climate change. As a gaming and computer enthusiast, this article sounded very interesting. GPU's by far, consume alot of electricty and are major contributors in household electricty (myself included). Further, with the boom of crypto mining, many people over the last year have been buying several GPU's in hopes of one day becoming a crytpo giant. 

In the same article, Nvidia stated that they reduced their emissions by 15% per employee and set a goal to have 65% of its global electricity use come from renewable sources by the end of 2025. Along these lines, I decided to do my project regarding modeling GPU efficiency and how that ties into future energy consumption.

At the moment, I have been looking for a dataset for this task. I could curate my own dataset but I believe it would be too small to create valid and accurate predictions.

### 10/14/22 

After further research, I have realized that my initial project that included GPU data is extremely hard to find. So, I have deviated my project. My new project does still involve household emissions but in terms of CO2 equivalent. The data I have collected is from https://stats.oecd.org/Index.aspx?DataSetCode=air_ghg#. The project will put an emphasis on emissions from the residential sector. In addition, I will compare trends over time from 1990 to 2020 and observe how policies and laws have added value/ altered the charts. Further, using machine learning I will predict emissions for the current year and future.

### 10/21/22

The project is divided into two main phases: 
- Observing Trends in various countries CO2 emissions over time (1990-2020) and analyse climate policies to uncover trends and ties.
- Predict future emission data (2021,2022 and 2050) and inspect course.

### 10/31/22

Currently, I have been able to acquire emission data from 56 different countries. Speicifically, each of these countries have emission data from the year 1990 to 2020.
Further, I have generated charts of several of these countries which will benefit when I case study certain regions of the globe. For instance, I have already been able to compare climate change laws of countries such as Denmark and United States to observe patterns. In addition, I have a few side by side graph analysis already done (See case_study_1.png in src folder). 

The next steps is a deep analysis of this law and emission relationship. 

### 11/13/22

Over the last week, I have been looking into climate changes laws that have been passed within the last few years to predict the outcome or impact of it by 2025. In specific, I have looked into India, the USA, and Denmark. India for example had published their National Action Plan on Climate Change in 2008 which outlines eight “national missions" including solar, energy efficiency, sustainable habitat. There was a drastic decrease after this law. In 2022, India officially submitted its updated Nationally Determined Contributions (NDC) targets, having first announced them at COP26. Using this data, I am predicting their CO2e by 2025. I am currently finding deep relationships for Denmark and its laws before I start modeling using machine learning. Code updates will be provided next journal entry.

### 11/25/22

So far, I have generated two different types of models. Firstly, using the NeuralProphet API, I am modeling the CO2e emissions in the form of a yearly time series data. Although this is giving out great results, for some countries, I do see a slight discrepancy between the prediction and actual results as this is solely based on the Univariate data. On the other hand, I am modeling using Linear Regression specifically designed for univariate non-stationary (increasing) data. This seems to be a great way of predicting future emmissions as well.
