# PHP, PDO and Databases

## Setting up
This practical is about using PHP to work with a MySQL database. We will work with the films tables we created in the practical last week. If you don't have these handy you can import the *films.sql* file. 

## Listing all items from the database
In a text editor open list.php.

Modify the connection settings so that you use the values for your MySQL database, username and passwork. These should be:
* database: student number e.g. u1234567
* username: student number e.g. u1234567
* password: date of birth e.g. 01jan97

Add a foreach loop in the body of the document that will display the title of each of the films.

## Creating a 'browseable' list
Using the lecture slides/example as a guide build a simple ‘browseable’ web application
  * Modify your list.php page so that each film is displayed as a hyperlink that links to a page named *details.php* (you will need to create a *details.php* page).
  * If you can get this to work, try and pass the specific film's id in the query string.
  * In *details.php* connect to your database and run a query that will display the full details for the selected film. 

## Create a search facility for your *films* table
* Create a new HTML page and add the following form:
```html
<form action="results.php" method="get">
<label for="search">Enter a search term:</label>
<input type="text" name="search" id="search">
<input type="submit" name="submitBtn" value="Search">
</form>
```

* Create a PHP page *results.php*. To start with simply get it to display the search term the user has entered
* Look at the lecture slides and example for advice on how you can use this search term to query a database and display films with titles that match the search term
* If you can get this to work, try and build a more sophisticated search facility e.g, You could use a select menu like the following that would allow users to search by film title or by year. You will need to make some changes to *results.php* as well to allow for the more flexible search.

```html
<label for="field"></label>
<select id="field" name="field">
    <option value="title">Film Title</option>
    <option value="year">Film Year</option>
</select>
```

## There's more
* We haven't looked at writing PHP for key actions such as create, update or delete. We will look at these in week 10.
* Using the above examples as a basis you are now in a position to attempt the assignment. See the Assignment Worksheet under Assignments on Unilearn for a suggested workflow.  
