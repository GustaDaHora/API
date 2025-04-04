# Contact API

A simple RESTful API built with Node.js and Express.js for serving static content to the front end of a Notes application with basic authentication capabilities.

## Features
- RESTful API endpoints
- SQLite database integration with Knex.js
- Password hashing with bcryptjs
- Async error handling
- Development mode with auto-restart
- Database migration support

## Prerequisites
- Node.js (v14.x or higher recommended)
- npm (v6.x or higher)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/GustaDaHora/API.git
cd API
```

2. Install dependencies:

```bash
npm install
```

Run database migrations:

```bash
npm run migrate
```

Start the server:

```bash
npm start
```

The API will be running on http://localhost:3000 by default (port may vary based on server.js configuration).

Available Scripts
```
npm start
```
Runs the production server
```
npm run dev
```
Runs with nodemon for development
```
npm run migrate
```
Runs database migrations

Dependencies
> express: Web framework
> knex: SQL query builder
> sqlite3: SQLite database
> bcryptjs: Password hashing
> express-async-errors: Async error handling

Development
For development with live reloading:

```bash
npm run dev
```

To create a new database migration:

```bash
npx knex migrate:make migration_name
```

Configuration
Database: SQLite (configured in knexfile.js)

Port: Defined in src/server.js (default: 3000)

Add environment variables as needed in a .env file

Contact
Author: Gustavo da Hora
GitHub: [GustaDaHora](github.com/GustaDaHora)
