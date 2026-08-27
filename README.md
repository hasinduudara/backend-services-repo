# ECA Backend Services

## Student Information
* **Student Name:** M.Hasindu Udara
* **Student Number:** 241722041
* **Slack Handle:** hasiduudara
* **GCP Project ID:** hasinduudaraportfolio

## Project Description
This repository is the parent super-repository containing the core business microservices for the e-commerce platform. It includes the User Service, Product Service, and Order Service as Git submodules. The system demonstrates polyglot persistence by utilizing both relational and non-relational databases in a cloud-native architecture.

## Technology Stack
* Java 25
* Spring Boot & Spring Data
* MySQL (Google Cloud SQL)
* MongoDB (Google Cloud Firestore in Native Mode)
* Google Cloud Storage (Buckets)
* Google Cloud Platform (MIGs, Auto Scaling, Health Checks)

## Setup / Getting Started Instructions
1. Clone this repository recursively to fetch all service submodules: 
   `git clone --recurse-submodules https://github.com/hasinduudara/backend-services-repo.git`
2. Configure database connections:
   * Place the `firestore-key.json` in the Order Service directory.
   * Ensure Cloud SQL credentials are correctly set in the configuration server.
3. Build the microservices using Maven: `mvn clean install`
4. Deploy to Google Cloud Platform using PM2 for process management and automatic restarts.
