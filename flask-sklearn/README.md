# Overview

This project is to deploy a flask based ML webapp in the azure webapp serviceand toconduct load test on it using locust. The webapp deployment is automated using azure pipeline.

## Project Plan
Project Plan

*Link to Trello board https://trello.com/invite/b/6E5p4ZVN/8f8b2599781f03ae2146c9c5ee55a52f/project6


*Link to spreadsheet project plan  https://docs.google.com/spreadsheets/d/1-eWv2khCIhTI6tuPomEeAxwZsJ4DZlzss0qTuMlwClc/edit?usp=sharing

## Instructions


* Architectural Diagram (Shows how key parts of the system work)>
![architecture](https://user-images.githubusercontent.com/108992155/192412566-32f24aa5-55db-4a25-9b5e-18af5d30a1ba.PNG)
<p>
1.Clone the Project files to VisualStudio/ Azure cloud CLI.<br>
2.Create virtual environment.<br>
3.Go to directory where files are kept.<br>
4.Run make all.<br>
5.Deploy the webapp using the c<br>ommand 'az webapp up' and name, runtime=python:3.7.<br>
6.Check weather deployment occured without error by checking the GUI using URL and running './make_predict_azure.sh' command in CLI.<br>
7.Run the load test using locust.<br>
8.Create a service connection in azure devops organisation.<br>
9.Create an agent pool and an add agent (if you are using a shared azure service).<br>
10.Create a pipeline in the project.<br>
11.Select github repository.<br>
12.Select existing YAML file.<br>
13.Make changes which are necessary in YAML (like agent pool name, service connection ...).<br>
14.Add any additional steps you want to add in the build or deployment stage.<br>
15.Save the pipeline.<br>
16.Run the Pipeline.<br>
</p>

* Project running on Azure App Service<br>
###Azure app service
![2022-09-25 (1)](https://user-images.githubusercontent.com/108992155/192120328-69260032-849c-41a9-ac45-f3de344ff29f.png)

* Project cloned into Azure Cloud Shell
![ss of github clonning](https://user-images.githubusercontent.com/108992155/192417481-8b161de4-43d4-4dae-860f-dbd5b584f74b.PNG)



* Passing tests that are displayed after running the `make all` command from the `Makefile`

![ss of make file passing](https://user-images.githubusercontent.com/108992155/192417515-5f12c1ab-2ff1-4f53-a035-f483f342cff8.PNG)

* Output of a test run

* Successful deploy of the project in Azure Pipelines. <br>
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
<br>
###Successful prediction by webapp<br>
![2022-09-25 (3)](https://user-images.githubusercontent.com/108992155/192120485-0c8d48ce-f4b0-45fe-8aec-8dbcfa288568.png)
<br>
<br>

* Output of streamed log files from deployed application<br>
![2022-09-25](https://user-images.githubusercontent.com/108992155/192417990-1c8441cd-632e-4c6c-adf3-2311a235a90b.png)
<br>
<br>

###Conducting load test on the deployed app<br>
![locust run ss](https://user-images.githubusercontent.com/108992155/192152707-0b8d8392-9385-4efb-bb6a-573fe45c2504.JPG)
![locust run ss2](https://user-images.githubusercontent.com/108992155/192152713-6ecc16b3-ced0-4a39-a31d-bdf110b159ac.JPG)
<br>
<br>
## Enhancements

this project can be improved by adding testplans, creating the webapp  more interactive and settingup custom alert.

## Demo 

<TODO: Add link Screencast on YouTube>



###successful run in pipeline
![2022-09-25 (4)](https://user-images.githubusercontent.com/108992155/192120545-fd6195eb-b9c7-45fc-98cb-bcbcfd26dcf1.png)


