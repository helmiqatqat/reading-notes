# Socket.io

## Web Sockets

**What is a Web Socket?**

- WebSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection. 

**Describe the Web Socket request/response handshake and what happens once the connection is established.**

- To establish a WebSocket connection, the client sends a WebSocket handshake request, for which the server returns a WebSocket handshake response, The handshake starts with an HTTP request/response, allowing servers to handle HTTP connections as well as WebSocket connections on the same port. Once the connection is established, communication switches to a bidirectional binary protocol which does not conform to the HTTP protocol.

**Web Sockets provide a standardized way for the server to send content to a client without first receiving a ____ from that client.**

- request.

## Socket.io Tutorial

**What does the event handler io.on() do?**

- Listens for events

**Describe some possible proof of life or proof that the code works as expected**

- Establishing a Connection: You can verify the code by ensuring that the client can successfully establish a connection with the server using Socket.IO. This involves checking if the handshake process occurs correctly and the connection is established without errors.

- Emit and Receive Events: Socket.IO facilitates real-time communication between the client and server through events. You can emit events from the client and verify if the server receives them correctly, or vice versa. This can include sending messages, broadcasting data, or triggering specific events.

- Implementing Acknowledgments: Socket.IO supports acknowledgments, which allow you to receive a confirmation that an event was received and processed by the recipient. By implementing acknowledgments in your code, you can ensure that events are acknowledged properly, providing evidence of the expected behavior.


**What does socket.emit() do?**

- fires the event.

## Socket.io vs Web Sockets

**What is the difference between WebSocket and Socket.IO? (think Git and GitHub, or OAuth and Auth0).**

- WebSocket is the communication Protocol that provides bidirectional communication between the Client and the Server over a TCP connection; WebSocket remains open all the time, so they allow real-time data transfer. When clients trigger the request to the server, it does not close the connection on receiving the response; it rather persists and waits for the Client or server to terminate the request.

- Socket.IO is a library that enables real-time and full-duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface. Generally, it is divided into two parts; both WebSocket vs Socket.io are event-driven libraries.

**When would you use Socket.IO?**

- Cross-Browser Compatibility: Socket.IO is a library built on top of WebSocket that provides a higher-level API and handles various browser inconsistencies and fallback mechanisms automatically. If you need to ensure seamless cross-browser compatibility and want a consistent API for real-time communication, Socket.IO simplifies the development process.

- Real-Time Applications: If you're building a real-time application that requires instant updates and interactive features, Socket.IO offers additional features like event-driven communication, broadcasting to multiple clients, room management, and automatic reconnection. It provides a robust and feature-rich framework that simplifies the development of real-time applications.

- Scalability: Socket.IO includes features like load balancing and horizontal scaling to handle large numbers of concurrent connections. It allows you to distribute the workload across multiple servers, making it suitable for applications that require high scalability and can handle a large user base.

- Ease of Use: Socket.IO offers a simple and intuitive API that abstracts the complexities of WebSocket communication. It provides convenient features like event handling, room management, and built-in error handling. If you value ease of use and rapid development, Socket.IO can be a good choice.

**When would you use WebSockets?**
- Low-Level Control: WebSocket provides a low-level protocol for establishing a persistent connection between a client and a server. It offers a raw and minimalistic communication channel, allowing you to have more control over the data exchange. If you require fine-grained control over the communication protocol and want to implement specific features from scratch, WebSocket can be a good choice.

- Custom Implementations: WebSocket is ideal when you need to develop a custom real-time communication solution tailored to your specific requirements. It allows you to design and implement the protocol and the corresponding server-side and client-side code from the ground up.

- Efficiency: WebSocket is generally considered more efficient in terms of performance and resource usage compared to higher-level frameworks like Socket.IO. If you have strict performance requirements or need to minimize overhead, WebSocket can be a suitable option.