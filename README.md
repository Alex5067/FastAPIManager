# User Manager

## Backend

The project backend is made using Python.
The database was created using SQLAlchemy.
The framework for creating the RESTful API is FastAPI.
The backend needs to be running for the frontend to work.

### Models

There are 2 entities:

Admin:
*   id
*   email
*   hashedPW
*   users (relation with User)

User:
*   id
*   avatar
*   email
*   firstName
*   lastName
*   position
*   skills
*   adminId (relation with Admin)

## Frontend

The project frontend is made using React.
The styles of each component are modified in their respective .css.
The skills chart uses the Chart.js library.

### Usage

### `git clone https://github.com/Alex5067/FastAPIManager.git src`
### `cd src/docker`
### `docker-compose up`

First you need creaate admin with email and password on backend, then you will can login on frontend and see all users from database.
Open [http://localhost:8000/docs](http://localhost:8000/docs) to view API methods.

The page will reload if you make edits.\
The page shows all the available CRUD options for the backend.
Using the "Try it out" option for each operation modifies the database.db file or use Postman.


Open [http://localhost:3000](http://localhost:3000) to view web-form allow you check users.
The page will reload if you make edits.

