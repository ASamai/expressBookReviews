# **Book Review Backend Application Using Node.JS and Express**

This application is a book review system developed using a code template that I forked from the IBM skills network repository during my IBM Full Stack Software developer certification. The name of the course that this final project was made for is "Backend application development with Node.JS and Express".

In this final project, I have built a server-side online book review application and integrated it with a secure REST API server which will use authentication at session level using JWT.The application was tested using Promises callbacks or Async-Await functions.

## Understanding the user routes
Navigate to the router directory having the below 3 files:

booksdb.js - This contains the the preloaded book information for this application.

general.js - This contains the skeletal implementations for the routes which a general user can access.

auth_users.js - This contains the skeletal implementations for the routes which an authorized user can access.

## Getting the list of books available in shop using JSON.stringify
In general.js, the following heading has the code for getting the list of books available in shop using the JSON.stringify method: 
"public_users.get('/',function (req, res) {."

## Getting the book details based on ISBN
In general.js, the following heading contains the code for getting the book details based on ISBN. This was tested using postmanm: "public_users.get('/isbn/:isbn',function (req, res) {"

## Getting the book details based on the Author
In general.js, the following heading contains the code for getting the book details based on the author:
"public_users.get('/author/:author',function (req, res) {"

## Getting the Book Reviews
In general.js, the following heading contains the code for geetting the book reviews:

"public_users.get('/review/:isbn',function (req, res) {"

## Registering users
Code has been entered to register new users

## Signing in users
The code will validate and sign in a customer based on the username and password. It will also save the user credentials for the session as a JWT.

## Adding or modifying book reviews
You have to give a review as a request query & it must get posted with the username (stored in the session) posted. If the same user posts a different review on the same ISBN, it should modify the existing review. If another user logs in and posts a review on the same ISBN, it will get added as a different review under the same ISBN.
