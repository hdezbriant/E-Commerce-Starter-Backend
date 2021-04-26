# E-Commerce Starter Backend

## What is this for?
This is a command-line app for initializing a basic E-Commerce database and seeding it with placeholder data to help you get your database off the ground! \
The items included have some associations to mimic what your typical E-Commerce site uses to show effective results with meaningful associations.

## Getting Started

This app uses `MYSQL2` and `Sequelize` packages with `npm` to create, seed, and manage the database and items, so you'll need to install all the packages. Additionally, the app will use the `dotenv` package to provide a dynamic port for accessing the database, and allowing you to share this code with others without revealing your mysql credentials.
The dependencies are already defined in the incluced `package.json`, so all you need to do, is open up your terminal and run:

```
npm install
```

To get all the packages set up!

Use the `schema.sql` file in the `db` folder to create your database using the MySQL shell command: 

```mysql -u **YOUR USERNAME** -p < db/schema.sql```

After completing the prompt by entering your password, a database called `ecommerce_db` will be created!

To seed the newly created database with placeholder data: using your terminal, run the command: 

```npm run seed```

After this step, you're all set!


### Demonstration Video
