					SQL Injection, Identification and Prevention

Standardized query language (SQL) is one of the major tools used in the method of inserting, filtering and retrieving information from a database. Loads of SQL queries will be coursing through your web applications on almost every page load regardless of size. With just a web browser and some basic SQL knowledge and an internet connection, an attacker can exploit flaws in your web application – extracting user data, discovering or resetting credentials and using it as a launch point for deeper assaults on your network.

We’re going to get to work our way up to SQL injection attacks and the reason they are scarier than a clown who lives in a drainpipe. But in order to understand injection/vulnerabilities, we need to take a step back and review that basic SQL knowledge first.
 
 							What is SQL?

SQL should not be thought of as a language or tool that is use for getting data out of a database. Limiting its power and complexity directly leads to many of the security issues that occur when you put a web application in front of a SQL database. SQL is a full programming language unto itself and can be used just like any other programming language.

In SQL, query doesn't just mean asking for something like in the real world, we're really diving deep into the database with SQL. In fact, it’s probably better if you start mentally substituting the word “command” every time you hear “query”. In particular if you’re trying to convince an executive or someone about the potential seriousness of SQL Injection attacks, saying: “This flaw lets attackers execute arbitrary commands on our server.” Sounds much more frightening than something that otherwise sounds like: “They can run reports on our data.” It’s natural to think of queries like questions: “Hey, can you throw me that ball?”. However in SQL terms a “query” might be more like: “I’m throwing a 100mph fastball at your head.”

There are many aspect to SQL and further studies will expose the user to as many useful techniques to execute as possible. 

								 
