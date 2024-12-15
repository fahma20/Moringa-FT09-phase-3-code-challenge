## Article, Author, and Magazine Management System
This project implements a Magazine domain with three models: Author, Article, and Magazine. It demonstrates CRUD functionality and relationships between authors, articles, and magazines.

## Features
Author: Manage authors with name validation and database CRUD operations.
Magazine: Manage magazines with name and category validation and CRUD operations.
Article: Manage articles with title validation and CRUD operations, linked to authors and magazines.

## Relationships
Authors can have multiple articles and contribute to multiple magazines (many-to-many).
Articles are associated with a single author and magazine.
Magazines can have many articles and authors.

## Setup Instructions

1. Install dependencies:

   `` pipenv install``

2. Activate the virtual environment:

    ``pipenv shell``

3. Initialize the database:

    ``python3 app.py``

## Core Methods

1. Author
Create, Read, Update, Delete (CRUD) authors.
Author names are non-modifiable after creation.
2. Magazine
CRUD magazines with name and category validation.
Magazines can be updated after creation.
3. Article
CRUD articles with title validation.
Articles are linked to authors and magazines via foreign keys.

 ## Relationships and Aggregation
Articles return their associated author and magazine.
Authors can retrieve all articles and magazines they’ve contributed to.
Magazines can retrieve all articles and authors contributing to them.

## Running Tests
Run tests with:
  ``pytest``

## License
This project is licensed under the MIT License.


