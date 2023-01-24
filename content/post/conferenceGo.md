---
title: "Conference Go"
date: "2022-06-01"
author: "Yehsun"
cover: "img/conference/main.png"
---
![list](/img/conference/mainContinued.png)


 > A conference & presentation aggregator web app for attendees and presenters. Developed full-stack, single-page web app with Restful API. Combined custom and third party API calls.Implemented poller/ rabbitMQ for communication between microservices.

 ### Tech stack
  Django REST framework, React, Python, JavaScript, PostgreSQL, Docker, RabbitMQ, RabbitMQ, RESTful API's

### External API Integrations
* [Pexels](https://python-gitlab.readthedocs.io/en/stable/api-usage.html)
   - Provides a access token for full list of available public resources.
   - The gitlab.Gitlab class provides managers to access the GitLab resources. Each manager provides a set of methods to act on the resources. The available methods depend on the resource type.
* [Weather ](https://docs.gitlab.com/ee/api/projects.html)
    - Get a list of the public project can be accessed without any authentication.
    - Retrieve data from the each project for the attribute: projectId, project name, group name, group id, team members, language usage, commits distributions,started date. 

### Conference Form
![list](/img/conference/createConference.png)
  - A form that can be completed by anyone who would like to create a new conference.
  - The newly created conference dynamically updates on the main page.

### Attend Conference
![list](/img/conference/attend.png)
  - A form that can be completed where the user chooses the conference they would like to attend and inputs their information. 
  - The success message appears when a user successfully signs up for a conference.

![list](/img/conference/success.png)


> In case you wonder how I created these projects in detail, please visit my `gitlab repository` [ Conference Go II](https://gitlab.com/yehsunkang/conference-go-ii)