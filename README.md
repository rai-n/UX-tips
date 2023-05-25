## Lazy loading
Lazy loading is an optimization technique that lets the WordPress website only load the media, for example, content and images currently visible to the user’s screen. This delays the loading time of media that the user has not seen yet. Eventually, it helps to boost website performance and decrease page loading times.

Here are some ways to optimize lazy loading for WordPress:

1. Use a lazy loading plugin: There are several plugins available that can help you implement lazy loading on your WordPress site.
2. Use a CDN: A content delivery network (CDN) can help you speed up your website by caching your content and delivering it from servers closer to your users.
    - Choose a reliable CDN provider
    - Install CDN enabler plugin to integrate the CDN service to your site
    - E.g. WP Super Cache, WP Rocket
3. Optimize your images: Optimizing your images can help you reduce their file size and improve your website’s performance. 

## Click through rate
CTR stands for Click-Through Rate. It is a ratio showing how often people who see your ad or free product listing end up clicking it. CTR can be used to gauge how well your keywords and ads, and free listings, are performing.

For example, if your ad is shown 100 times and clicked on 10 times, then your CTR is 10%. A high CTR is preferable because it means that users find your ad or webpage highly relevant and engaging to the target audience.

### Optimize
There are several ways to optimize click-through rates (CTR) and conversion rates. Here are some strategies that can help you improve your CTR and conversion rates:

1. Improve your audience qualification: The more qualified your audience is in relation to your ad, the higher the click-through rate will be.
2. Target the right times of day: Your audience may be online and open to your message at specific times of the day.
3. Improve your messaging: Make sure your messaging is clear and concise.
4. Improve your calls to action: Make sure your calls to action are clear and compelling.
5. Multiply the number of ad variations: By creating multiple ad variations, you can test which ads perform best and optimize accordingly.

## Skeleton screens
A skeleton screen is a blank version of the page that is displayed while the content is being loaded. This gives the user an idea of what the page will look like and helps them understand that content is being loaded.

Here are some benefits of using skeleton screens:

1. **Improved user experience**: Skeleton screens can help improve user experience by reducing perceived load times.
2. **Reduced bounce rates**: Faster load times can help reduce bounce rates.
2. **Better engagement**: Users are more likely to engage with your website if it loads quickly.

### Reducing bounce rate
Here are some tips to reduce bounce rate:

1. Improve page load time: A slow website can lead to higher bounce rates. You can improve page load time by optimizing images, using a content delivery network (CDN), and lazy loading images.
2. Make your website mobile-friendly: More than half of all internet traffic comes from mobile devices. If your website is not mobile-friendly, you could be losing potential customers.
3. Use **clear calls-to-action**: Make it clear what you want users to do on your website. Use clear calls-to-action (CTAs) to guide users through your site.
4. Improve content readability: Use headings, bullet points, and short paragraphs to make your content easy to read.
5. Use high-quality images: High-quality images can help make your website more visually appealing and engaging.
6. Optimize for search engines: Optimizing your website for search engines can help drive more traffic to your site and reduce bounce rates.

## General SEO Tips
1. Use keywords: Use relevant keywords throughout your website, including in your page titles, meta descriptions, and content.
2. Optimize your images: Use descriptive file names and alt tags for your images.
3. Improve page load time: A slow website can hurt your search engine rankings. You can improve page load time by optimizing images, using a content delivery network (CDN), and lazy loading images.
4. Use internal linking: Link to other pages on your website to help search engines understand the structure of your site.
5. Create high-quality content: High-quality content can help improve your search engine rankings and keep users engaged on your site.

## Browser Caching vs Cookies vs Elasticache 
Browser Caching, Cookies, and Elasticache are different mechanisms used in web development to improve performance and enhance user experience. Let's discuss each of them briefly:

