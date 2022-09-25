# Overview

This project is to deploy a flask based ML webapp in the azure webapp serviceand toconduct load test on it using locust. The webapp deployment is automated using azure pipeline.

## Project Plan
Project Plan

*Link to Trello board https://trello.com/invite/b/6E5p4ZVN/8f8b2599781f03ae2146c9c5ee55a52f/project6


*Link to spreadsheet project plan  https://docs.google.com/spreadsheets/d/1-eWv2khCIhTI6tuPomEeAxwZsJ4DZlzss0qTuMlwClc/edit?usp=sharing

## Instructions

<TODO:  
* Architectural Diagram (Shows how key parts of the system work)>

<TODO:  Instructions for running the Python project.  How could a user with no context run this project without asking you for any help.  Include screenshots with explicit steps to create that work. Be sure to at least include the following screenshots:

* Project running on Azure App Service



###Azure app service
![2022-09-25 (1)](https://user-images.githubusercontent.com/108992155/192120328-69260032-849c-41a9-ac45-f3de344ff29f.png)

* Project cloned into Azure Cloud Shell

* Passing tests that are displayed after running the `make all` command from the `Makefile`

* Output of a test run

* Successful deploy of the project in Azure Pipelines.  [Note the official documentation should be referred to and double checked as you setup CI/CD](https://docs.microsoft.com/en-us/azure/devops/pipelines/ecosystems/python-webapp?view=azure-devops).
###Deploying webapp using azure pipeline into azure app service
![2022-09-25 (2)](https://user-images.githubusercontent.com/108992155/192120282-5246a7a0-37f4-4308-9627-3d8dde4b06be.png)

* Running Azure App Service from Azure Pipelines automatic deployment

* Successful prediction from deployed flask app in Azure Cloud Shell.  [Use this file as a template for the deployed prediction](https://github.com/udacity/nd082-Azure-Cloud-DevOps-Starter-Code/blob/master/C2-AgileDevelopmentwithAzure/project/starter_files/flask-sklearn/make_predict_azure_app.sh).
The output should look similar to this:

```bash
udacity@Azure:~$ ./make_predict_azure_app.sh
Port: 443
{"prediction":[20.35373177134412]}
```
###Successful prediction by webapp
![2022-09-25 (3)](https://user-images.githubusercontent.com/108992155/192120485-0c8d48ce-f4b0-45fe-8aec-8dbcfa288568.png)


* Output of streamed log files from deployed application


###Conducting load test on the deployed app
![locust run ss](https://user-images.githubusercontent.com/108992155/192152707-0b8d8392-9385-4efb-bb6a-573fe45c2504.JPG)
![locust run ss2](https://user-images.githubusercontent.com/108992155/192152713-6ecc16b3-ced0-4a39-a31d-bdf110b159ac.JPG)

> 
## Enhancements

<TODO: A short description of how to improve the project in the future>

## Demo 

<TODO: Add link Screencast on YouTube>


## Screenshots







###successful run in pipeline
![2022-09-25 (4)](https://user-images.githubusercontent.com/108992155/192120545-fd6195eb-b9c7-45fc-98cb-bcbcfd26dcf1.png)


