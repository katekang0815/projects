---
title: "Project Spark"
date: "2023-01-18"
author: "Yehsun"
cover: "img/main.png"

---


A central hub to view, collaborate, and comment on all cohort's projects from the 19-week Hack Reactor Software Engineering Immersive program. Students of the May cohort and all future cohorts that could benefit from having a website dedicated to displaying sample projects, as well as all Hack Reactor staff and alumni.


<img src="img/list.png">

## CommentVO

| text | timestamp | user | project |
|-|-|-|-|
| string | datetime | foreign key | foreign key |

![logged in navbar](static/../../../static/img/list.png)

## Integrations

The application requires integrating data from each project's gitlab.

* [python-gitlab](https://python-gitlab.readthedocs.io/en/stable/api-usage.html)
   - Provides a access token for full list of available public resources.
   - The gitlab.Gitlab class provides managers to access the GitLab resources. Each manager provides a set of methods to act on the resources. The available methods depend on the resource type.
* [GitLab Docs](https://docs.gitlab.com/ee/api/projects.html): 
    - Get a list of the public project can be accessed without any authentication.
    - Retrieve data from the each project for the attribute: projectId, project name, group name, group id, team members, language usage, commits distributions,started date. 
