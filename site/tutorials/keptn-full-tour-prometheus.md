summary: Take a full tour on Keptn with Prometheus
id: keptn-full-tour-prometheus
categories: Prometheus,aks,eks,gke,openshift,pks,minikube
tags: keptn
status: Published 
authors: Jürgen Etzlstorfer
Feedback Link: https://keptn.sh


# Keptn Full Tour on Prometheus

## Welcome
Duration: 2:00 

In this tutorial you'll get a full tour through Keptn. Before we get started you'll get to know what you will learn while you walk yourself through this tutorial.

### What you'll learn
- How to create a sample project
- How to onboard a first microservice
- How to deploy your first microservice with blue/green deployments
- How to setup quality gates 
- How to prevent bad builds of your microservice to reach production
- How to automatically roll back bad builds of your microservices
- How to integrate other tools like Slack, MS Team, etc in your Keptn integration

You'll find a time estimate until the end of this tutorial in the right top corner of your screen - this should give you guidance how much time is needed for each step.

## Prerequisite
Duration: 10:00

Before you can get started, please make sure to have Keptn installed on your Kubernetes cluster.

If not, please follow one of these tutorials to install Keptn on your favourite Kubernetes distribution.

Negative
: Do not proceed until you have created your Kubernetes cluster and installed Keptn on it.

TODO INSERT TUTORIALS

<!-- include other files -->

{{ snippets/manage/createProject.md }}

{{ snippets/manage/onboardService.md }}

{{ snippets/monitoring/setupPrometheus.md }}

{{ snippets/monitoring/install-sliprovider-prometheus.md }}

{{ snippets/quality-gates/setupQualityGate.md }}

{{ snippets/self-healing/upscalePrometheus.md }}

{{ snippets/integrations/gettingStarted.md }}

## Finish
Duration: 1:00

Thanks for taking a full tour through Keptn!
Although Keptn has even more to offer that should have given you a good overview what you can do with Keptn.

### What we've covered

- We have created a sample project with the Keptn CLI and set up a multi-stage delivery pipeline with the `shipyard` file
- We have onboarded our first microservice
- We used a blue/green deployment to deploy the service 
- We have set up Prometheus to monitor our applications
- We have set up quality gates based on service level objectives
- We have tested our quality gates by deploying a bad build to our cluster and verified that Keptn quality gates stopped them.
- We have set up self-healing to automatically scale our application 
- We have learned how to extend our Keptn installation with other tools

