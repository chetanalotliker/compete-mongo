Installation involved when creating this repo (This is only one time)

- npm init
- npm install express --save
- npm install -g nodemon
- npm install mongodb --save

Instructions to Run this Repo

- npm install
- Add the Mongo db connection string in db.js file
- nodemon app
- Import postman collection
- Create Mongo DB as bookstore and create a books collection.
- Add document in database/books.json just as a reference
- Run the API from Postman collection

How to execute queries in mongo shell - mongo db compass

- Show dbs
- Use db bookstore
- Bookstore.books
- db.books.find({"author":"Mock Author"})

Note: You can try other queries in mongo shell.

What are indexes and how to add indexes in mongo db

- To create index: db.books.createIndex({ rating:6})
- Run this stats: db.books.find({rating:6}).explain('executionStats')
- Get the index: db.books.getIndexes()
- Drop the index: db.books.dropIndex({rating:6})
