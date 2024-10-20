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
