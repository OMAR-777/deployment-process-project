[![<ORG_NAME>](https://circleci.com/gh/OMAR-777/deployment-process-project.svg?style=svg)](https://app.circleci.com/pipelines/github/OMAR-777/deployment-process-project)

# Deployment Process Project: Udagram

* [Overview](#overview)
* [Udagram](#udagram)
* [AWS Services](#aws-services)
* [Testing](#testing)
* [Built With](#built-with)
* [License](#license)
* [Infrastructure Description](./Docs/Infrastructure_description.md)
* [Pipeline Description](./Docs/Pipeline_description.md)
* [Application dependencies](./Docs/Application_dependencies.md)



## Overview

This is the final project of Udacity's Full Stack Javascript Developer course which covers the topics of the deployment process.

In this project we learnt how to take a newly developed Full-Stack application then use AWS services to deploy the application manually the first time, then setup a pipeline in CircleCi and connect it to this repositry to automate the deployment process when code is pushed on the the main branch.

The project will also include writing documentation and runbooks covering the operations of the deployment process. Those runbooks will serve as a way to communicate with future developers and anybody involved in diagnosing outages of the Full-Stack application.


## Udagram

The Project used in the deployment process is provided by Udacity, it's called **Udagram** (name is inspired from Instagram) - an Image Filtering application, allows users to register and log into a web client, post photos to the feed, and process photos using an image filtering service. It has two components:

    Frontend - Angular web application built with Ionic framework
    Backend RESTful API - Node-Typescript application



## Udagram Preview
### Link to the website: 
http://udagram-frontend-bucket-743.s3-website-us-east-1.amazonaws.com/

![Alt text](Docs/Screenshots/Udagram-Preview.png?raw=true "Title")


---
## AWS Services

the necessary AWS services configured for running the application:

1. RDS database running Postgres.
1. S3 bucket for hosting the uploaded files. 
1. S3 bucket for hosting the frontend (Angular project).
1. EB (ElasticBeansTalk) for hosting the backend API.

## Testing

This project contains two different test suite: unit tests and End-To-End tests(e2e). Follow these steps to run the tests.

1. `cd starter/udagram-frontend`
1. `npm run test`
1. `npm run e2e`

There are no Unit test on the back-end

### Unit Tests:

Unit tests are using the Jasmine Framework.

### End to End Tests:

The e2e tests are using Protractor and Jasmine.

## Built With

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework

## License

[License](LICENSE.txt)
