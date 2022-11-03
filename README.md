# Udagram [![CircleCI](https://dl.circleci.com/status-badge/img/gh/seifalaa/udagram/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/seifalaa/udagram/tree/master)

A project that demonstrate how to deploy a fullstack app to AWS.
<br>
You can check the app from this [link](http://udgram-frontend.s3-website-us-east-1.amazonaws.com)

this project includes:

1. Creating an AWS RDS instance and connect a Nodejs App to it.  
2. Deploying a backend API to AWS using Elastic Beanstalk.
3. Deploying a frontend application to AWS using S3 Static website hosting.
4. Creating a CI/CD pipeline using CircleCi and Github.

## Application Architecture

![application_architecture](./screenshots/flow.png)

### Description

* The user opens the browser and visits the web app
* The server aka (AWS S3 Static Web Hosting) receives the request and responds with the requested page
* The web app send a HTTP request to the backend server hosted on (AWS Elastic Beanstalk) to get the data.
* The backend server receives the request and fetches the data from the database (AWS RDS) and sends it back to the frontend.
* The data gets displayed.

## CI/CD Pipeline

![application_architecture](./screenshots/pipeline.png)

### Description

* A developer commits his code changes to the Github Repo
* A CI/CD trigger gets triggered.
* The pipeline gets the new changes and pushes them to AWS

## Screenshots

You can find screenshots with the infrastructure and the CI/CD pipeline in the `screenshots` folder

## Getting started

1. [Backend Doc](./udagram-api/README.md)
2. [Frontend Doc](./udagram-frontend/README.md)

## Built With

<div>
  <p>
    <img src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white" alt="typescript" />
    <img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="postgresql" />
    <img src="https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white" alt="angular" />
    <img src="https://img.shields.io/badge/Inonic-3880FF?style=for-the-badge&logo=ionic&logoColor=white" alt="ionic" />
    <img src="https://img.shields.io/badge/prettier-1A2C34?style=for-the-badge&logo=prettier&logoColor=F7BA3E" alt="prettier" />
    <img src="https://img.shields.io/badge/eslint-3A33D1?style=for-the-badge&logo=eslint&logoColor=white" alt="eslint" />
    <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="node" />
    <img src="https://img.shields.io/badge/circleci-343434?style=for-the-badge&logo=circleci&logoColor=white" alt="circleci" />
    <img src="https://img.shields.io/badge/Amazon_AWS-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white" alt="aws" />
</p>
</div>
