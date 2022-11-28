# Understanding SQL Injection, Identification and Prevention

Standardized query language (SQL) is still the dominant method of inserting, filtering and retrieving information from a database. It’s not usually regarded this way, but SQL is a full programming language unto itself. With some basic SQL knowledge and an internet connection, an attacker can exploit flaws in a web application – extracting user data, discovering or resetting credentials and using it as a launch point for deeper assaults on the network.

SQL commands are used to Create, Read, Update and Delete (CRUD) the information inside of database tables. Most web applications and frameworks revolve around these same principles, building out forms to manipulate the underlying data which is stored in the database. It’s important to know these commands as SQL Injection attacks are built upon the notion of altering what you would expect to happen and slipping past your defenses.

Traditionally SQL Injection attacks (which have been around since the invention of the HTML tag) have been the domain of big web applications, but now that that a billion people have gotten online and the development of SQLite as a free portable database: 
Everything has a web configuration interface backed by a database, and everything is susceptible to SQL injection attacks.

Some prevention methods:

Database

Sufficient and appropriate database user permissions set
Extraneous or unused database features disabled
Database logging enabled
Database backup / restore procedure
Database connection filtering procedures enabled (example: MySQL has options to prevent execution of multiple SQL statements in a single query)
Database drivers up to date

Application

Using filtering options
Using parameterization options
Using DB calls only when needed? (Could you use a static site generator?)
Code lint/checks for potential SQL injection points
Manual check for SQL Injection prone points
Application logging

Web Server / Web Firewall

Use WAF SQL Injection pre-filters
Rate limit to prevent mass SQL Injection attempts
Alert on SQL Injection pattern attempts
