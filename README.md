## E-Commerce Back End

The E-Commerce Back End is a powerful and scalable backend solution for your e-commerce website, allowing you to manage products, categories, and tags efficiently. This application is built using Express.js and Sequelize, providing a robust API to interact with a MySQL database.

## Table of Contents

Installation
Usage
API Routes
Contributing
License

## Installation
To set up and run the E-Commerce Back End on your local machine, follow these steps:

Clone this repository to your local environment using the following command:

## bash

git clone https://github.com/bellaloc/ecommerce.git
Navigate to the project directory:

cd ecommerce

Install the required dependencies:

npm install
Configure the database connection by creating a .env file in the root directory and adding the following environment variables:

makefile in .ENV:

DB_NAME='ecommerce_db'
DB_USER='root'
DB_PASSWORD='Password'


## in mySql run the tables:

DROP DATABASE IF EXISTS ecommerce_db;

CREATE DATABASE ecommerce_db;

## Create and seed the database:

npm run seed
or node seeds/index.js

Start the server:
npm start

Your E-Commerce Back End is now running locally on your machine.

## Usage
Once the server is up and running, you can interact with the API using a tool like Insomnia or Postman.

Ensure you have the API routes and endpoints set up correctly in your API client:

GET routes for categories, products, and tags
POST routes to create new categories, products, and tags
PUT routes to update existing categories, products, and tags
DELETE routes to remove categories, products, and tags
Make sure to include the necessary data in the request body when creating or updating resources.

## API Routes
GET /api/categories: Get all categories.

GET /api/categories/:id: Get a single category by ID.

POST /api/categories: Create a new category.

PUT /api/categories/:id: Update a category by ID.

DELETE /api/categories/:id: Delete a category by ID.

GET /api/products: Get all products.

GET /api/products/:id: Get a single product by ID.

POST /api/products: Create a new product.

PUT /api/products/:id: Update a product by ID.

DELETE /api/products/:id: Delete a product by ID.

GET /api/tags: Get all tags.

GET /api/tags/:id: Get a single tag by ID.

POST /api/tags: Create a new tag.

PUT /api/tags/:id: Update a tag by ID.

DELETE /api/tags/:id: Delete a tag by ID.

Remember to provide the necessary data in the request body when creating or updating resources.

## Contributing
Contributions are welcome! If you'd like to contribute to this project, please follow these guidelines:

## Fork the repository
Create a new branch for your feature or fix
Make your changes
Test your changes
Submit a pull request
License

## This project is licensed under the MIT License - see the LICENSE file for details.