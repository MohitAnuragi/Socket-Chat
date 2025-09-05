# Cross-Platform Socket Chat Application

## Description

A simple **client-server chat application** built in **C++**, supporting **both Linux and Windows** platforms.  
The project demonstrates how to use **sockets** for real-time communication while handling cross-platform differences with conditional compilation.  

Both the **client** and **server** can send and receive messages until either side types `exit`.  

---

## Table of Contents

- [Features](#features)  
- [Installation](#installation)  
- [Tech Stack](#tech-stack)  
- [Demo](#demo)  
- [Usage](#usage)  
- [Contact](#contact)  

---

## Features

- 🌍 Cross-platform: Works on **Windows** and **Linux**  
- 💬 Real-time **two-way chat** between client and server  
- 🔌 Handles **graceful disconnection** on `exit`  
- 🖥️ Simple **command-line interface**  
- ⚡ Demonstrates **Winsock (Windows)** and **POSIX sockets (Linux)**  

---

## Installation

### Linux / macOS
```bash
# Clone the repo
git clone https://github.com/MohitAnuragi/Socket-Chat.git
cd Socket-Chat

# Compile server & client
g++ server.cpp -o server
g++ client.cpp -o client

# Run in separate terminals
./server
./client

```
### Windows (MinGW / MSVC)
```bash
# Clone the repo
git clone https://github.com/MohitAnuragi/Socket-Chat.git
cd Socket-Chat

# Compile with Winsock library
g++ server.cpp -o server.exe -lws2_32
g++ client.cpp -o client.exe -lws2_32

# Run in separate terminals (CMD/PowerShell)
server.exe
client.exe
```
## Tech Stack

1. C++

2. POSIX sockets (Linux/macOS)

3. Winsock2 (Windows)

## Demo

      +-------------------+              +-------------------+
      |                   |              |                   |
      |      CLIENT       |              |      SERVER       |
      |                   |              |                   |
      +---------+---------+              +---------+---------+
                |                                |
                |   Connect (TCP, port 8080)     |
                +------------------------------->|
                |                                |
                |   Connection accepted          |
                |<-------------------------------+
<img width="1808" height="465" alt="image" src="https://github.com/user-attachments/assets/e7b04ed2-9469-4fd4-9de1-693baea748f1" />

## Usage

1. Start the server first (./server or server.exe).

2. Run the client (./client or client.exe).

3. Exchange messages between client and server.

4. Type exit to close the connection gracefully.

## Contact

Author: Mohit Anuragi

Email: anuragimohit468@gmail.com

LinkedIn: [linkedin.com/in/yourprofile](https://www.linkedin.com/in/mohit-a-52989b2b2)

GitHub: [github.com/MohitAnuragi](https://github.com/MohitAnuragi/)
