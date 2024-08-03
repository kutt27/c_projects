## Steps to Implement

**Setup the Server**:

- Create a socket.
- Bind it to an address and port.
- Listen for incoming connections.
- Accept connections from clients.

**Handle Multiple Clients**:

- Use threads or select/poll to manage multiple client connections concurrently.
- Each client will have a dedicated handler that can read from and write to the client socket.

**Broadcast Messages**:

- When a message is received from one client, it should be broadcast to all other connected clients.
- Maintain a list of all connected client sockets for broadcasting.

**Client Implementation**:

- Connect to the server socket.
- Send and receive messages from the server.
- Handle the display of incoming messages and user input simultaneously.
