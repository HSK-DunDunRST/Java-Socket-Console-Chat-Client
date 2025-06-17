# Java Socket Console Chat Client

## Introduction

This project is a console-based chat client implemented using Java socket programming. Users can connect to a chat server and exchange messages in real time. Each client handles message sending and receiving in separate threads to ensure stable operation in a multithreaded environment.

## Features

- **Chat Client**: Connects to a server to send and receive messages
- **Multithreading**: Handles reading and writing messages in independent threads
- **Real-time Messaging**: Exchanges messages with the server in real time
- **Simple Console UI**

## Project Structure

```
src/
  main/
    java/
      com/
        hsk/
          socket/
            chat/
              client/
                Main.java
                ReadThread.java
                WriteThread.java
```

- **Main.java**: Entry point for running the client
- **ReadThread.java**: Receives messages from the server
- **WriteThread.java**: Sends messages to the server

## Build & Run

### Requirements

- Java 17 or higher
- Maven 3.x or higher

### Build

```sh
mvn clean package
```

### Run

```sh
java -cp target/Java-Socket-Console-Chat-Client-1.0-SNAPSHOT.jar com.hsk.socket.chat.client.Main
```

## Usage

1. Make sure the server is running.
2. Start the client to connect to the server.
3. Type messages in the console to send them to other users via the server.
4. Incoming messages from the server will be displayed in real time.

## Future Improvements

- Provide a GUI-based client
- Add chat room features and message storage (DB integration)
- Implement client authentication and user management

---

## License

MIT License
