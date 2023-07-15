# Technical Paper: REST Architecture

## Abstract
This technical paper gives detailed information on the Representational State Transfer (REST) architecture. It provides the basic REST concepts. The paper provides related information on REST architecture.
## 1. Introduction
REST was introduced in 2000 by Roy Fielding for designing networked applications. After that, it got popularity in web development. REST provides a set of rules and regulations that help in enabling reliable, scalable systems. 
## 2. Fundamental Concepts
REST design and implementation are built upon several fundamental concepts:

### 2.1 Resources
REST resources represent any entity, such as data objects, services, or collections that can be identified. URI tries to identify the resources. URI helps in accessing resources and manipulating them.

### 2.2 Uniform Interface
REST helps in performing the interaction between clients and servers. It helps in communication between the client and server with the help of main components.

#### 2.2.1 Resource Identification
URI tries to locate resources. It provides an improved way to locate or identify resources. There are mainly two parts in URIs that locate the resource that is base URI and path segment.

#### 2.2.2 Resource Manipulation
REST system provides a standard HTTP method to change or edit or manipulate resources. Basically, the methods are GET, POST, PUT, PATCH, and DELETE. Each method has its own work like creating new resources, updating existing resources, and deleting resources.  
#### 2.2.3 Resource Representation
Communication between client and server happened in JSON(JavaScript Object Notation) format or XML (eXtensible Markup Language). The client can request specific representation by specifying desired media type in the HTTP Accept header.

#### 2.2.4 Self-Descriptive Messages
To understand complete syntax each request and response contains all the necessary information. The request and response messages include HTTP headers.

### 2.3 Statelessness
Statelessness is one of the main fundamental properties of REST. It says that whatever the request client made to the server should contain all the required information to process the request. Servers do not maintain any client-specific state between requests. These principles of REST has helped in scalability, reliability, and simplicity in RESTful system.

## 3. REST Constraints
REST gives an instruction set of architectural constraints that tells us how to do design and how to perform implementation. 

### 3.1 Client-Server
The client-server constraints separately handle the concern related to client and server. Basically, This separation provides independent evolution and helps in enhancing scalability between client and server. In other words, the client and server can be handled individually without affecting each other.

### 3.2 Stateless
RESTful systems are stateless. All each request contains all the information required to process it, and servers do not maintain any client-specific state between requests. This constraint improves scalability, as servers can handle requests from any client without requiring session management.

### 3.3 Cacheable
REST helps in reducing server load and in performance by using caching. Responses from servers can be marked as cacheable, allowing clients to cache the response. RESTful this property helps in increasing the overall system and reducing the load on the server.

### 3.4 Layered System
RESTful has a layered system. This contract allows for the deployment of several components such as proxies, gateways, and balancers between clients and servers. These layered systems provide additional functionality such as caching, security, protocol, and translation, without creating disturbance or affecting client-server.

### 3.5 Uniform Interface
The uniform interface constraint ensures consistency and simplicity in interactions between clients and servers. It consists of four components: resource identification, resource manipulation using HTTP methods, resource representation, and self-descriptive messages. This constraint simplifies client-server interactions, promotes reusability, and enables the decoupling of clients and servers.

## 4. Designing RESTful APIs
When designing RESTful APIs, there are several step should be practiced to consider:

- Use nouns to represent resources in the URI.
- Utilize appropriate HTTP methods for resource manipulation.
- Return relevant HTTP status codes for each request.
- Provide a consistent and logical resource hierarchy.
- Support content negotiation to allow clients to specify desired representations.
- Use hypermedia links (HATEOAS) to provide discoverability and navigate between resources.

## 5. Conclusion
REST architecture offers a standardized approach to designing networked applications. By leveraging its fundamental concepts, adhering to constraints, and following best practices, developers can create scalable, reliable, and interoperable systems. Understanding the key concepts and principles of REST is essential for modern web development.

## References
1. Fielding, R. T. (2000). Architectural Styles and the Design of Network-based Software Architectures (Doctoral dissertation). University of California, Irvine.
2. Richardson, L., & Amundsen, M. (2013). RESTful Web APIs: Services for a Changing World. O'Reilly Media.
3. Fielding, R. T. (2008). REST APIs must be hypertext-driven. Retrieved from https://roy.gbiv.com/untangled/2008/rest-apis-must-be-hypertext-driven
