---
title: "Project Spark"
date: "2022-09-01"
author: "Yehsun"
cover: "img/spark/main.png"

---


 > A central hub to view, collaborate, and comment on all cohort's projects from the 19-week Hack Reactor Software Engineering Immersive program. Students of the May cohort and all future cohorts that could benefit from having a website dedicated to displaying sample projects, as well as all Hack Reactor staff and alumni.

 ### Tech stack
  Django REST framework, React, Python, JavaScript, PostgreSQL, Docker,  SimpleJWT auth

### API design
For `API endpoints` for projects in-depth, look at [API design](https://gitlab.com/salmons1/salmon-project/-/blob/main/docs/apis.md)

### External API Integrations
* [python-gitlab](https://python-gitlab.readthedocs.io/en/stable/api-usage.html)
   - Provides a access token for full list of available public resources.
   - The gitlab.Gitlab class provides managers to access the GitLab resources. Each manager provides a set of methods to act on the resources. The available methods depend on the resource type.
* [GitLab Docs](https://docs.gitlab.com/ee/api/projects.html): 
    - Get a list of the public project can be accessed without any authentication.
    - Retrieve data from the each project for the attribute: projectId, project name, group name, group id, team members, language usage, commits distributions,started date. 


![list](/img/spark/list.png)

### Functionality

* Anyone can view all final projects from the 19-week Hack Reactor Software Engineering Immersive program
* Only users who signup and login may leave a comment
* Search function to find projects based on project name, owners, month and year, etc.
* 
  
#### Data models_User & Project
| project_id | username | avatar_id | bio |
|-|-|-|-|
| string | string | int  | string|



![detail](/img/spark/detail.png)


### Project detail page features

* preview of their website if deployed
* README file
* all GitLab group and project information
* miniaturized view of wireframe files
* bar chart of languages used
* pie chart breaking down the number of commits per member
* 

#### Data models_Comment
| text | timestamp | user | project |
|-|-|-|-|
| string | datetime | foreign key | foreign key |


![profile](/img/spark/profile.png)
### Profile page

* Changing avatar and bio

> In case you wonder how I created these projects in detail, please visit my `gitlab repository` [ projectSpark](https://gitlab.com/yehsunkang/projects-spark)