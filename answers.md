1. What is responsible for defining the routes of the `games` resource?
create_router.js within the server structure


2. What do you notice about the folder structure?  Whats the client responsible for? Whats the server responsible for?
Client is handling the input and representation through the container and components, server is handling the routes and the details of the games


3. What are the the responsibilities of server.js?
Sets up an Express server and connects to MongoDB. Links to database collection and creates the routes for the games, then listens on port 9000 for the API routes being called


4. What are the responsibilities of the `gamesRouter`?
Creates API routes to gamesCollection, which is the list of games (i.e. exploding kittens) held in the database


5. What process does the the client (front-end) use to communicate with the server?
I think it uses the fetching in the GamesService to get/post/delete games via the server


6. What optional second argument does the `fetch` method take? And what is it used for in this application? Hint: See [Using Fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch) on the MDN docs
An init argument, to configure a range of settings like use of CORS, the URL methods etc - as it is in this app to set the type of request.


7. Which of the games API routes does the front-end application consume (i.e. make requests to)?
Get all, post, and delete (which takes a game ID as an argument)


8. What are we using the [MongoDB Driver](http://mongodb.github.io/node-mongodb-native/) for?
It's letting us connect Node/Express to MongoDB so we can use fetching and chaining promises through asynchronous actions