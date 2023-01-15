# Complete Mongo

Just a REST api's done using node js and mongo db just for practice.

This application has books as a collection. There are api's like GET, POST, PATCH and DELETE
which are used to insert the book, view, update and delete the book from the books collection

## Installation involved when creating this repo (This is only one time)

- npm init
- npm install express --save
- npm install -g nodemon
- npm install mongodb --save

## Instructions to Run this Repo

- npm install
- Add the Mongo db connection string in db.js file
- nodemon app
- Import postman collection
- Create Mongo DB as bookstore and create a books collection.
- Add document in database/books.json just as a reference
- Run the API from Postman collection

## How to execute queries in mongo shell - mongo db compass

### `show dbs`

This will show all the databases present in the mongo db

### `Use db bookstore`

You can select the required database. In this case we are using the bookstore database.

### `Bookstore.books`

You can go in that particular collection that you are going to use.

### `db.books.find({"author":"Mock Author"})`

Find the books those are having author as Mock Author

- Note: You can try other queries in mongo shell.

## What are indexes and how to add indexes in mongo db

### `db.books.createIndex({ rating:6})`

To create the index

### `db.books.find({rating:6}).explain('executionStats')`

This will just show the stats for that particular index

### `Get the index: db.books.getIndexes()`

To get the indexes on the particular collection

### `Drop the index: db.books.dropIndex({rating:6})`

Used to drop the index for the particular collection
