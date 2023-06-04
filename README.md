# Survey Results Web Application

This is a web application that displays survey results, including total surveys, average age, oldest and youngest person, food preferences, and entertainment preferences. The application uses Node.js, Express.js, MongoDB, and HTML/CSS for the server, database, and frontend components.

Installation

To run the Survey Results web application locally, please follow these steps:

Clone the repository:
bash
Copy code
git clone <repository_url>
Install the required dependencies by navigating to the project directory and running:
Copy code
npm install
Set up the MongoDB connection by providing your MongoDB database URL in the .env file located in the project's root directory:
makefile
Copy code
MONGODB_URI=<your_mongodb_url>
Start the server by running:
sql
Copy code
npm start
Access the web application by opening your browser and visiting http://localhost:3000.

Code Structure

The code for the Survey Results web application is structured as follows:

server.js: The entry point of the application. Sets up the server, connects to the database, and defines the API routes.
models/dataModel.js: Defines the Mongoose schema and model for the survey data. The schema includes fields for the surname, name, contact, currentDate, age, favoriteFoods, and ratings.
public/index.html: The HTML file that displays the survey results. It includes JavaScript code to fetch data from the server and populate the values dynamically.
public/style.css: The CSS file that styles the HTML elements.
routes/api.js: Defines the API routes for fetching the survey data. It uses the DataModel to interact with the MongoDB database.
Survey Data Model

The survey data is stored in a MongoDB database using Mongoose. The DataModel defined in models/dataModel.js represents the data schema and provides an interface to interact with the data. The schema includes the following fields:

surname (String): The surname of the survey respondent.
name (String): The name of the survey respondent.
contact (String): The contact information of the survey respondent.
currentDate (Date): The date when the survey was submitted.
age (Number): The age of the survey respondent.
favoriteFoods (Array of Strings): The favorite foods of the survey respondent.
ratings (Object): The ratings for different entertainment preferences (eatOut, watchMovies, watchTV, listenToRadio).
API Routes

The application provides the following API routes:

GET /api/survey-data: Retrieves the survey data from the database and returns it as JSON. This data is used to populate the survey results in the HTML file.

Dependencies

The Survey Results web application uses the following major dependencies:

express: A minimal and flexible web application framework for Node.js.
mongoose: An Object Data Modeling (ODM) library for MongoDB and Node.js.
dotenv: A module to load environment variables from a .env file.
Conclusion

The Survey Results web application provides an interface to view and analyze survey data. By following the installation instructions, you can set up the application locally and explore the survey results in your browser.

For any questions or issues, please contact shongwe1408@gmail.com.com.







