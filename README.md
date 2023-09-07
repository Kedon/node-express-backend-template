# Node Express Backend Template

## Node Express Backend Architecture

This repository is the practical demonstration of the backend best practices discussed in the article on Medium:  [Medium: Backend Development: Bridging The Communication Gap](https://github.com/Kedon/node-express-backend-template). It's been crafted to serve as a blueprint for setting up a robust Node Express backend architecture.

### Overview

- **Name**: node-express-backend-template
- **Version**: 1.0.0
- **Description**: Simple Node Express Backend Architecture

## Table of Contents
- [Features](#features)
- [Getting Started](#getting-started)
- [Scripts](#scripts)
- [Dependencies](#dependencies)
- [Sequelize ORM](#using-sequelize-with-node-express-backend)
- [Environment Variables](#environment-variables)
- [License](#license)
- [Bugs and Issues](#bugs-and-issues)
- [Author](#author)

## Features
- **Descriptive Ordering in Responses**: Streamlined ordering of API response data.
- **Navigation Support**: Extended information in paginated backend responses.
- **Descriptive Column Names**: Enhancing clarity especially during database operations.

## Getting Started
The main entry to the application is `./build/index.js`.

**Repository**: [GitHub Link](https://github.com/Kedon/node-express-backend-template)

## Scripts
- **Build**: `tsc --skipLibCheck`
- **Start**: `source ./.env.development.sh && nodemon -w`
- **Starter**: `tsc --skipLibCheck && node ./build.js`
- **TS Watch**: `tsc -w`

## Dependencies
Here's a list of core dependencies that power the application:
- bcryptjs
- compression
- cookie-parser
- cors
- dotenv
- express
- pg
- pgtools
- sequelize
- among others

## Using Sequelize with Node Express Backend

Sequelize is one of the most popular ORMs (Object-Relational Mapping) for Node.js and it brings numerous advantages to your backend development:

### Advantages of Using Sequelize:
1. **Database Agnostic**: Sequelize supports multiple databases like PostgreSQL, MySQL, MariaDB, SQLite, and MSSQL. This means you can switch between databases with minimal changes to your codebase.
2. **Model Definition**: Define your table's structure and relationships right within your code, ensuring your database schema and business logic remain in sync.
3. **Migrations & Seeding**: Database migrations allow you to manage changes to your database schema and seed your database with initial data.
4. **Validation**: Built-in validation tools ensure the data you're inserting or updating matches what your application expects.
5. **Flexibility**: Sequelize provides both a high-level ORM API and a lower-level query builder API, letting you choose the best tool for the job.

### Setting Up the First User:

To set up your first user account in the database, follow these steps:

1. Navigate to the file `src/database/models/account.model.ts`.
2. Uncomment the `createAccount()` function. This function has been set up to provide an easy way to seed an initial user into your database.
3. Once you've uncommented and potentially updated the user details within the `createAccount()` function, run your application. This will execute the function and insert a user into the `accounts` table.
4. It's recommended to comment the function again after creating the first user to prevent duplicate entries or unintended database operations in subsequent runs.

Remember, Sequelize is a powerful tool that can speed up development, increase code quality, and create a more maintainable backend. Embrace its features to make the most out of your Node Express Backend.

## Environment Variables
The project makes use of several environment configurations. Find a detailed list in the `.env.development.sh` file. Some key variables include:
- **NODE_ENV**: Determines the application environment.
- **USE_HTTPS**: Activates HTTPS for the server.
- **PORT**: Port number for the server.
- Besides database and other configurations

## License
This project is licensed under the MIT license.

## Bugs and Issues
For any bugs or issues, kindly raise them in the issues section.

## Author
**Valdenir**: Lead Developer and Author of the associated Medium Article.
