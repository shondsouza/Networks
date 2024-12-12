# UDP Client-Server Chat Application

This is a simple UDP-based client-server chat application built in Java. The application demonstrates basic communication between a UDP client and a UDP server using datagram sockets. The server listens for messages from the client, processes them, and sends a modified response back to the client.

## Features

- **UDP Client**: Sends a message to the server and waits for a response.
- **UDP Server**: Receives the message, processes it (converts to uppercase), and sends it back to the client.
- **Real-time Message Display**: The client displays the message from the server in real-time.

## Prerequisites

- Java Development Kit (JDK) 8 or higher.
- A basic understanding of UDP (User Datagram Protocol) and socket programming in Java.

## Files

- `UDPServer.java`: The server code which listens on port 9876 for incoming client messages and sends back the uppercase version of the message.
- `UDPClient.java`: The client code which sends a message to the server and waits for the response.

## How to Run

### 1. Compile the Java Files
Navigate to your project folder and compile both the client and server files:

```bash
javac UDPServer.java
javac UDPClient.java
```

### 2. Run the Server
Start the server in one terminal window:

```bash
java UDPServer
```

The server will start and wait for messages from the client.

### 3. Run the Client
In another terminal window, start the client:

```bash
java UDPClient
```

The client will prompt you to enter a string. After entering a message, it will send the message to the server, which will return the message in uppercase.

### 4. Example

**Client Side**:
```
Enter the string to be converted into Uppercase: Hello, UDP!
```

**Server Side**:
```
Server is Up
RECEIVED: Hello, UDP!
```

**Client Side**:
```
FROM SERVER: HELLO, UDP!
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

Feel free to fork this repository, make changes, and open pull requests. Contributions are always welcome!

## Acknowledgments

- Java Documentation for DatagramSocket and DatagramPacket classes.
- Open-source community for making learning easy!
