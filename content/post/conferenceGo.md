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
* [Pexels](https://www.pexels.com/api/documentation/#photos-search)
  API to get the URL of a picture of the city when create a new location instance

* [Geocoding API ](https://openweathermap.org/api/geocoding-api)
 Translating the city and state for the conference into latitude and longitude
* [Current weather data ](https://openweathermap.org/current)
  API to get the current weather for the latitude and longitude found in the Geocoding API

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