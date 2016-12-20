# Migrate an Application Server to the Cloud

This project has two parts: analytical and technical. 

* For the analytical portion, you will examine a scenario where certain services are to be migrated to the cloud, and make a recommendation about which cloud provider to use. 
* For the technical portion, you will write a Packer config file to create a virtual machine image for a server. We will provide the server specifications.

Both parts of the project need to be successfully completed for the project to be considered complete. 

## Project Introduction

Our fictional companies are evaluating their cloud computing strategies. Each company is facing a different situation. In this project, you will accomplish two goals:

* First, you will analyze the situation in any one of those companies, and make a recommendation about the cloud provider and platform to adopt.
* Second, you will demonstrate your cloud computing skills by writing a Packer configuration for a virtual machine on AWS.

Both parts of the project need to be successfully completed for the project to be considered complete.

For the analytical portion of this project you are encouraged, but not required, to use the same company that you picked for your P0 submission. As with that project, the scenarios may need to be augmented with details from your own experience, research, and imagination.

## Analytical Section Description and Requirements

These are the requirements for the analytical section of the project:

* Pick any one of the three fictional scenarios described later in this lesson. You are encouraged, but not required, to choose the same company that you did for P0.
* Pick any 2 public cloud providers from among Amazon Web Services, Google Cloud Platform, or Microsoft Azure, and analyze how good a fit each is for your needs. Your analysis should take the following into account:
  * Does the organization already use services from these cloud platforms or related companies? For instance, MS SQL server would count for MS Azure, and Google Apps would count for Google Cloud Platform.
  * Are any of the employees familiar with one or the other of the cloud platforms? If so, how much weight should be given to this familiarity? Is such preexistent expertise more or less important than the ease of providing of additional services?
  * What types of VM would best serve the application needs on each of the cloud platforms? Pick the most appropriate VM type, or types (eg for web server and DB server).
  * Are there any specific regional requirements?
  * Are there some company goals that make one of the solutions more attractive?
  * Assume normal usage 300 days a year; high usage 53 days a year and a 10x increase in traffic and load in the high usage period.
* Given the above profiles, calculate the cost of running the application on each of the cloud platforms for a year, using current prices. Add links to the pricing pages. Since prices change, also specify the date when you retrieved a given pricing page.
* Based on the comparative analysis, make a recommendation about which cloud platform to use. Which cloud service should the team pick for this particular application migration, and why?

### Scenario 1: Ungeneric

As more companies sign up to be Ungeneric customers, the company is facing the challenge that its own hardware servers can no longer handle the load. It is very difficult to add servers quickly for the needed capacity. Instead of managing a rapidly growing server farm, it seems sensible to move to some cloud platform. 

The existing codebase for the application is largely in Ruby and it uses MySQL for the database. Philosophically the team is more oriented toward open source tools (e.g., Linux over Windows) While the company currently has no cloud platform preference, but would prefer to move to one of industry leaders, assuming more features and better support. 

From a usage perspective, the product is not CPU or RAM intensive. One important consideration is that a multinational company wants Ungeneric's product to be available for employees in its China and Europe offices. 

### Scenario 2: Twisted Threads 

Twisted Threads currently uses a small cloud services provider that has not proved very robust. Uptime is fine during ordinary usage, but unreliable at peak times when inventory is rapidly cycled out, such as during the holidays or during a change of season. 

The service is proving expensive, particularly since the application requirements for a single server are quite small: 500MB of RAM, but at peak times CPU usage goes through the roof. The thinking among the team is that moving to a different, better known cloud platform, preferably one that has good autoscaling capabilities, would be advantageous.

The codebase is largely in C++. Prior to moving to the current cloud services provider, the company hosted its own servers using Windows.The inventory systems, POS infrastructure for brick-and-mortar stores, and back office systems are still Windows-based. The developers are comfortable in a Windows environment and lean toward Azure. However, the company founder feels that Amazon would be a good choice as there is also the possibility of hosting a storefront on Amazon Marketplace. 

This is a source of some tension as the developers feel they might lose their jobs if Twisted Threads no longer maintains its own online storefront but uses the services provided by Amazon. The founder has tried to reassure them that their jobs are safe. Her argument is that with a reliable infrastructure, developers can focus on new growth initiatives for the company rather than be in firefighting mode all the time.

### Scenario 3: ChalkFull

There is a push at ChalkFull to add a new feature: a way for teachers to build lesson plans quickly. The idea is that teachers can share lesson plans they have previously used on a website. Other teachers from across the country can view and comment on the lesson plans, and also revise them for their own use. In addition, ChalkFull will host supplementary materials in the form of images, videos, quizzes, links to external web resources, etc. that can be incorporated into the lesson plan. The expectation is that this feature will be available as an add-on to the existing product within the next quarter, and then marketed as a separate, stand-alone product within six months. 

Rather than add to its existing server farm, ChalkFull intends to use a cloud provider to host this new product. The analysis on what provider to use has just begun. ChalkFull's existing codebase is in Python (back end) and JavaScript (front end), and they intend to use MongoDB as a database. The chosen provider must handle these languages well. The expectation also is that usage will spike about three weeks before the start of each school term. During the school year, a smaller spike on weekends is expected as teachers prepare their lessons for the upcoming week.

## Technical Section Description and Requirements

After you have made your recommendation and are waiting for a final decision from management, you decide to make a VM configuration to run a SonarQube server. SonarQube is an open source platform to manage code quality, for example: checking for duplicated code, maintaining code standards; conducting unit tests, etc. The VM configuration could be used on any of the cloud platforms, so you don't have to wait to hear what management has decided.

Create a Packer configuration (that is, a Packer file and scripts to be run) for an image that would meet the requirements for installing a working SonarQube server. 

* The Packer configuration should create a VM that meets the [technical specifications](http://docs.sonarqube.org/display/SONAR/Requirements) that would allow SonarQube to be installed. That is, the created VM should have:
  * The requisite hardware provisioned.
  * An appropriate JRE (either Oracle JRE or OpenJDK). Use the latest supported version; if older versions are supported by SonarQube, you need not include them.
  * An appropriate SQL Server.
* Please note: **you do not have to install the SonarQube software itself**. All you need to do is write the Packer configuration for a host that meets the above requirements, so that it can eventually run the SonarQube software. 
* Cloud credentials should be provided as environment variables. They **should not** be included in the submitted Packer files!

Test your Packer configuration by building this VM on AWS, using the account you created during the lessons preceding this project.

## Project Assessment and Submission Details

### What should I submit?

Your submission will consist of two items:

* The document with your analysis and the recommendation based on that analysis. This document must be submitted in **Markdown format**. 
* The Packer configuration files for the server. 

### How will the project be reviewed? 

Your submission will be reviewed using [this rubric](https://review.udacity.com/#!/rubrics/179/view). Please go through the rubric carefully to ensure that you have addressed all the project requirements.

### What is the procedure to submit the project? 

When you are confident that your project meets all the requirements of the rubric, you can submit it at [the Project Reviews site](https://review.udacity.com/#!/rubrics/179/submit-file).

