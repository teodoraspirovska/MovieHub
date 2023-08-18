# MovieHub
I developed a web application using Python and Flask, along with HTML, CSS, Bootstrap for styling, Jinja for templating, and SQLAlchemy for database interaction. The application allows users to add, rate, edit, and delete movies.

## Technologies Used:

Flask: A Python web framework that handles routing, rendering templates, and managing requests.
SQLAlchemy: A library for working with databases in a Pythonic way, allowing us to define models as classes.
Flask-WTF: An extension that integrates WTForms, a library for creating and handling forms.
Flask-Bootstrap: An extension that integrates Bootstrap styles and components into the Flask application.

## Project Flow:

### Importing Required Libraries:

Import necessary libraries like Flask, SQLAlchemy, Flask-WTF, Bootstrap, and more.

### Setting Up API and Database Configuration:

Set up API key and URLs for communicating with themoviedb.org API.
Configure the Flask app and create a SQLite database using SQLAlchemy.

### Defining the Database Model:

Define a database model Movie with attributes like id, title, year, description, rating, ranking, review, and img_url.

### Creating Forms:

Create two FlaskForm classes (FindMovieForm and RateMovieForm) using Flask-WTF.
These forms are used to collect input from users for adding movies and rating movies.

### Routing and Views:

Define routes using Flask's @app.route() decorator.
The main page (/) lists all movies, sorted by their ratings.

![card front home](https://github.com/teodoraspirovska/MovieHub/assets/133661233/e81d9ae1-c1c0-4e48-b915-3ecbdb38a679)

![card back home](https://github.com/teodoraspirovska/MovieHub/assets/133661233/4fefdfdc-d3a2-4dc3-8a56-dc210e5722dd)

The home function retrieves movies from the database and calculates their rankings.
The add_movie function handles adding movies by querying themoviedb.org API and displaying options for selection.

![add](https://github.com/teodoraspirovska/MovieHub/assets/133661233/cd8cedf3-7e02-4c29-9fb1-c8cee2267dfb)

The find_movie function is used to finalize adding a movie after selection.

![select](https://github.com/teodoraspirovska/MovieHub/assets/133661233/6c70b8c7-781c-4b17-9bca-61b4f8c1e805)

The rate_movie function allows users to rate and review a movie.
![rate movie](https://github.com/teodoraspirovska/MovieHub/assets/133661233/f356145e-d990-4022-a4da-4392f9ea2478)

The delete_movie function handles movie deletion.
![delete](https://github.com/teodoraspirovska/MovieHub/assets/133661233/87b16cf1-083e-43eb-a61c-cc878ad6cd88)

## Templates and Rendering:
Use Jinja templating engine to dynamically render HTML templates with data.
HTML templates are stored in the templates folder.
Bootstrap classes are used for styling.

## What I Learned:
Throughout this project, I learned to create a web application using Flask, integrating forms for user input, connecting to an external API, utilizing a database using SQLAlchemy, implementing CRUD (Create, Read, Update, Delete) functionality, and styling the application with Bootstrap.

## Conclusion:
In summary, I developed a Flask web application that allows users to manage movies. Users can add movies by searching for them on themoviedb.org, rate and review movies, and also delete movies. The application uses HTML templates, Bootstrap for styling, Flask for routing, SQLAlchemy for database operations, and WTForms for handling forms. This experience enhanced my skills in web development, API integration, and database management.
