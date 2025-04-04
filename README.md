# C++ Chat Application

This is a terminal-based Chat Application built using C++ with socket programming and networking concepts. It enables real-time communication between a server and multiple clients using the TCP protocol.

The current version demonstrates communication between two clients for demo purposes, but the implementation supports multiple clients.

## ✅ Features

- Built using C++ socket programming
- Uses TCP protocol for reliable message delivery
- Terminal-based interface (no GUI)
- Supports multiple clients (demo includes 2 clients)
- Real-time message broadcasting from server to clients

## 🔧 Requirements

- C++ Compiler (like `g++` or `MinGW`)
- Terminal (Linux/macOS or Windows command prompt/PowerShell)
- All machines must be on the **same network**
- **Localhost (127.0.0.1) is not supported**

## ⚙️ How to Compile

### On Linux/macOS

```bash
g++ server/server.cpp -o server
g++ client/client.cpp -o client
g++ client2/client2.cpp -o client2
```

### On Windows

```bash
g++ server\server.cpp -o server.exe
g++ client\client.cpp -o client.exe
g++ client2\client2.cpp -o client2.exe
```

## 🚀 How to Run

### Step 1: Start the Server

Run the server on one machine:

```bash
./server
```

### Step 2: Start the Clients

Run each client on separate machines (or terminals) on the **same network**:

```bash
./client
```

```bash
./client2
```

### Step 3: Connect to Server

Each client will prompt for the server's IP address.  
Enter the server machine’s **local IP address** (e.g., `192.168.x.x`).

### Step 4: Start Chatting

Once connected, clients can chat with each other via the server. Messages are relayed in real-time.

## 📌 Notes

- The code provided is for learning/demo purposes.
- The demo is set up for 2 clients, but the server can handle **multiple clients** with the existing threading logic.
- Ensure firewalls or antivirus do not block the application.
