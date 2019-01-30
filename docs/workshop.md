# 1. Omnia Radix Workshop 1

Purpose

The purpose of the workshop is to give a general and hands-on introduction to Radix. We do this by "forking" and example application, get familiar with the application, establish a CI environment locally, move the application into Radix and then establish the full CI/CD DevOps cycle.

<!-- TOC -->

- [1. Omnia Radix Workshop 1](#1-omnia-radix-workshop-1)
    - [1.1. Part 1](#11-part-1)
        - [1.1.1. Pre-requisites](#111-pre-requisites)
        - [1.1.2. Getting started](#112-getting-started)
        - [1.1.3. Exploring the Echo app](#113-exploring-the-echo-app)
        - [1.1.4. Exploring the Echo app](#114-exploring-the-echo-app)
        - [1.1.5. Preparing for Radix](#115-preparing-for-radix)
        - [1.1.6. Explore radixconfig.yaml](#116-explore-radixconfigyaml)
        - [1.1.7. Creating the application on Radix](#117-creating-the-application-on-radix)
        - [1.1.8. Using multiple branches - multiple environments](#118-using-multiple-branches---multiple-environments)
        - [1.1.9. Monitoring & Metrics](#119-monitoring--metrics)
    - [1.2. Part 2](#12-part-2)
        - [1.2.1. Next steps](#121-next-steps)
    - [1.3. Q&A](#13-qa)
    - [1.4. Where to get started & get help](#14-where-to-get-started--get-help)

<!-- /TOC -->
## 1.1. Part 1

### 1.1.1. Pre-requisites

- Added to proper AD Group ```fg_radix_platform_user```
- Verify access to Radix -- url --
- Account on github.com
- Git installed and working locally against github.com
- Docker running locally
- Local dev. environment (IDE++)
- Node js eco system installed and running ([Downnload Nodejs](https://nodejs.org/en/download/))
- Laptop that "works" on “Statoil Approved” WiFi. If not - know how to handle proxy fun for both Docker and local development environment

### 1.1.2. Getting started

1. Fork repository to your home on github. Consider choosing an alternative name.

### 1.1.3. Exploring the Echo app

1. Move into the [echo](./echo/README.md) folder and explore how to develop the Echo app using ```Node.js``` as well as Dockerizing the application.

### 1.1.4. Exploring the Echo app

1. Move into the [www](./www/README.md) folder and explore how to develop the WWW app using ```Node.js``` as well as Dockerizing the application. 

Remember that the Echo app needs to run somewhere to get proper response.

### 1.1.5. Preparing for Radix

* The Radix cluster we use for the workshop is available at https://web-radix-web-console-prod.playground.dev.radix.equinor.com/

Important to know:

1. The difference between ```platform user``` and ```application user```
2. Important terminology: ```application```, ```environments```,```components```, and ```pods```
3. ```raidxconfig.yaml``` - lives on the master branch and is your infrastrucure as code - drive your app in Radix.

### 1.1.6. Explore radixconfig.yaml

1. Reading the [docs](https://github.com/equinor/radix-operator/blob/master/docs/radixconfig.md)
2. Exploring the config file for the example app [./radixconfig.yaml](./radixconfig.yaml)

### 1.1.7. Creating the application on Radix

1. Update the name of ```your instance``` of the application in radixconfig.yaml
2. Follow the getting started guide or "just do it!"
3. Do a change to trigger the initial build. Examine web-hooks and reponse in Radix
4. Verify that the app work on the public end-point it has been given.

### 1.1.8. Using multiple branches - multiple environments

Radix support connecting a branch to a specific environment. Let's explore this.

1. Move to "new" branch (feature1)
2. Examine code - the new feature  (getting a new env variable from Radix)
3. Move back to master, update the radixconfig.yaml file, commit, push and explore what's happening in Radix.
4. Check-out feature1, do a change, commit, push and explore what's happening in Radix.


### 1.1.9. Monitoring & Metrics

- To Be Decided

## 1.2. Part 2

### 1.2.1. Next steps

* Move your own apps into Radix


## 1.3. Q&A

(Status as of January 2019)
* Storage - databases
* Authentication
* Logging

## 1.4. Where to get started & get help

* Slack (#omnia_radix, #omnia_radix_support)
* www.radix.equinor.com - https://console.radix.equinor.com/