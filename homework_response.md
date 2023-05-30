Questions

1. What is responsible for defining the routes of the games resource?

<!-- The createRouter function within the create_router.js file is responsible. This file shows a template for all restful routes and actions.  -->

2. What do you notice about the folder structure? Whats the client responsible for? Whats the server responsible for?

<!-- 
Client:
The client is responsible for defining and holding all of the components and containers. 

Server:
The server holds the seed data as well as the router which defines the restful routes. It also contains the server.js file which creates the express server and tells it which port to listen to and what to return when it receives any request.

 -->

3. What are the the responsibilities of server.js?

<!-- It creates the express server and tells it which port to listen to and what to return when it receives any request. It also connects to the front end to the Mongo DB -->

4. What are the responsibilities of the gamesRouter?

<!-- The gamesRouter is a new router created and being passed the gamesCollection (after being pulled from the DB). 

It handles the restful routes using a copy of the router template, specifially for the games. -->

5. What process does the the client (front-end) use to communicate with the server?

<!-- 
The client uses the restful routes (post, put, delete and get) to communicate with the server and database. It sends a request for information to be returned, changed, deleted in the database and receives a response accordingly.
-->


6. What optional second argument does the fetch method take? And what is it used for in this application? Hint: See Using Fetch on the MDN docs

<!-- Second argument is an init options object. This allows you to customise and configure the request that is being made (eg. method, body, headers) -->

7. Which of the games API routes does the front-end application consume (i.e. make requests to)?

<!-- 
All except the second get and the put. 
  -->


8. What are we using the MongoDB Driver for?

<!-- This is used to pass information from the server to the Mongo database. -->