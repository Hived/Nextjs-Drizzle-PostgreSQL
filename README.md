# Next.js with PostgreSQL and Drizzle ORM Starter

A starter project/template for building web applications with Next.js, PostgreSQL, and Drizzle ORM. This project includes a basic setup with Drizzle, an Object-Relational Mapping (ORM) library, and uses Docker for PostgreSQL, making it easy to kickstart your development with Next.js, PostgreSQL, Drizzle, and containerization.

## Features

- **Next.js:** React framework for building web applications.
- **PostgreSQL:** A powerful open-source relational database system.
- **Drizzle ORM:** Object-Relational Mapping for simplified database interactions.
- **Docker:** Containerization for PostgreSQL database.

## Getting Started

1. **Install dependencies:**

    ```bash
    npm install
    ```

2. **Set up PostgreSQL with Docker:**

    - Make sure you have Docker installed.
    - Update the database configuration in `docker-compose.yml` and `.env`. Replace `myusername`, `mypassword`, and `mydatabase` with your desired PostgreSQL username, password, and database name and `/path/on/host` with your path.
    - Run the following command to start a PostgreSQL container:

    ```bash
    docker compose up
    ```

3. **Run the application:**

    ```bash
    npm run dev
    ```

    The application will be accessible at `http://localhost:3000`.

4. **Run the Drizzle ORM:**

    - Push your schema changes directly to the database

    ```bash
    npx drizzle-kit push:pg
    ```

    - Run the drizzle studio

    ```bash
    npx drizzle-kit studio
    ```

    The application will be accessible at `https://local.drizzle.studio/`.

## Contributing

Feel free to contribute by opening issues or pull requests.