1. Browser Caching:
Browser caching is a technique used to store static web resources, such as HTML files, CSS stylesheets, JavaScript files, and images, on the user's device. When a user visits a website, these resources are downloaded and stored in the browser cache. On subsequent visits, the browser can fetch the resources from the cache instead of re-downloading them from the server, resulting in faster page load times.
Browser caching is achieved by setting appropriate HTTP headers, such as Cache-Control and Expires, which instruct the browser on how long it can cache the resources. By leveraging browser caching effectively, web developers can reduce the number of server requests and improve website performance.

2. Cookies:
Cookies are small text files stored on the user's device by websites they visit. They are primarily used to store user-specific data, such as login information, preferences, and shopping cart contents. Cookies allow websites to remember user actions and provide personalized experiences.
Cookies are sent between the browser and the server with each request, allowing the server to identify and recognize the user. They can be used for session management, user tracking, and targeted advertising. However, it's important to handle cookies with caution to respect user privacy and comply with relevant regulations, such as GDPR.

3. Elasticache:
Elasticache is a web service provided by Amazon Web Services (AWS) that offers a fully managed in-memory caching system. It is designed to improve the performance and scalability of web applications by offloading frequently accessed data from the backend database.
Elasticache supports two widely used caching engines: Memcached and Redis. By storing data in memory, Elasticache reduces the need to fetch data from the database, resulting in faster response times and reduced load on the database.

Elasticache is often used in scenarios where quick access to cached data is critical, such as session management, frequently accessed database queries, and storing precomputed results. It can be seamlessly integrated with various web applications hosted on AWS.

In summary, browser caching improves website performance by storing static resources on the user's device, cookies store user-specific data, and Elasticache provides an in-memory caching system to accelerate data access and reduce backend load. Each of these mechanisms plays a different role in web development and can be leveraged based on specific requirements and use cases.

## Storage types in browser
1. Storage Capacity:
LocalStorage: LocalStorage provides a larger storage capacity compared to cookies. It typically allows storing around 5-10MB of data per origin (website domain).
Cookies: Cookies have a much smaller storage capacity compared to LocalStorage. Each cookie can store only up to 4KB of data, and there is usually a limit of 20-50 cookies per domain.

2. Data Persistence:
LocalStorage: Data stored in LocalStorage persists even after the browser is closed and reopened. The data remains available until explicitly cleared by the user or through programmatic removal.
Cookies: Cookies can have an expiration date/time set, making them either session cookies (deleted when the browser session ends) or persistent cookies (remain until their expiration date). This allows cookies to retain data across different sessions.

3. Automatic Data Transmission:
LocalStorage: Data stored in LocalStorage is not automatically transmitted to the server with each request. It remains on the client-side and can be accessed or manipulated by JavaScript on the same domain.
Cookies: Cookies are automatically transmitted to the server with each request made to the same domain. This allows the server to read and utilize the cookie data, making cookies suitable for scenarios like session management and user tracking.

4. Accessibility:
LocalStorage: Data stored in LocalStorage is accessible only by the web application running on the same domain. Other websites or scripts cannot access or modify this data due to the "same-origin policy" enforced by browsers.
Cookies: Cookies can be accessed by both the web application that created them and any other scripts running on the same domain. This accessibility allows for scenarios like third-party integrations or analytics tracking.

5. Security Considerations:
LocalStorage: LocalStorage is generally considered more secure than cookies since it is not automatically transmitted to the server and is not susceptible to Cross-Site Scripting (XSS) attacks through HTTP-only flags.
Cookies: Cookies can have the HTTP-only flag set, which prevents client-side JavaScript from accessing the cookie. This provides additional security against XSS attacks. However, cookies are vulnerable to **Cross-Site Request Forgery** (CSRF) attacks if not properly secured.

In summary, LocalStorage provides larger storage capacity and persists data across browser sessions, while cookies have a smaller storage capacity but are automatically transmitted to the server and can be accessed by both the web application and other scripts. The choice between LocalStorage and cookies depends on factors such as data size, persistence requirements, security considerations, and whether the data needs to be transmitted to the server with each request.

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