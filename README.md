# LanSync

## Linux Utility for Transferring Files within a Local Area Network (LAN)

LanSync is a Linux-based file transfer utility developed in C++ using TCP socket programming.
The project enables file sharing between systems connected within the same Local Area Network (LAN) through a client-server architecture.

The sender connects to the receiver using an IP address and port number and transfers files securely over TCP sockets.

---

## Features

* File transfer within LAN
* TCP socket-based communication
* Client-server architecture
* Linux-compatible implementation
* Console-based interface
* Modular C++ project structure
* Basic logging support

---

## Tech Stack

* C++
* Linux
* TCP/IP Sockets
* Object-Oriented Programming (OOP)
* Git & GitHub

---

## Project Structure

```bash
src/
└── console/
    ├── Console.cpp
    ├── Console.hpp
    │
    ├── Logger/
    │   ├── BaseLogger.cpp
    │   ├── BaseLogger.hpp
    │   ├── ConsoleLogger.cpp
    │   └── ConsoleLogger.hpp
    │
    ├── networks/
    │   ├── LinuxSockets.cpp
    │   └── LinuxSockets.hpp
    │
    └── exceptions/
        └── Exceptions.hpp
```

---

## How It Works

### Sender

* Connects to receiver using IP address and port
* Sends files through TCP connection

### Receiver

* Waits for incoming connection
* Receives and stores transferred files

---

## How to Run

### Clone Repository

```bash
git clone <your-repo-link>
cd LanSync
```

### Compile

```bash
g++ src/console/*.cpp \
src/console/Logger/*.cpp \
src/console/networks/*.cpp \
-o app
```

### Run Receiver

```bash
./app receive <port> <number-of-files>
```

Example:

```bash
./app receive 8080 1
```

### Run Sender

```bash
./app send <receiver-ip> <receiver-port> <file>
```

Example:

```bash
./app send 127.0.0.1 8080 sample.txt
```

---

## Learning Outcomes

This project helped in understanding:

* Socket Programming
* TCP/IP Communication
* Linux Networking
* File Handling in C++
* Client-Server Architecture
* Header and Source File Management
* Debugging and Dependency Handling

---

## Future Improvements

* Multi-client support
* File encryption
* Authentication system
* File compression
* Progress tracking
* GUI support

---

## Author

Nirjana Das
