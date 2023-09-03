# API Integration

## Review API Server Build

**Explain the different between a query string parameter and a path parameter.**

- path parameter is prefixed by '/'.
- query parameter is prefixed by ?.

```URL
/pathParam?queryParam=value'
```

**What would our API URL with a path id parameter be given the following information:**

```bash
Domain: http://our-site.com
v3
model name: stuff
id: things
```

```url
http://our-site.com/v3/stuff/things
```

**We have created a dynamic API with an “interface”. Describe how that interface works to a non-technical friend.**

Let's say we are in a resturant driveway where we order food, the driver speaks to the machine to place orders and the kitchen recieves that order and start working on it, then eventually the driver gets his meal. The driver here is the client who sends http requests, the machine is interface that recieves that http request and send it to the server and take the result to deliever it to the client, the kitchen is the server that handles the requests.

## Review Auth Server Build

**Describe how you would use middleware to implement basic and bearer auth.**

- Basic (username + password) to be used on the /signin route only
- Bearer (token) to be used on any other route in the server that requires a logged in user

**Describe the handshake necessary to implement OAuth.**

- The OAuth processes is initiated in the browser, using a 3rd party authentication/authorization service. It will, once the user has granted permission, invoke a GET on your /oauth route. The OAuth middleware should at this point complete the handshaking process, create/update a local user account in our database, and return an object with a re-authentication/bearer token and the user object

**Describe how Role Based Access Control works to a non-technical friend.**

- Assume you are in a company where it has fingerprint access to each section, assuming you are a normal employee you can enter the company doors freely because you work here, you are authorized to enter the building, but assuming you want to go to the room where confidentional data for the company exists, there is a fingerprint machine on the door, if you put your finger, it will give you "access denied" because you are not allowed to enter there because you are a normal employee, but your boss can enter there, this is basically the RBAC, each role gives capabilites and authorities to the user holding that role.
