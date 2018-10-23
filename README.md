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
</details>




# Introduction

## What is Serverless?
