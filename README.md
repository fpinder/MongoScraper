# Burger

[Mongo Scraper!](https://evening-savannah-93916.herokuapp.com/)

**Object**

_The Application [Mongo Scraper!](https://evening-savannah-93916.herokuapp.com) hosted on Heroku is created has a web app that lets users view and leave comments on the latest New York Times news. Whenever a user visits the site, the app will scrape stories from a New York Times news and display them on the screen. Each scraped article is saved to the application database. The Mongo Scraper app will display the following information for each article: The `Headline` - the title of the article; The `Summary` - a short summary of the article; and The `URL` - the url to the original article. Users are able to leave comments on the articles displayed and revisit them later. The comments are saved to the database as well and associated with their articles. Users are able to delete comments left on articles. All stored comments arre visible to every user._

`home handlebars Page`

<a href="#"><img src="https://github.com/fpinder/burger/blob/master/public/assets/images/eat_the_burger_Readme.JPG" alt="Home Page"></a>

_The application also has an error checking process `(express-validator)` before the page is submitted to ensure that the user has entered a burger name to prevent empty fields in the database_

`Error Checking`

<a href="#"><img src="#" alt="error checking"></a>

**The application Burger is organized with the following structure:**

```
Burger
.
├── config
│   ├── connection.js
│   └── orm.js
│ 
├── controllers
│   └── burgers_controller.js
│
├── db
│   ├── schema.sql
│   └── seeds.sql
│
├── models
│   └── burger.js
│ 
├── node_modules
│ 
├── package.json
│
├── public
│   └── assets
│       ├── css
│       │   └── burger_style.css
│       └── img
│           └── burger.png
│  
│
├── server.js
│
└── views
    ├── index.handlebars
    └── layouts
        └── main.handlebars


```

**_Technology used_**

_This app uses JavaScript, Node.js, Mysql and 5 NPM packages: Express, Express-handlebars, express-validato, Body-parser, dotenv and Nodemon_

| Files Used         | Role in the App                                                                                                                                                   |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| node_modules       | node modules includes the NPM packages                                                                                                                            |
| express            | used to handle routing                                                                                                                                            |
| .gitignore         | This will tell git not to track these files, and thus they won't be committed to Github                                                                           |
| package.json       | JSON Source file the has all the dependencies.                                                                                                                    |
| bodyParser         | Used to sets up the Express app to handle data parsing.                                                                                                           |
| Dotenv             | Dotenv is a zero-dependency module that loads environment variables from a .env file into process.env.                                                            |
| Express            | A minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications.                                  |
| Express-handlebars | Handlebars provides the power necessary to let you build semantic templates effectively with no frustration.                                                      |
| Nodemon            | nodemon is a tool that helps develop node.js based applications by automatically restarting the node application when file changes in the directory are detected. |
| express-validator  | Express middleware for the validator module.                                                                                                                      |

**Config Setup:** _`connection.js` setup the code to connect Node to MySQL. `orm.js` methods that will execute the necessary MySQL commands in the controllers. These methods will be used to retrieve and store data in your database_

**Model Setup:** _`burger.js` the code that will call the ORM functions using burger specific input for the ORM_

**Controller Setup:** _`burgers_controller.js` control the routers for the app_

**View Setup:** _`index.handlebars` file used by Handlebars and `index.handlebars` to have the template that Handlebars can render onto_

**DB Setup/excerpts** _The application's data is stored in MySql via the `schema.sql.` and `seeds.sql`_

**Schema.sql**

```
DROP DATABASE IF EXISTS burgers_db;

CREATE DATABASE burgers_db;

USE burgers_db;

CREATE TABLE burgers
(
id int NOT NULL AUTO_INCREMENT,
burger_name varchar(255) NOT NULL,
devoured BOOLEAN DEFAULT false,
PRIMARY KEY (id)
);

```

**Seeds.sql**

```
INSERT INTO burgers  (burger_name, devoured) VALUES ('Beef Burgers', false);
INSERT INTO burgers  (burger_name, devoured) VALUES ('Turkey Burgers', false);
INSERT INTO burgers  (burger_name, devoured) VALUES ('Veggie Burgers', false);
```

#

Lincense by <a href="https://creativecommons.org/licenses/by/3.0/" rel="nofollow">CC-BY</a>
