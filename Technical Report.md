# REST
**REpresentational State Transfer** (REST) is a software architectural style that defines the constraints to create web services. 
The web services that follows the REST architectural style is called **RESTful** Web Services. It differentiates between the computer system and web services.
In the REST architectural style, the implementation of the client and the implementation of the server can be done independently without each knowing about the other.
By using a REST interface, different clients hit the same REST endpoints, perform the same actions, and receive the same responses.

![REST](https://raw.githubusercontent.com/Codecademy/articles/0b631b51723fbb3cc652ef5f009082aa71916e63/images/rest_api.svg)
## REST Architectue
REST architecture describe **six** barriers.
* Uniform Interface
* Client-server
* Stateless
* Layered system
* Cacheable
* Code on Demand (optional)

![REST architecture](https://images.javatpoint.com/blog/images/what-is-rest.png)

### 1. Uniform Interface
The Uniform Interface defines the interface between client and server. It simplifies and decomposes the architecture which enables every part to be developed. The Uniform Interface has four guiding principles:
* **Resource-based:** Individual resources are identified using the URI as a resource identifier. The resources themselves are different from the representations returned to the customer. For example, the server cannot send the database but represents some database records expressed to HTML, XML or JSON depending on the server request and the implementation details.
 **Manipulation of resources by representation:** When a client represents a resource associated with metadata, there is information on the server to modify or delete it.
* **Self-Descriptive Message:** Each message contains enough information to describe how the message is processed. For example, the parser can be specified by the Internet media type (known as the MIME type).
* **As the engine of Hypermedia Application State (HATEOAS):** Customers provide states by query-string parameters, body content, request headers, and requested URIs. The services provide customers with the state by response codes, response headers and body content. It is called hypermedia (hyperlink within hypertext).
* In addition to the above description, HATEOS also means that, where necessary, the object or itself is contained in the linked body (or header) to supply the URI for retrieving the related objects.
* The same interface that any REST services provide is fundamental to the design.

### 2. Client-server
A client-server interface separates the client from the server. For Example, the separation of concerns not having an internal relationship with internal storage for each server to improve the portability of customer's data codes. Servers are not connected with the user interface or user status to make the server simpler and scalable. Servers and clients are independently replaced and developed until the interface is changed.

### 3. Stateless
Stateless means the state of the service doesn't persist between subsequent requests and response. It means that the request itself contains the state required to handle the request. It can be a query-string parameter, entity, or header as a part of the URI. The URI identifies the resource and state (or state change) of that resource in the unit. After the server performs the appropriate state or status piece (s) that matters are sent back to the client through the header, status, and response body.

Example, the data stored in a database. Consider the application state of having data that may vary according to client and request. The resource state is constant for every customer who requests it.

### 4. Layered system
It is directly connected to the end server or by any intermediary whether a client cannot tell. Intermediate servers improve the system scalability by enabling load-balancing and providing a shared cache. Layers can enforce security policies.

### 5. Cacheable
On the World Wide Web, customers can cache responses. Therefore, responses clearly define themselves as unacceptable or prevent customers from reusing stale or inappropriate data to further requests. Well-managed caching eliminates some client-server interactions to improving scalability and performance.

### 6. Code on Demand (optional)
The server temporarily moves or optimizes the functionality of a client by logic that it executes. Examples of compiled components are Java applets and client-side scripts.

## Refernces 
* [Code Academy](https://www.codecademy.com/article/what-is-rest)
* [GeeksforGeeks](https://www.geeksforgeeks.org/why-rest-api-is-important-to-learn/)
* [JavaTpoint](https://www.javatpoint.com/what-is-rest)
