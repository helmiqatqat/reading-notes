# Message Queues

## Socket.io Chat Example

**Explain to a non-technical recruiter what the Chat Example (above) does.**

- It uses a realtime service to make users connected to the same server interact with each other.

**What proof of life are we getting on the backend from the above app?**

- The console.log messages.

**Socket.IO gives us the i0.emit() method to send an event to everyone. What flag would you use if you want to send a message to everyone except for a certain emitting socket?**

- broadcast flag.

## Rooms

**What is a room and how might a room be useful?**

- A room is an arbitrary channel that sockets can join and leave. It can be used to broadcast events to a subset of clients.

**How do you join a room?**

- socket.join(...) 

**How do you leave a room?**

- socket.leave(...) 

## Namespaces

**What is a Namespace and what does it allow you to do?**

- A Namespace is a communication channel that allows you to split the logic of your application over a single shared connection (also called "multiplexing").

**Each namespace potentially has its own what? (hint: 3 things)**

- Rvent handlers.
- Rooms.
- Middlewares.

**Discuss a possible use case for separate namespaces**

- You want to create a special namespace that only authorized users have access to, so the logic related to those users is separated from the rest of the application

- Your application has multiple tenants so you want to dynamically create one namespace per tenant