# TRAIN-TRAVELING-APP

Our app is targeting people who commute by train, that wants to get in contact with other people, who are on the same train as them. We are limiting the app to only work in Denmark, as we wanted this to be our focus area. From our classes, we heard that there are approximately as many Android users as iOS users in Denmark, and for this reason we decided to develop the app as a cross platform app, to reduce the costs and time of developing two native solutions.
The core functionality of the app is going to be the ability to find other people on the route the user has searched for, and then being able to send an invitation to go on a date with the person, the other person will have to do the same thing, for the date to be confirmed. To make it easier for people to find each other on the train, when the date has been confirmed, we had the idea to add chat functionality to the app. We would need a place to keep all this information, which should be available for all users, because of this, we would need a backend database, so the app will have something to pull and send data to.
In general, it is not a good practice to make direct connections between a mobile app and a remote database, because of performance and security reasons. That is why, we decided to make an extra layer, a Web API, between our app and database. This will make the app more lightweight and scalable.

We wanted most of the functionality of the program to be on the backend, so the solution was easier to build. This gives us the flexibility to add any type of client, for example a website, if it was needed later to reach more customers. If we found out during the process, that another language was better to build the API in, it would have been easy to switch to the other language as well, or move to another database without influencing the app.
We decided that the best way to build this app, would be to use an API to make all the calls to the database, and not just sending raw SQL queries from the phone. We also figured out that by having most of the functionality on the API, that it would minimize the use of the battery on the phone, which was something that was important for us.
The API is built using C# and it’s using JSON as the format it sends and receives in. The API is hosted on an external server.
We found out early in the process that we would need to run the API on an external server, as you couldn’t communicate with the API when it was on a local machine, using a real device. We also found this to be a good idea, as it was how the release version should run.
The use of API’s was not a new topic for the group as we had some experience from last semester where we learned, in a workshop, to work with restful API’s. We used some tutorials from internet[Ref 2] to get the idea how to build a Web API to communicate with the database in .Net framework. Beside that creating and using a Web API is very similar to a WCF service, which we learned and got experience with last semester.

A full report of the project can be found in the pdf attached to this repository where a more in-depth look into the sections of the project is presented.

Also a list with the links of all the repositories where the app has been developed can be found in "Repository links.txt.
