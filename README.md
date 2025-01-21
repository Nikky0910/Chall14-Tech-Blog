# Chall14-Tech-Blog

## Description

This application serves as a CMS-style blog platform for developers to publish their blog posts and engage with others through comments. Built entirely from scratch, it follows the Model-View-Controller (MVC) paradigm and is deployed to Render. The application utilizes Handlebars.js for dynamic templating, Sequelize for efficient database management, and express-session to provide secure user authentication.

## Table of Contents (Optional)

- [Installation](#installation)
- [Usage](#usage)
- [License](#license)

## Installation

Follow these steps to set up and run the e-commerce back-end project locally:

1. **Clone the Repository**  
   First, clone the repository to your local machine using the following command:

   ```bash
   git clone https://github.com/Nikky0910/Chall14-Tech-Blog
    ```
2. **Navigate to the Project Directory**  
   After cloning, navigate to the project directory:

   ```bash
   cd Chall14-Tech-Blog
    ```
3. **Install Dependencies**  
    Install the required Node.js packages by running:

   ```bash
   npm install
    ```
    This will install the following dependencies:
    - **dotenv**: Loads environment variables from a .env file into process.env, keeping sensitive information secure.
    - **express**: A web framework for building a robust API and handling HTTP requests and routing.
    - **pg**: The PostgreSQL client for Node.js, used to interact with the database.
    - **sequelize**: An ORM library for Node.js that simplifies database management with models, associations, and queries.
    - **bcrypt**: A library for hashing passwords
    - **express-session**: A middleware for session management.
    - **connect-session-sequelize**: a middleware to store session data in the database.
    - **express-handlebars**: a templating engine for dynamic content rendering.

4. **Set Up Enviroment Variables**  
    Create a .env file in the root directory and configure it with the following variables:
     ```bash
     DB_USER="postgres"
     DB_PASSWORD= "your_password"
     DB_NAME="techblog_db"
     ```
     Replace your DB_USER, DB_PASSWORD and DB_NAME with your PostgreSQL database credentials.

5. **Run the database** 
    Navigate to the db folder through the terminal and run the schema by typing:
    ```bash
   psql -U postgres
   \i schema.sql
   \c techblog_db;
    ```

6. **Seed your database**
    Run the seed by typing:
        ```bash
            npm run seed
        ```
6. **Start the server**  
   Launch the application by running:

   ```bash
   npm start
    ```
    The server should start on  http://localhost:3001 or the port specified in your environment variables.

## Usage

Link to the GitHub repository:

<a href = "https://github.com/Nikky0910/Chall14-Tech-Blog"> Github Repo</a>

Link to the deployed application: 

<a href = "https://chall14-tech-blog.onrender.com"> TechBlog website</a>

## License

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
