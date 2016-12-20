#Very Rough Draft

Project Title
Write a Chef Cookbook
Description
Defining infrastructure as code is a change that can help in various parts of the software lifecycle. It will make deployment easier and safer, it will make provisioning and launching test environments simpler, and it will give a common language and place for developers and operations to talk about infrastructure. It's also a powerful event you can start, a first step in the ELSA model.

Your task in this project has two parts:
Written
There is an application in active development that has a set of dependencies that are hard to install and take a long time. It's hard to onboard new team members, time consuming to set up a test server with the latest version for QA team, and often there are problems when deploying to production.
Using ELSA change management model as a framework, describe an approach you would take to solve this problem. Write a couple of sentences for each step in your approach that would correspond to Event, Language, Structure and Agency.
Technical
Write cookbooks that define a working SonarQube server, and a separate database server for it, according to the spec below. You can use existing cookbooks from https://supermarket.chef.io. If you don't include existing cookbooks directly, but just use them as base for your work, you have to link to the source repository in the accompanying README file and give credit to the author(s).
You can prepare for the project  [here](https://learn.chef.io/tutorials/). Take the following groups of  tutorials: “Get started with Chef” and “Develop and test your infrastructure code locally.”
By the end of the tutorial, you will have a working web application on an Apache web server with a MySQL database. For this project, you’ll build something similar using a different stack, so it may be helpful to look at and fully understand the project components before starting the tutorial.
Project components:
Cookbook for a Database server - Postgres stable (as of today - 9.5.2 http://www.postgresql.org/support/versioning/)
Cookbook for a SonarQube Server LTS version (as of today - 4.5.7 - http://www.sonarqube.org/downloads/), using Java JDK version 8
Cookbook for additional information in Message of the Day (MOTD) showing SonarQube and Postgres versions respectively
A README file describing contents and the usage of the cookbooks
