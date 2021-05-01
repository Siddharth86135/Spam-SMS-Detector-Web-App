# Car-Price-Prediction-Web-App

## Objective

We try to classify SMS messages as SPAM or NOT SPAM using various ML algorithms. The notebook (spam_classifier.ipynb)consists steps to process and explore the dataset, convert messages to vectors and applying ML techniques for the same.

The notebook(spam_classifier_rnn.ipynb) uses a Recurrent Neural Network (RNN) and LSTM to classify the messages. RNNs are networks with loops in them, allowing information from previous time step to persist capable of handling long-term dependencies.

In this project, I have explored and compared text preprocessing and feature selection methods among word count, character count, bag of words, removing stop words, stemming, and Lemmatization. Logistic regression classifier is used to detect ham or spam SMS messages. The dataset is a collection of 5,574 text messages in English, taggled according being ham (legitimate) or spam. 

## Dataset

The Dataset is a set of SMS tagged messages  collected for SMS Spam research. It contains one set of SMS messages in English of 5,574 messages, tagged acording being ham (legitimate) or spam.

The dataset is available [here.](https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection)

Example Messages:

```
ham What you doing?how are you? 
ham Ok lar... Joking wif u oni... 
ham dun say so early hor... U c already then say... 
ham MY NO. IN LUTON 0125698789 RING ME IF UR AROUND! H* 
ham Siva is in hostel aha:-. 
ham Cos i was out shopping wif darren jus now n i called him 2 ask wat present he wan lor. Then he started guessing who i was wif n he finally guessed darren lor. 
spam FreeMsg: Txt: CALL to No: 86888 & claim your reward of 3 hours talk time to use from your phone now! ubscribe6GBP/ mnth inc 3hrs 16 stop?txtStop 
spam Sunshine Quiz! Win a super Sony DVD recorder if you canname the capital of Australia? Text MQUIZ to 82277. B 
spam URGENT! Your Mobile No 07808726822 was awarded a L2,000 Bonus Caller Prize on 02/09/03! This is our 2nd attempt to contact YOU! Call 0871-872-9758 BOX95QU 

```


## Model Deployement

Taking ML models from conceptualization to production is typically complex and time-consuming. You have to manage large amounts of data to train the model, choose the best algorithm for training it, manage the compute capacity while training it, and then deploy the model into a production environment. Amazon SageMaker reduces this complexity by making it much easier to build and deploy ML models. After you choose the right algorithms and frameworks from the wide range of choices available, SageMaker manages all of the underlying infrastructure to train your model at petabyte scale, and deploy it to production.

1. Machine Learning Model Deployment Using Heroku Cloud

Heroku is a cloud Platform as a Service that helps developers quickly deploy, manage, and scale moderns applications without infrastructure headaches.f you want to deploy your model for the first time, I recommend that you try Heroku because it is flexible and easy to use.

It offers a wide range of services and tools to speed up your development and helps you avoid starting everything from scratch. It also supports several widely used programming languages like Python, Java, PHP, Node, Go, Ruby, Scala, and Clojure.

The good thing about Heroku is that it makes it easy to create, deploy and manage your app. You can do this right from the command line using the Heroku CLI (available for Windows, Linux, and Mac users).

On the deployment part, you can upload your trained machine learning model and source code onto Heroku by linking your Github repository to your Heroku account.


2. Machine Learning Model Deployment Using Microsoft Azure Functions

Azure Functions is a serverless cloud service provided by Microsoft Azure as a Functions-as-a-service (FaaS). Azure functions help developers offload infrastructure management tasks and focus on running their applications.

With serverless, you can write a snippet of code that runs your model and then deploy the code and machine learning model on Azure Functions and call it for prediction as an API. Azure functions are similar to Google cloud functions.

Azure Functions supports different functions developed in C#, F#, Node.js, Python, PHP, JavaScript, Java 8, Powershell Core, and TypeScript.

If you have a big machine learning model, then Azure functions is the right choice for you. It supports the deployment of large ML packages such as deep learning frameworks (Tensorflow and Pytorch).


3. Machine Learning Model Deployment Using AWS Lambda

AWS Lambda is a serverless computing service provided by Amazon as part of Amazon Web Services. AWS lambda helps you run your code without managing the underlying infrastructure.

With Lambda, you can upload your code in a container image or zip file. Lambda will automatically allocate computational power to run your code based on the incoming requests or events without requiring you to configure anything.

AWS Lambda allows your code to be associated with other AWS resources such as Amazon DyanamoDB table, Amazon S3 bucket, Amazon SNS notification, and Amazon Kinesis stream. Therefore you can easily deploy your machine learning model on AWS Lambda, and you can access it through an API using Amazon API Gateway. You can write Lambda functions in the following supported programming languages: Python, Java, Go, PowerShell, Node.js, Ruby, and C# code.

AWS Lambda is very cheap because you only pay when you invoke the lambda function (that is, when you make prediction requests). It can save lots of money compared to the cost of running containers or Virtual Machines. If you want to monitor the lambda functions you have created, AWS Lambda will do it on your behalf.

AWS Lambda will monitor real-time metrics including error rates, total requests, function-level concurrency usage, latency, and throttled requests through Amazon CloudWatch. Then you can view the statistics for each lambda function by using AWS Lambda Console or Amazon CloudWatch Console.
