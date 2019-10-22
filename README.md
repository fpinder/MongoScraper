# Mongo Scraper

[Mongo Scraper!](https://evening-savannah-93916.herokuapp.com/)

**Object**

_The Application [Mongo Scraper!](https://evening-savannah-93916.herokuapp.com) hosted on Heroku is created has a web app that lets users view and leave comments on the latest New York Times news. Whenever a user visits the site, the app will scrape stories from a New York Times news and display them on the screen. Each scraped article is saved to the application database. The Mongo Scraper app will display the following information for each article: The `Headline` - the title of the article; The `Summary` - a short summary of the article; and The `URL` - the url to the original article. Users are able to leave comments on the articles displayed and revisit them later. The comments are saved to the database as well and associated with their articles. Users are able to delete comments left on articles. All stored comments arre visible to every user._

`home handlebars Page`

<a href="#"><img src="https://github.com/fpinder/MongoScraper/blob/master/public/assets/images/background.jpg" alt="Home Page"></a>

`Articles Scraped`

<a href="#"><img src="https://github.com/fpinder/MongoScraper/blob/master/public/assets/images/Capture2.jpg" alt="Articles Scraped"></a>

_The application also has an error checking process in the to preevent duplicated news in the database. Additionaly, `notes-modal.handlebars` ensure that the user has entered a note to prevent empty fields in the database_

`Note Checking`

<a href="#"><img src="https://github.com/fpinder/MongoScraper/blob/master/public/assets/images/Capture4.jpg" alt="Note Checking"></a>

`Notes`

<a href="#"><img src="https://github.com/fpinder/MongoScraper/blob/master/public/assets/images/Capture5.jpg" alt="Notes"></a>

_The application also provides a process for the user to delete the articles. However, the saved article are not deleted_

`Clear Articles`

<a href="#"><img src="https://github.com/fpinder/MongoScraper/blob/master/public/assets/images/Capture6.jpg" alt="Clear Articles"></a>

**_Technology used_**

_This app uses JavaScript, Node.js, Mysql and 5 NPM packages: Express, Express-handlebars, express-validato, Body-parser, dotenv and Nodemon_

| Files Used         | Role in the App                                                                                                                                                         |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| node_modules       | node modules includes the NPM packages                                                                                                                                  |
| express            | used to handle routing                                                                                                                                                  |
| .gitignore         | This will tell git not to track these files, and thus they won't be committed to Github                                                                                 |
| package.json       | JSON Source file the has all the dependencies.                                                                                                                          |
| bodyParser         | Used to sets up the Express app to handle data parsing.                                                                                                                 |
| mongoose           | It manages relationships between data, provides schema validation, and is used to translate between objects in code and the representation of those objects in MongoDB. |
| axios              | is a promise-based HTTP client that works both in the browser and in a node.js environment.                                                                             |
| exprese-handlebars | Handlebars provides the power necessary to let you build semantic templates effectively with no frustration.                                                            |
| cheerio            | is a Node.js library that helps developers interpret and analyze web pages using a jQuery-like syntax.                                                                  |

#

Lincense by <a href="https://creativecommons.org/licenses/by/3.0/" rel="nofollow">CC-BY</a>
