# Backend of ECommerce Application

## Purpose
This is the backend of an ecommerce application. The purpose of this project is to provide the user with a connection to their database that is functionally useable on the frontend of their site. 

### User Story
AS A manager at an internet retail company
I WANT a back end for my e-commerce website that uses the latest technologies
SO THAT my company can compete with other e-commerce companies

## Application Details
Since this is purely a backend application, there is no live deployment. To use or test the app, follow the installation instructuions.

This application uses the sequelize package to connect the server to the database.

### Installation
To use the app, clone the repository to your local machine and run an npm install. To create the database, source the schema.sql file in your SQL shell. Then, run npm run seed in your terminal to seed the database. Then run npm start to start the server and test the API endpoints using your preferred method (Postman, Insomnia, etc.). 

Server will run locally on port 3001.

### Code Summary
There are 4 Models: Category, Product, Tag, and ProductTag. ProductTag is a through table for relating Product & Tag in a many-to-many relationship. 

API routes are split into the following files: category-routes, product-routes, and tag-routes.

Each has api endpoints written for get all from table, get one from table based on id, delete one from table based on id, update one, and post one. 

The API endpoints are:
- /api/categories
- /api/categories/:id
- /api/products
- /api/products/:id
- /api/tags
- /api/tags/:id

### Technologies Used
Backend: Javascript, Node.js

Project dependencies: Express.js, mysql2, sequelize, dotenv

## Deployed Application

[Link to Google Drive Walkthrough Video](https://drive.google.com/file/d/1HdSGnKSWSG1qpppa--w7IJZS5iG4maZi/view)
