
## PHP 
PHP is a server-side scripting language that is used to create dynamic web pages. It was originally created in 1994 by Rasmus Lerdorf as a set of Common Gateway Interface (CGI) scripts.

PHP is commonly used for web development, but it can also be used as a general-purpose programming language. Some common use cases for PHP include:
1. Creating dynamic web pages
2. Building web applications
3. Developing content management systems (CMS)
4. Creating e-commerce websites
5. Building APIs

The basic syntax of PHP is similar to that of C and Perl. Here’s an example of a simple PHP script:
```
<?php
echo "Hello, world!";
?>
```

Object-oriented programming (OOP) is a programming paradigm that uses objects to represent and manipulate data. In PHP, you can use OOP to create classes that represent database connections and queries.

Here’s an example of a simple PHP class that connects to a MySQL database:

class Database {
  private $host = "localhost";
  private $username = "username";
  private $password = "password";
  private $database = "database";

  public function connect() {
    $dsn = "mysql:host=$this->host;dbname=$this->database";
    $pdo = new PDO($dsn, $this->username, $this->password);
    return $pdo;
  }
}

This class defines a private $host, $username, $password, and $database property, as well as a public connect() method that returns a new PDO object.

To use this class to execute a query, you would first create a new instance of the Database class:

$db = new Database();

Then you could call the connect() method to get a new PDO object:

$pdo = $db->connect();

Once you have a PDO object, you can use it to execute queries against the database.


### Example
This example shows how you can define routes in PHP and use them to include different files based on the current URI. The included files can then generate HTML as needed.

```
<?php
// index.php

// Define routes
$routes = [
    '/' => 'home',
    '/about' => 'about',
    '/contact' => 'contact'
];

// Get the current URI
$uri = $_SERVER['REQUEST_URI'];

// Check if the URI is in the routes array
if (array_key_exists($uri, $routes)) {
    // If it is, include the corresponding file
    include $routes[$uri] . '.php';
} else {
    // If it isn't, show a 404 error
    header('HTTP/1.0 404 Not Found');
    echo '404 Not Found';
}

// home.php
<!DOCTYPE html>
<html>
<head>
	<title>Home Page</title>
</head>
<body>
	<h1>Welcome to the Home Page!</h1>
</body>
</html>

// about.php
<!DOCTYPE html>
<html>
<head>
	<title>About Page</title>
</head>
<body>
	<h1>Welcome to the About Page!</h1>
</body>
</html>

// contact.php
<!DOCTYPE html>
<html>
<head>
	<title>Contact Page</title>
</head>
<body>
	<h1>Welcome to the Contact Page!</h1>
</body>
</html>
```

#### PHP vs ExpressJs

PHP and ExpressJS are both server-side web application frameworks that allow developers to build web applications. However, there are some differences between the two.

PHP is a server-side scripting language that is used to create dynamic web pages. It is one of the most popular programming languages for web development and is used by many websites, including Facebook and Wikipedia. PHP is an open-source language that can be used on any platform.

ExpressJS, on the other hand, is a Node.js web application framework that is used to build web applications. It provides a set of features for building web applications, including routing, middleware support, and templating engines. ExpressJS is also open-source and can be used on any platform.

One of the main differences between PHP and ExpressJS is that PHP is a programming language while ExpressJS is a framework. This means that PHP can be used to build any type of application while ExpressJS is specifically designed for building web applications.

Another difference between the two is that PHP has been around for much longer than ExpressJS. PHP was first released in 1995 while ExpressJS was first released in 2010. This means that PHP has a larger community and more resources available than ExpressJS.