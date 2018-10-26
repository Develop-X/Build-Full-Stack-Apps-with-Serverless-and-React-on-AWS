# Build-Full-Stack-Apps-with-Serverless-and-React-on-AWS

[![Price](https://img.shields.io/badge/price-FREE-0098f7.svg)](https://github.com/Develop-X/Build-Full-Stack-Apps-with-Serverless-and-React-on-AWS/blob/master/LICENSE)

> This project is inspired from [Serverless Stack](https://serverless-stack.com/)

> The structure of README is inspired from [GoogleCloudPlatform Demo](https://github.com/GoogleCloudPlatform/microservices-demo)

Build a full-stack production ready note taking app using Serverless and React on AWS (Lambda, IAM, S3, Cognito, API Gateway, DynamoDB, Route 53, CloudFront, Certificate Manager, Amazon CloudWatch). 

<details>
  <summary><strong>Presentation</strong></summary>

- [ Serverless Stack - pdf](https://s3.amazonaws.com/anomaly/ServerlessStack/ServerlessStack-v3.3.1.pdf)

- Step-by-step instructions with screenshots for setting up your AWS services
- Build a REST API backend with our Serverless tutorial
- Easy to understand explanations for creating a single-page application with our React.js tutorial
- Over 100 chapters that take you all the way from creating your AWS account to deploying your app on your own domain
- Complete code samples hosted on GitHub for both the backend and frontend

</details>

# Table of contents

* [INTRODUCTION](https://github.com/Develop-X/Build-Full-Stack-Apps-with-Serverless-and-React-on-AWS#introduction)
** What is Serverless? ** What is AWS Lambda? ** Why create Serverless apps? 
* [SET UP YOUR AWS ACCOUNT](https://github.com/Develop-X/Build-Full-Stack-Apps-with-Serverless-and-React-on-AWS#set-up-your-aws-account)
** Create an IAM user ** What is IAM ** What is an ARN ** Conﬁgure the AWS CLI
* [SETTING UP THE SERVERLESS BACKEND](https://github.com/Develop-X/Build-Full-Stack-Apps-with-Serverless-and-React-on-AWS#setting-up-the-serverless-backend)
** Create a DynamoDB table ** Create an S3 bucket for ﬁle uploads ** Create a Cognito user pool ** Create a Cognito test user **Set up the Serverless Framework ** Add support for ES6/ES7 JavaScript
* [BUILDING A SERVERLESS REST API](https://github.com/Develop-X/Build-Full-Stack-Apps-with-Serverless-and-React-on-AWS#building-a-serverless-api)
** Add a create note API ** Add a get note API ** Add a list all the notes API ** Add an update note API ** Add a delete note API
* [DEPLOYING THE BACKEND](https://github.com/Develop-X/Build-Full-Stack-Apps-with-Serverless-and-React-on-AWS#deploying-the-backend)
** Deploy the APIs ** Create a Cognito identity pool ** Cognito user pool vs identity pool ** Test the APIs
* [SETTING UP A REACT APP](https://github.com/Develop-X/Build-Full-Stack-Apps-with-Serverless-and-React-on-AWS#setting-up-a-react-app)
** Create a new React.js app ** Add app favicons ** Set up custom fonts ** Set up Bootstrap ** Handle routes with React Router ** Create containers ** Adding links in the navbar ** Handle 404s ** Conﬁgure AWS Amplify
* [BUILDING A REACT APP](https://github.com/Develop-X/Build-Full-Stack-Apps-with-Serverless-and-React-on-AWS#building-a-react-app)
** Create a login page Login with AWS Cognito ** Add the session to the state ** Load the state from the session ** Clear the session on logout ** Redirect on login and logout ** Give feedback while logging in ** Create a signup page ** Create the signup form ** Signup with AWS Cognito ** Add the create note page ** Add the create note page **Call the create API Upload a ﬁle to S3 ** List all the notes ** Call the list API ** Display a note ** Render the note form ** Save changes to a note ** Delete a note ** Set up secure pages ** Create a route that redirects ** Use the redirect routes ** Redirect on login
* [DEPLOYING A REACT APP ON AWS](https://github.com/Develop-X/Build-Full-Stack-Apps-with-Serverless-and-React-on-AWS#deploying-a-react-app-on-aws)
** Deploy the Frontend ** Create an S3 bucket ** Deploy to S3 ** Create a CloudFront distribution ** Set up your domain with CloudFront ** Set up www domain redirect ** Set up SSL ** Deploy updates ** Update the app ** Deploy again
* [INTRODUCTION TO AUTOMATION](https://github.com/Develop-X/Build-Full-Stack-Apps-with-Serverless-and-React-on-AWS#Introduction-to-automation)
** Getting production ready
* [ICREATE A NEW BACKEND](https://github.com/Develop-X/Build-Full-Stack-Apps-with-Serverless-and-React-on-AWS#create-a-new-backend)
** Initialize the backend repo ** Organize the backend repo
* [INFRASTRUCTURE AS CODE](https://github.com/Develop-X/Build-Full-Stack-Apps-with-Serverless-and-React-on-AWS#infrastructure-as-code)
** What is Infrastructure as Code? ** Conﬁgure DynamoDB in Serverless ** Conﬁgure S3 in Serverless ** Conﬁgure Cognito User Pool in Serverless ** Conﬁgure Cognito Identity Pool in Serverless ** Use environment variables in Lambda functions ** Deploy your Serverless infrastructure
* [ADDING A STRIPE BILLING API](https://github.com/Develop-X/Build-Full-Stack-Apps-with-Serverless-and-React-on-AWS#adding-a-stripe-billing-api)
** Working with 3rd party APIs ** Setup a Stripe account ** Add a billing API ** Load secrets from env.yml ** Test the billing API
* [ADDING UNIT TESTS](https://github.com/Develop-X/Build-Full-Stack-Apps-with-Serverless-and-React-on-AWS#adding-unit-tests)
** Unit tests in Serverless
* [AUTOMATING SERVERLESS DEPLOYMENTS](https://github.com/Develop-X/Build-Full-Stack-Apps-with-Serverless-and-React-on-AWS#automating-serverless-deployments)
** Automating Serverless deployments ** Setting up your project on Seed ** Conﬁgure secrets in Seed ** Deploying through Seed ** Set custom domains through Seed ** Test the conﬁgured APIs ** Monitoring deployments in Seed
* [CONNECT TO THE NEW BACKEND](https://github.com/Develop-X/Build-Full-Stack-Apps-with-Serverless-and-React-on-AWS#connect-to-the-new-backend)
** Initialize the frontend repo ** Manage environments in Create React App
* [ADDING A BILLING FORM](https://github.com/Develop-X/Build-Full-Stack-Apps-with-Serverless-and-React-on-AWS#adding-a-billing-form)
** Create a settings page ** Add Stripe keys to conﬁg ** Create a billing form ** Connect the billing form
* [AUTOMATING REACT APP DEPLOYMENTS](https://github.com/Develop-X/Build-Full-Stack-Apps-with-Serverless-and-React-on-AWS#automating-react-app-deployments)
** Automating React Deployments ** Create a build script ** Setting up your project on Netlify ** Custom Domains in Netlify ** Frontend workﬂow
* [CONCLUSION](https://github.com/Develop-X/Build-Full-Stack-Apps-with-Serverless-and-React-on-AWS#conclusion)
** Wrapping up ** Futher reading ** Giving back ** Changelog ** Staying up to date

<details>
  <summary><strong>Technologies & Services</strong></summary>

  We’ll be using the following set of technologies and services to build our serverless application.
* Lambda (https://aws.amazon.com/lambda/) & API Gateway (https://aws.amazon.com/apigateway/) for our serverless API 
* DynamoDB (https://aws.amazon.com/dynamodb/) for our database 
* Cognito (https://aws.amazon.com/cognito/) for user authentication and securing our APIs 
* S3 (https://aws.amazon.com/s3/) for hosting our app and ﬁle uploads 
* CloudFront (https://aws.amazon.com/cloudfront/) for serving out our app 
* Route 53 (https://aws.amazon.com/route53/) for our domain 
* Certiﬁcate Manager (https://aws.amazon.com/certiﬁcate-manager) for SSL 
* React.js (https://facebook.github.io/react/) for our single page app 
* React Router (https://github.com/ReactTraining/react-router) for routing Bootstrap (http://getbootstrap.com) for the UI Kit Stripe (https://stripe.com) for processing credit card payments Seed (https://seed.run) for automating Serverless deployments Netlify (https://netlify.com) for automating React deployments GitHub (https://github.com) for hosting our project repos.

You need Node v8.10+ and NPM v5.5+

</details>

## Part I
### Here is what is covered in order.
#### For the backend:
* Conﬁgure your AWS account 
* Create your database using DynamoDB 
* Set up S3 for ﬁle uploads 
* Set up Cognito User Pools to manage user accounts 
* Set up Cognito Identity Pool to secure our ﬁle uploads 
* Set up the Serverless Framework to work with Lambda & API Gateway 
* Write the various backend APIs

#### For the frontend:
* Set up our project with Create React App
* Add favicons, fonts, and a UI Kit using Bootstrap
* Set up routes using React-Router 
* Use AWS Cognito SDK to login and signup users 
* Plugin to the backend APIs to manage our notes 
* Use the AWS JS SDK to upload ﬁles 
* Create an S3 bucket to upload our app 
* Conﬁgure CloudFront to serve out our app 
* Point our domain with Route 53 to CloudFront 
* Set up SSL to serve our app over HTTPS

## Part II
### Here is what is covered in order.
#### For the backend:
* Conﬁgure DynamoDB through code
* Conﬁgure S3 through code 
* Conﬁgure Cognito User Pool through code 
* Conﬁgure Cognito Identity Pool through code 
* Environment variables in Serverless Framework 
* Working with the Stripe API 
* Working with secrets in Serverless Framework 
* Unit tests in Serverless 
* Automating deployments using Seed 
* Conﬁguring custom domains through Seed 
* Monitoring deployments through Seed

#### For the frontend
* Environments in Create React App 
* Accepting credit card payments in React 
* Automating deployments using Netlify 
* Conﬁgure custom domains through Netlify

# Introduction

## What is Serverless?

Traditionally, we’ve built and deployed web applications where we have some degree of control over the HTTP requests that are made to our server. Our application runs on that server and we are responsible for provisioning and managing the resources for it. There are a few issues with this.

1. We are charged for keeping the server up even when we are not serving out any requests.
2. We are responsible for uptime and maintenance of the server and all its resources.
3. We are also responsible for applying the appropriate security updates to the server.
4. As our usage scales we need to manage scaling up our server as well. And as a result manage scaling it down when we don’t have as much usage.

For smaller companies and individual developers this can be a lot to handle. This ends up distracting from the more important job that we have; building and maintaining the actual application. At larger organizations this is handled by the infrastructure team and usually it is not the responsibility of the individual developer. However, the processes necessary to support this can end up slowing down development times. As you cannot just go ahead and build your application without working with the infrastructure team to help you get up and running. As developers we’ve been looking for a solution to these problems and this is where serverless comes in. 

### Serverless Computing

Serverless computing (or serverless for short), is an execution model where the cloud provider (AWS, Azure, or Google Cloud) is responsible for executing a piece of code by dynamically allocating the resources. And only charging for the amount of resources used to run the code. The code is typically run inside stateless containers that can be triggered by a variety of events including http requests, database events, queuing services, monitoring alerts, ﬁle uploads, scheduled events (cron jobs), etc. The code that is sent to the cloud provider for execution is usually in the form of a function. Hence serverless is sometimes referred to as “Functions as a Service” or “FaaS” . Following are the FaaS offerings of the major cloud providers:

* AWS: AWS Lambda (https://aws.amazon.com/lambda/)
* Microsoft Azure: Azure Functions (https://azure.microsoft.com/en-us/services/functions/)
* Google Cloud: Cloud Functions (https://cloud.google.com/functions/)

While serverless abstracts the underlying infrastructure away from the developer, servers are still involved in executing our functions.
Since your code is going to be executed as individual functions, there are a couple of things that we need to be aware of. 

### Microservices

The biggest change that we are faced with while transitioning to a serverless world is that our application needs to be architectured in the form of functions. You might be used to deploying your application as a single Rails or Express monolith app. But in the serverless world you are typically required to adopt a more microservice based architecture. You can get around this by running your entire application inside a single function as a monolith and handling the routing yourself. But this isn’t recommended since it is better to reduce the size of your functions. We’ll talk about this below. 

### Stateless Functions

Your functions are typically run inside secure (almost) stateless containers. This means that you won’t be able to run code in your application server that executes long after an event has completed or uses a prior execution context to serve a request. You have to effectively assume that your function is invoked anew every single time.

### Cold Starts

Since your functions are run inside a container that is brought up on demand to respond to an event, there is some latency associated with it. This is referred to as a Cold Start . Your container might be kept around for a little while after your function has completed execution. If another event is triggered during this time it responds far more quickly and this is typically known as a Warm Start .
The duration of cold starts depends on the implementation of the speciﬁc cloud provider. On AWS Lambda it can range from anywhere between a few hundred milliseconds to a few seconds. It can depend on the runtime (or language) used, the size of the function (as a package), and of course the cloud provider in question. Cold starts have drastically improved over the years as cloud providers have gotten much better at optimizing for lower latency times.
Aside from optimizing your functions, you can use simple tricks like a separate scheduled function to invoke your function every few minutes to keep it warm. Serverless Framework (https://serverless.com) which we are going to be using in this tutorial has a few plugins to help keep your functions warm (https://github.com/FidelLimited/serverless-plugin-warmup).
Now that we have a good idea of serverless computing, let’s take a deeper look at what is a Lambda function and how your code is going to be executed.

## What is AWS Lambda?

AWS Lambda (https://aws.amazon.com/lambda/) (or Lambda for short) is a serverless computing service provided by AWS. In this chapter we are going to be using Lambda to build our serverless application. And while we don’t need to deal with the internals of how Lambda works, it’s important to have a general idea of how your functions will be executed.
 
### Lambda Specs

Let’s start by quickly looking at the technical speciﬁcations of AWS Lambda. Lambda supports the following runtimes.

* Node.js: v8.10 and v6.10 
* Java 8
* Python: 3.6 and 2.7
* .NET Core: 1.0.1 and 2.0
* Go 1.x

Each function runs inside a container with a 64-bit Amazon Linux AMI. And the execution environment has:
* Memory: 128MB - 3008MB
* Ephemeral disk space: 512MB
* Max execution duration: 300 seconds
* Compressed package size: 50MB
* Uncompressed package size: 250MB

You might notice that CPU is not mentioned as a part of the container speciﬁcation. This is because you cannot control the CPU directly. As you increase the memory, the CPU is increased as well.
The ephemeral disk space is available in the form of the /tmp directory. You can only use this space for temporary storage since subsequent invocations will not have access to this. We’ll talk a bit more on the stateless nature of the Lambda functions below.
The execution duration means that your Lambda function can run for a maximum of 300 seconds or 5 minutes. This means that Lambda isn’t meant for long running processes.
The package size refers to all your code necessary to run your function. This includes any dependencies ( node_modules/ directory in case of Node.js) that your function might import. There is a limit of 250MB on the uncompressed package and a 50MB limit once it has been compressed. We’ll take a look at the packaging process below. 

### Lambda Function

Finally here is what a Lambda function (a Node.js version) looks like.
<img src="/images/Lambda.PNG">
```
Here myHandler is the name of our Lambda function. The event object contains all the information about the event that triggered this Lambda. In the case of a HTTP request it’ll be information about the speciﬁc HTTP request. The context object contains info about the runtime our Lambda function is executing in. After we do all the work inside our Lambda function, we simply call the callback function with the results (or the error) and AWS will respond to the HTTP request with it. 
```

### Execution Model

The container (and the resources used by it) that runs our function is managed completely by AWS. It is brought up when an event takes place and is turned off if it is not being used. If additional requests are made while the original event is being served, a new container is brought up to serve a request. This means that if we are undergoing a usage spike, the cloud provider simply creates multiple instances of the container with our function to serve those requests.

This has some interesting implications. Firstly, our functions are effectively stateless. Secondly, each request (or event) is served by a single instance of a Lambda function. This means that you are not going to be handling concurrent requests in your code. AWS brings up a container whenever there is a new request. It does make some optimizations here. It will hang on to the container for a few minutes (5 - 15mins depending on the load) so it can respond to subsequent requests without a cold start. 

### Stateless Functions

The above execution model makes Lambda functions effectively stateless. This means that every time your Lambda function is triggered by an event it is invoked in a completely new environment. You don’t have access to the execution context of the previous event.
However, due to the optimization noted above, the actual Lambda function is invoked only once per container instantiation. Recall that our functions are run inside containers. So when a function is ﬁrst invoked, all the code in our handler function gets executed and the handler function gets invoked. If the container is still available for subsequent requests, your function will get invoked and not the code around it.
For example, the createNewDbConnection method below is called once per container instantiation and not every time the Lambda function is invoked. The myHandler function on the other hand is called on every invocation.
```
var dbConnection = createNewDbConnection();
exports.myHandler = function(event, context, callback) 
 {  
	var result = dbConnection.makeQuery();  
	callback(null, result);
 };
```
This caching effect of containers also applies to the /tmp directory that we talked about above. It is available as long as the container is being cached.
Now you can guess that this isn’t a very reliable way to make our Lambda functions stateful. This is because we just don’t control the underlying process by which Lambda is invoked or it’s containers are cached.

### Pricing

Finally, Lambda functions are billed only for the time it takes to execute your function. And it is calculated from the time it begins executing till when it returns or terminates. It is rounded up to the nearest 100ms.
Note that while AWS might keep the container with your Lambda function around after it has completed; you are not going to be charged for this.
Lambda comes with a very generous free tier and it is unlikely that you will go over this while working on this guide.
The Lambda free tier includes 1M free requests per month and 400,000 GB-seconds of compute time per month. Past this, it costs $0.20 per 1 million requests and $0.00001667 for every GB-seconds. The GB-seconds is based on the memory consumption of the Lambda function. For further details check out the Lambda pricing page (https://aws.amazon.com/lambda/pricing/).
In our experience, Lambda is usually the least expensive part of our infrastructure costs.

Next, let’s take a deeper look into the advantages of serverless.

## Why Create Serverless Apps?

It is important to address why it is worth learning how to create serverless apps. There are a couple of reasons why serverless apps are favored over traditional server hosted apps.

1. Low maintenance 
2. Low cost 
3. Easy to scale

The biggest beneﬁt by far is that you only need to worry about your code and nothing else. And the low maintenance is a result of not having any servers to manage. You don’t need to actively ensure that your server is running properly or that you have the right security updates on it. You deal with your own application code and nothing else.
The main reason it’s cheaper to run serverless applications is that you are effectively only paying per request. So when your application is not being used, you are not being charged for it. 

# Create an AWS Account

Let’s ﬁrst get started by creating an AWS (Amazon Web Services) account. Of course you can skip this if you already have one. Head over to the AWS homepage (https://aws.amazon.com) and hit the Create a Free Account and follow the steps to create your account.


## Create an IAM User

Amazon IAM (Identity and Access Management) enables you to manage users and user permissions in AWS. You can create one or more IAM users in your AWS account. You might create an IAM user for someone who needs access to your AWS console, or when you have a new application that needs to make API calls to AWS. This is to add an extra layer of security to your AWS account.
In this chapter, we are going to create a new IAM user for a couple of the AWS related tools we are going to be using later. 

### Create User

* First, log in to your AWS Console (https://console.aws.amazon.com) and select IAM from the list of services.
* Select Users.
* Select Add User.

