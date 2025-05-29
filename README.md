3T WebApp & Database Helm Charts
=================================

This repository contains Helm charts for deploying the 3T web application and its associated database on Kubernetes clusters.

Repository Structure
--------------------
- db/: Contains Helm chart configurations for deploying the database component.
- Jenkinsfile: Defines the CI/CD pipeline for automating the deployment process using Jenkins.

Prerequisites
-------------
- A Kubernetes cluster
- Helm installed on your local machine
- Jenkins set up for CI/CD (if utilizing the provided Jenkinsfile)

Installation
------------

1. Clone the repository:

   git clone https://github.com/AnonyIIMessiah/3t-webapp-database-helm.git
   cd 3t-webapp-database-helm

2. Deploy the database using Helm:

   helm install db ./db

   Note: Ensure that the db chart is properly configured before deployment.

3. Set up the CI/CD pipeline:

   Integrate the provided Jenkinsfile into your Jenkins setup to automate the deployment process.

Configuration
-------------
Customize the Helm charts by modifying the values.yaml files within each chart directory.
This allows you to set parameters such as image versions, resource allocations, and environment-specific settings.

License
-------
This project is licensed under the MIT License.
