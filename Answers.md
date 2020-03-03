1) What is responsible for defining the routes of the games resource?
create_router.js in the server/helpers/ folder within Express.

2) What do you notice about the folder structure? Whats the client responsible for? Whats the server responsible for?
games_app consists of two components, Client and Server. Client is responsible for the front end side of things, rendering items and communicating with the server. Server is responsible for the backend side of things, such as seeding the Database, RESTful routes, running the database and communicating with the database via client requests.

3) What are the the responsibilities of server.js?
To allow Cross Origin Resource Sharing (cors), running middleware.

4) What are the responsibilities of the gamesRouter?
To create a reusable router that functions with the "/api/games" file path to allow dry code with regards to following RESTful Routes.

5) What process does the client (front-end) use to communicate with the server?
eventBus?

6) What optional second argument does the fetch method take? And what is it used for in this application? Hint: See Using Fetch on the MDN docs
Post request. Jsonifying the payload that is fed in.

7) Which of the games API routes does the front-end application consume (i.e. make requests to)?
router.get (/api/games - line 8), router.post (/api/games - line 32) and router.delete (/api/games/:id - line 46).

8) What are we using the MongoDB Driver for?
