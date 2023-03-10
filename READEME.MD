# Meower - Twitter for Cats

A basic twitter clone built to demonstrate the full stack π₯ (client, server, database).

With the following features:

* Cats can send a mew πΈβοΈ
* Cats can see all mews that have been sent π»π

![example-site](example-site.gif)

## Objectives

* [ ] π Diagram the Full Stack
* [ ] π Differentiate between Client and Server
* [ ] β¨οΈ Get user input on the Client
* [ ] β‘οΈ Send user input from the client with fetch to the server
* [ ] π Store data in a database
* [ ] π Retrieve data from a database on the Server
* [ ] β¬οΈ Retrieve data from a server on the client using Fetch
* [ ] π Hide/Show elements on the client
* [ ] β¨ Add elements to the page on the client
* [ ] π Deploy the client with now.sh
* [ ] π Deploy the database with mlab
* [ ] π Deploy the server with now.sh

## Front-end

* [x] Create client folder
* [x] Setup index.html
* [x] Bring in Skeleton CSS
  * http://getskeleton.com/
  * https://cdnjs.cloudflare.com/ajax/libs/skeleton/2.0.4/skeleton.min.css
* [x] Create Header
* [x] Create form
  * [x] Name
  * [x] Content
  * [x] u-full-width to both inputs
* [x] Listen for form submit
* [x] Hide the form
* [x] Show loading spinner
* [x] Get data from form and log it
* β Get user input on the Client
* β Hide/Show elements on the client

## Back-end

* [x] Create server folder
* [x] npm init -y
* [x] npm install express morgan
* [x] Setup index.js
* [x] Add GET / route
* [x] Add POST /mews route
  * [x] log out req.body

## Front-end

* [x] fetch POST /mews with form data
* [x] See the CORS error and revel in this moment
* β Send user input from the client with fetch to the server

## Back-end

* [x] npm install cors
* [x] Make sure the server is recieving the data
* [x] Add JSON body parser middleware
* [x] Validate name and content
  * [x] Must be a string
  * [x] Cannot be empty
* [x] If not valid
  * [x] Error code 422
  * [x] Invalid mew, must contain name and content
* [] Setup DB Connection
  * [] npm install monk
  * [] connect to db
  * [] create document collection (mews)
* [] If Valid
  * [] Create mew object with
    * [] name, content, created_date
  * [] Insert into DB
  * [] Respond with created mew object
* β Store data in a database

## Front-end

* [] Log out created Mew after POST request
* [] Show the form
* [] Hide loading spinner

## Back-end

* [] GET /mews
  * [] Respond with mews from DB
* β Retrieve data from a database on the Server

## Front-end

* [] fetch GET /mews
  * [] Iterate over array
  * [] Append each to page
  * [] Reverse before appending
  * [] Show the form
  * [] Hide loading spinner
* [ ] fetch GET /mews after creating a mew
* β Retrieve data from a server on the client using Fetch
* β Hide/Show elements on the client
* β Add elements to the page on the client

## Back-end

* [ ] npm install bad-words
  * [ ] Use filter before inserting into DB
* [ ] npm install express-rate-limit
  * [ ] Limit to 1 request every 15 seconds

## Deploy

* β Deploy server with now
  * [] Setup environment variables
    * [] Database connection
      * process.env.MONGO_URI
  * β Show mlab
  * [ ] Deploy with environment variable
    * now -e MONGO_URI=@meower-db
  * [ ] Add alias
* β Deploy client folder with now
  * [ ] Set API_URL based on hostname

## What's next?

* Add comments/replies to a mew
* User Accounts
  * Don't just have the user enter their name
  * Sign up/Login
* User Profiles
  - Only show mews from a given user
* Search Mews
* Hashtags
* User @mentions
* Realtime feed of mews