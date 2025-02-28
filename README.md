# 🔒 Encrypted Chat

A chat application with **End-to-End Encryption (E2EE)** built in **Python**, using **Sockets** and **SSL** for secure communication between client and server.

---

## 🚀 Features

- 🔐 **SSL Encryption** to secure communications.
- 🧵 **Multithreading support** to handle multiple clients simultaneously.
- 📜 **Graphical User Interface (GUI)** using Tkinter for the client.
- 📢 **Public message broadcasting**.
- 👥 **Command to list connected users**.
- ❌ **Handles client disconnections gracefully**.

---

## 🛠️ Installation & Execution

### 1️⃣ Clone the repository

```bash
git clone git@github.com:FJLdx/encrypted-chat.git
cd encrypted-chat
```

### 2️⃣ Generate SSL Certificates

Before starting, generate SSL certificates to establish a secure connection:

```bash
openssl req -x509 -newkey rsa:4096 -keyout server-key.key -out server-cert.pem -days 365 -nodes
```

This will generate two files:
- `server-key.key`: Server private key.
- `server-cert.pem`: Public certificate.

### 3️⃣ Run the Server

```bash
python3 server.py
```

### 4️⃣ Run the Client

```bash
python3 client.py
```

You will be prompted for a username, and a chat window will open with the following options:
- **Write and send messages**.
- **List connected users** using the `List users` button.
- **Exit the chat** using the `Exit` button.

---

## 🖥️ Usage

1️⃣ Start the **server** before any clients.
2️⃣ Open multiple **clients** in different terminals or machines.
3️⃣ Enter a username when prompted.
4️⃣ Start chatting securely! 🔏

### 📜 Available Commands

| Command      | Description                      |
|-------------|----------------------------------|
| `!usuarios` | Displays connected users.       |

---

## 📜 Source Code

The source code is divided into:

- `server.py` → Chat server.
- `client.py` → Client with GUI.
- `server-cert.pem` → Server SSL certificate.
- `server-key.key` → Server private key.
- `server.csr` → Certificate signing request.

---

## 📜 License

This project is under the **MIT License**, allowing unrestricted use, modification, and distribution.

📌 **Developed by [FJLdx](https://github.com/FJLdx)**


