# LightBnB


LightBnB is an easy to use website that will help you book your next holiday accomadation with ease!
This was a database based project where SQL was primarily used to write my queries. The front end and back end of this website were forked while I focused mainly on the server and database. 

# Final Product
| !["Project home page!"](https://github.com/aidanantony/LightBnB/blob/main/LightBnB_WebApp-master/public/javascript/components/Home-page.png) |

| !["Create new listing page!"](https://github.com/aidanantony/LightBnB/blob/main/LightBnB_WebApp-master/public/javascript/components/Create-new-listing.png) |

| !["ERD diagram!"](https://github.com/aidanantony/LightBnB/blob/main/LightBnB_WebApp-master/public/javascript/components/ERD-diagram.png) |

# Setup
Just use the following commands to set up. Run the commands inside the quotes but do not include the quotes. To isntall, use the command "npm install". Next use "npm run local". You should now be able to see it in your browser at localhost:3000



## Project Structure

```
├── public
│   ├── index.html
│   ├── javascript
│   │   ├── components 
│   │   │   ├── header.js
│   │   │   ├── login_form.js
│   │   │   ├── new_property_form.js
│   │   │   ├── property_listing.js
│   │   │   ├── property_listings.js
│   │   │   ├── search_form.js
│   │   │   └── signup_form.js
│   │   ├── index.js
│   │   ├── libraries
│   │   ├── network.js
│   │   └── views_manager.js
│   └── styles
├── sass
└── server
  ├── apiRoutes.js
  ├── database.js
  ├── json
  ├── server.js
  └── userRoutes.js
```

* `public` contains all of the HTML, CSS, and client side JavaScript. 
  * `index.html` is the entry point to the application. It's the only html page because this is a single page application.
  * `javascript` contains all of the client side javascript files.
    * `index.js` starts up the application by rendering the listings.
    * `network.js` manages all ajax requests to the server.
    * `views_manager.js` manages which components appear on screen.
    * `components` contains all of the individual html components. They are all created using jQuery.
* `sass` contains all of the sass files. 
* `server` contains all of the server side and database code.
  * `server.js` is the entry point to the application. This connects the routes to the database.
  * `apiRoutes.js` and `userRoutes.js` are responsible for any HTTP requests to `/users/something` or `/api/something`. 
  * `json` is a directory that contains a bunch of dummy data in `.json` files.
  * `database.js` is responsible for all queries to the database. It doesn't currently connect to any database, all it does is return data from `.json` files.