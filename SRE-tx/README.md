# SRE Challenge

This challenge is divided in 3 tasks without right or wrong solutions. The only strong requirements are that it must run without errors after proper configuration and must be properly documented. 

## Pre-requisites
- any technology stack maybe used, but everything (including infrastructure) **must** be delivered **"as code"**
- **document** your code and explain your rationale and decisions. Even the most wise ones needs to read a scroll every once in a while...
- it must be easy to install and use
- dependencies should be self-contained (e.g. requirements.txt, package.json, etc)
- performance is not optional in software engineering. Your challenge should run in minutes, not hours


## Task 1
### Objective

Your objective is to build an app with the following API:

- endpoint that receives a path from Wikipedia, [fetches](https://en.wikipedia.org/wiki/Special:ApiSandbox#action=parse&format=json&page=Word_list&prop=wikitext) its content and returns its [word list](https://en.wikipedia.org/wiki/Word_list)
- may use any technology stack but must run on Linux
- must be containerized



## Task 2
### Objective

Your objective is to build the following infrastructure:

- Kubernetes cluster with two (2) worker nodes
- must expand worker pool automatically up to four (4) nodes
- custom network for pods, where pods can be accessed by VMs and/or services
- enable and setup the ingress service
- deploy the app from task 1 or, if it was not built, any webapp
- make sure the app is accessible through its ingress



## Task 3
### Objective

Your objective is to build a CI/CD pipeline with:

- CI that tests the app from task 1, if it was built, or any other app
- CI that tests the code from task 2 if it was built, or any other IaC
- CD that deploys the IaC from the CI stage
- CD that deploys the webapp from task 1  if it was built, or any other code
- pipeline that runs when there are code changes


## Extra points

- all tasks are built and dependent on each other
- monitoring is built and setup, both on the app and the IaC
- unit and/or integration tests on task 1