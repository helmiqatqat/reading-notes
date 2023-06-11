# Code 401 - Reading Class - 02

## ES6 Classes

**Classes are a template for creating ____.**

- Objects.

**Can a class declaration be hoisted?**

- Unlike function declarations, class declarations are not hoisted.

**How would you describe a constructor and contextual “this” to a non-technical friend?**

- Constuctor is like a chief you give him ingredients and he creates a recipe, 'this' is what the cheff use to define the name of the ingredient.

## Using Express Routing

**Within Express, what does routing refer to?**

- Routing in Express refers to how an application’s endpoints (URIs) respond to client requests.

**What is the difference between a route path and a route method?**

- A route path is a string or a pattern that defines the endpoints at which requests can be made. A route method is an HTTP method such as GET, POST, PUT, DELETE, etc. that is used to handle requests made to the server

**When is it appropriate to add next as a parameter to a route handler and what must you do if next has been passed to your middleware as a parameter?**
When there is a middleware function it is appropriate to add next as a parameter, if next has been passed to the middleware as a parameter, we should call it at the end of the middleware function so that control can be passed to the next middleware function in the stack.

## Express Routing

**What is an Express Router?**

- It is a class to create modular, mountable route handlers. A Router instance is a complete middleware and routing system; for this reason, it is often referred to as a “mini-app”.

**By what mean do we initialize express.Router() in an express server?**

- We initialize express.Router() by creating an instance of it using const router = express.Router(), which returns a new Router object that we can use to define our routes.

**What do we use route middleware for?**

- Authentication, Authorization, Logging, Request Parsing and Data Transformation, Error Handling and Request Validation.
