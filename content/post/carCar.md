---
title: "Car Car"
date: "2022-07-01"
author: "Yehsun"
cover: "img/car/main.png"
---

> A CRUD app that allows Car dealers to manage inventory, technicians to track record of services and customers to create a service request. Enhanced backend Restful API endpoints to optimize data delivery and React hooks to manage stateful components.

 ### Tech stack
  Django REST framework, Python, JavaScript, PostgreSQL, Docker, React, RESTful API's

### GHI Design
The three services intersect at a point represented by an Automobile. Each microservice interprets and focuses on it a different way. 


![list](/img/car/designMap.png)

Each microservice has its own directory to store files for their respective components. Within each directory, there is also a file designated to store functions related to fetching, to keep files more task focused. This organization is also reflected through the dropdown options in the navbar on the browser.

* Within the `Auto Services microservice`, an Automobile is represented in a way that focuses on whether or not it had at one point been sold by this dealership, if so, the automobile is considered a VIP.
* In the `Auto Sales microservice`, it focuses on whether or not the automobile is still available in inventory to determine if it can sell the particular automobile.
* In the `Inventory microservice`, although it also cares if the automobile exists in it, it's focus is more on the description properties of the automobile, like its color, year, and picture, which are not priorities of the other two microservices.

### Vehicle models List
![list](/img/car/inventory.png)
* This page lists all the vehicle models.

### Create a service appointment
![list](/img/car/appointmentForm.png)
* SeviceAppointmentForm
  - Create a form that allows a service concierge to enter the VIN of the vehicle, the name of the person to whom the vehicle belongs, the date and time of the appointment,the assigned technician, a reason for the service appointment.
  -  When the form is submitted, the service appointment should be saved in the application
  -  A  link in the navbar to get to the Enter a service appointment form.


![list](/img/car/appointmentList.png)
* List of appointments 
    - Get the list of service appointment VIN, customer name, date and time of the appointment, the assigned technician's name,the reason for the service.
    - Cancel/finish button
    - VIP treatment if the car was in inventory list

![list](/img/car/searchBar.png)
* ServiceHistory
  - Create a page that has an input that allows someone to type in the VIN.
  - On form submission,fetch all of the service appointments for an automobile with the VIN in the input.
  - Show that list of service appointments to include
  - Create a link in the navbar to get to the page that shows the service history for a specific VIN.

> In case you wonder how I created these projects in detail, please visit my `gitlab repository` [ projectCar](https://gitlab.com/yehsunkang/projectcar)