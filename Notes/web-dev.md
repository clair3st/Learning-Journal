## REST
*Resource:*[microsoft](https://learn.microsoft.com/en-us/azure/architecture/best-practices/api-design)

*What does REST stand for?*
Representational State Transfer

*REST APIs are designed around a ____.*
resources (objects, data or service that can be accessed by a client)

*What is an identifier of a resource? Give an example.*
URI that uniquely identifies a resource. e.g. `https://cities/usa/seattle`

*What are the most common HTTP verbs?*
GET, POST, PUT, PATCH, DELETE

*What should the URIs be based on?*
Business entities, for example users, orders

*What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?*
An API that expose a large number of small resources, it creates a bigger load on the server

*What status code does a successful GET request return?*
200

*What status code does an unsuccessful GET request return?*
404

*What status code does a successful POST request return?*
201

*What status code does a successful DELETE request return?*
204

## Functional Programming
*Resource:*[Medium](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

*What is functional programming?*
Functional Programming is a programming paradigm, a style of builing structure and elements of a program. It avoids changing state and mutable data.

*What is a pure function and how do we know if something is a pure function?*
A function that returns the same result if given the same arguments. It does not cause any side effects
For example a function that makes use of a global variable is not ture, the global variable can change, this will affect the output of the function.

*What are the benefits of a pure function?*
Makes testing easier

*What is immutability?*
The data's state can't be changed after its created. Instead you have to create a new copy

*What is Referential transparency?*
pure functions and immutable data create referential transperancy


## No SQL vs SQL
*Resource:* [SQL vs NoSQL](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

*List 5 differences between SQL and noSQL databases*

| SQL  | NoSQL |
| ------------- | ------------- |
| Relational Database  | Non-Relational Database |
| Table Based  | Document based  |
| Predefined Schema | Dynamic Schema  |
| Vertically Scalable | Horizontally scalable |

*What kind of data is a good fit for an SQL database?*
Those that require complex queries, datasets that aren't too large, and those that aren't hierarchical

*What kind of data is a good fit a NoSQL database?*
Big datasets, hieracrchical data



