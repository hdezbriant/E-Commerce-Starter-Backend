## ![badge](https://img.shields.io/static/v1?label=Licence&message=MIT&color=blue&style=plastic)

# E-Commerce Starter Backend

## What is this for?
This is a command-line app for initializing a basic E-Commerce database and seeding it with placeholder data to help you get your database off the ground! \
The items included have some associations to mimic what your typical E-Commerce site uses to show effective results with meaningful associations.
This app honors the CRUD system, meaning that you will be able to Create, Read, Update, and Delete data from the database.

## Getting Started

This app uses `MYSQL2` and `Sequelize` packages with `npm` to create, seed, and manage the database and items, so you'll need to install all the packages. Additionally, the app will use the `dotenv` package to provide a dynamic port for accessing the database, and allowing you to share this code with others without revealing your mysql credentials.
The dependencies are already defined in the incluced `package.json`, so all you need to do to get all the packages set up, is open up your terminal and run:

```npm install```

After that process is finished, use the `schema.sql` file in the `db` folder to create your database using the MySQL shell command: 

```mysql -u **YOUR USERNAME** -p < db/schema.sql```

After completing the prompt by entering your password, a database called `ecommerce_db` will be created!

To seed the newly created database with placeholder data: using your terminal, run the command: 

```npm run seed```

After this step, you're all set to fire up your server! Use the following command to get started!

```npm start```

## Testing Your Routes
Using `Insomnia`, you will be able to test the routes and requests to following api routes to access the respective tables:

```localhost:3001/api/categories```  
```localhost:3001/api/products```  
```localhost:3001/api/tags```  

Each of these routes will accept both `GET` and `POST` requests to Read All entries, and Create a new entry, respectively.  
In order to view a SINGLE Category, Product, or Tag, you will have to append the path with:  
```/*IDNUMBER*```  
Using the ID number of the desired item in the respective table.

Note that you MUST provide data in the form of a JSON in order to Create a new item or Update an existing one.  
Here's an example for updating the "Running Shoes" item in the "Products" table:  
```
{
   "product_name": "Combat Boots",
   "price": 120.00,
   "stock": 1,
   "tagIds": [1]
}
```  
In this case, we are updating the Product's Name, Price, How many are in Stock, and which Tags the item is associated with.

### Demonstration Video
### [Please refer to this video for a full demonstration!]()

### Contribution and Contact
If you have any feedback or suggestions, feel free to [E-mail me!](mailto:hernandez.briant@gmail.com)
