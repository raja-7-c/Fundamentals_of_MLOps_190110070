# Part 1

Perform some background research & answer the following questions:

1. In the notes of Week 1, we compared & contrasted MLOps with DevOps. In this question, you need to understand what is meant by the term ***AIOps***, & then contrast it with MLOps.

***AIOps***, sometimes referred to as ***Artificial Intelligence for IT Operations*** or ***Algorithmic IT Operations*** is a term invented by Gartner in 2016 as an industry category for Machine Learning analytics technology that enhances IT operations analytics.
AIOps platforms utilize big data, modern machine learning and other advanced analytics technologies to directly and indirectly enhance IT operations (monitoring, automation and service desk) functions with proactive, personal and dynamic insight. AIOps platforms enable the concurrent use of multiple data sources, data collection methods, analytical (real-time and deep) technologies, and presentation technologies. AIOps' ultimate goal is enhancing IT operations. The central process in AIOps is the intelligent filtering of signals our of the noise in IT systems. AIOps is an approach to use machine intelligence to solve this problem by collecting, processing, and observing intelligently IT operations data in order to identify root causes and propose solutions fast. In some cases, AIOps have the capability to solve problems without human intervention.

The term ***‘AIOps’*** is often used interchangeably with ***‘MLOps,’*** which is quite incorrect.

AIOps is all about supporting and reacting to its issues in real-time and providing analytics to your operations teams. These functions include performance monitoring, event analysis, correlation, and IT automation. According to Gartner, AIOps combines big data and machine learning to automate IT operations processes. Therefore, the end goal of AIOps is to automatically spot issues in day-to-day IT operations and proactively react to them using Artificial Intelligence. In fact, research shows that ***21% of organizations are planning to adopt AIOps within a year!***
MLOps, on the other hand, focuses on managing training and testing data that is needed to create machine learning models effectively. It is all about monitoring and management of ML models. It focuses on the Machine Learning operationalization pipeline. AIOps is all about applying cognitive computing techniques to improve IT operations, but it is not to be confused with MLOps.
Compared to MLOps, AIOps is a narrower practice that automates IT functions using machine learning. The goal of MLOps is to bridge the gap between operation teams and data scientists, and consequently between the execution and development of ML models. In contrast, the focus of AIOps is smart analysis of root causes and automated management of IT incidents. AIOps refers to the application of machine learning and artificial intelligence to IT operations to streamline repetitive tasks. MLOps, on the other hand, refers to the application of IT operations and DevOps practices in machine learning workflows.

2. ***Interpretable Machine Learning*** is another concept that has attracted lot of attention recently & is promoted by most of the MLOps frameworks. Explain what it means for a linear regression model to be interpretable. 

The biggest advantage of linear regression models is linearity: It makes the estimation procedure simple and, most importantly, these linear equations have an easy to understand interpretation on a modular level (i.e. the weights). This is one of the main reasons why the linear model and all similar models are so widespread in academic fields such as medicine, sociology, psychology, and many other quantitative research fields. For example, in the medical field, it is not only important to predict the clinical outcome of a patient, but also to quantify the influence of the drug and at the same time take sex, age, and other features into account in an interpretable way.

Estimated weights come with confidence intervals. A confidence interval is a range for the weight estimate that covers the "true" weight with a certain confidence. For example, a 95% confidence interval for a weight of 2 could range from 1 to 3. The interpretation of this interval would be: If we repeated the estimation 100 times with newly sampled data, the confidence interval would include the true weight in 95 out of 100 cases, given that the linear regression model is the correct model for the data.

Whether the model is the "correct" model depends on whether the relationships in the data meet certain assumptions, which are linearity, normality, homoscedasticity, independence, fixed features, and absence of multicollinearity.

***Normality***
It is assumed that the target outcome given the features follows a normal distribution. If this assumption is violated, the estimated confidence intervals of the feature weights are invalid.

***Homoscedasticity (constant variance)***
The variance of the error terms is assumed to be constant over the entire feature space. Suppose you want to predict the value of a house given the living area in square meters. You estimate a linear model that assumes that, regardless of the size of the house, the error around the predicted response has the same variance. This assumption is often violated in reality. In the house example, it is plausible that the variance of error terms around the predicted price is higher for larger houses, since prices are higher and there is more room for price fluctuations. Suppose the average error (difference between predicted and actual price) in your linear regression model is 50,000 Euros. If you assume homoscedasticity, you assume that the average error of 50,000 is the same for houses that cost 1 million and for houses that cost only 40,000. This is unreasonable because it would mean that we can expect negative house prices.

***Independence***
It is assumed that each instance is independent of any other instance. If you perform repeated measurements, such as multiple blood tests per patient, the data points are not independent. For dependent data you need special linear regression models, such as mixed effect models or GEEs. If you use the "normal" linear regression model, you might draw wrong conclusions from the model.

***Fixed features***
The input features are considered "fixed". Fixed means that they are treated as "given constants" and not as statistical variables. This implies that they are free of measurement errors. This is a rather unrealistic assumption. Without that assumption, however, you would have to fit very complex measurement error models that account for the measurement errors of your input features. And usually you do not want to do that.

***Absence of multicollinearity***
You do not want strongly correlated features, because this messes up the estimation of the weights. In a situation where two features are strongly correlated, it becomes problematic to estimate the weights because the feature effects are additive and it becomes indeterminable to which of the correlated features to attribute the effects.



# Part 2


[Amazon Web Services (AWS)](https://aws.amazon.com/) is a subsidiary of Amazon providing on-demand cloud computing platforms and APIs to individuals, companies, and governments, on a metered pay-as-you-go basis. To gain free, hands-on experience with the AWS platform, products, and services, one can start using the [AWS Free Tier](https://aws.amazon.com/free/) account. 

From Week 2 onwards, we will use some of the services of AWS to store our datasets, metadata, models & logs, and also to deploy trained models in production. All this can be achieved using the AWS Free Tier Account. 

Your task this week is to **follow the [instructions mentioned here](https://analyticshut.com/create-aws-account/) & create your own AWS Free Tier Account**, which you will use later in this course.

Once you create your account, use the [AWS Docs](https://docs.aws.amazon.com/) & explore some of the of services that the console offers (& **[Amazon S3](https://aws.amazon.com/s3/)** specifically).

