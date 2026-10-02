# Task 1 — Foundations & Product Catalog

# Tech Stack
. Server : Node.js, KOA , PostreSQL</br>
. Client : React(Next.js), Typescript

# Prequisites
 -> Node.js (v.18.0.0 or higher)</br>
 -> npm installed</br>
 -> A running instance of Postgresql.

# Configure enviroment variables:
  -> Create a `.env` file in the root directory and add your configuration details:</br>
     **DB_Details**</br>
     . DB_PORT     :"DB_PORT",</br>
     . DB_HOST     :"DB_HOST",</br>
     . DB_USER     :"DB_USER",</br>
     . DB_PASSWORD :"DB_PASSWORD",</br>
     . DB_NAME     :"DB_NAME',</br>
     **Server**</br>
     .PORT = "Server port"

# Route
  |**GET**| = `/products`      | Fetch a list of all products List/Items.</br>
  |**Get**| = `/products/:id`  | Fetch a Specific products by ID.</br>

  **http://localhost:`PORT`/products </br>**
  **http://localhost:`PORT`/products/:id**

###Repository Structure
#Server</br>
├── src/</br>
│   ├── controllers/      # Handles business logic for each route</br>
│   ├── models/           # Data definitions (schemas / ORM models)</br>
│   ├── dbconfig/         # Database connection and environment configurations </br>
│   ├── migrations/       # Database schema history and version control scripts</br>
│   ├── routes/           #  All application route definitions</br>
│   │   └── product_route.js</br>
│   └── index.js            # Main entry point mounting the root router</br>
└── package.json</br>
