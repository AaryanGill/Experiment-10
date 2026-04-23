# WEBSOCKET-CHAT-APP

A full-stack real-time chat application built using React and Spring Boot, demonstrating WebSocket-based communication with STOMP protocol.

## Overview

This project is a hands-on implementation of real-time communication using WebSockets. It showcases:

- User-to-user real-time messaging
- WebSocket connection using SockJS and STOMP
- Live UI updates without page refresh
- Frontend-backend integration (React + Spring Boot)
- Event-driven communication system

---

## Technology Stack

- **Frontend:** React (Vite)
- **Backend:** Spring Boot
- **Protocol:** WebSocket + STOMP
- **Libraries:** SockJS, STOMP.js
- **Build Tools:** Maven, npm

---

## Project Structure

```
src/
Experiment-10/
│
├── my-app/                 # React Frontend
│   ├── src/
│   │   ├── components/
│   │   │   ├── Chat.jsx
│   │   │   ├── MessageInput.jsx
│   │   │   └── MessageList.jsx
│   │   ├── App.jsx
│   │   ├── main.jsx
│   │   └── index.css
│   └── package.json
│
├── Demo_WebSocket/         # Spring Boot Backend
│   ├── src/main/java/
│   ├── src/main/resources/
│   └── pom.xml

```

## Features

- ✅ Real-time messaging
- ✅ WebSocket connection using SockJS + STOMP
- ✅ Broadcast messages to all connected users
- ✅ Username-based communication
- ✅ Dynamic UI updates (no refresh required)
- ✅ Clean and simple interface

---


## Getting Started

### Prerequisites

- Node.js (v16+)
- Java 17+
- Maven 3.6+

### Installation & Running

1. **Clone the repository:**
git clone https://github.com/AaryanGill/Experiment-10.git
cd Experiment-10

2. **Run the backend:**
cd Demo_WebSocket
mvn spring-boot:run

The backend will start on:

http://localhost:8080

3. **Run the frontend:**
cd my-app
npm install
npm install sockjs-client @stomp/stompjs
npm run dev

The frontend will start on:

http://localhost:5173

- **API / WebSocket Endpoints**
- **WebSocket Flow**
- **Server broadcasts messages to all clients**


## Key Components
- **Chat.jsx →** Manages WebSocket connection and subscriptions
- **MessageInput.jsx →** Handles user input and sending messages
- **MessageList.jsx →** Displays messages dynamically


## **Configuration**

- ✅ Vite Fix
define: {
  global: 'globalThis',
} 

- ✅ main.jsx Fix
import { Buffer } from "buffer";
import process from "process";

window.global = window;
window.Buffer = Buffer;
window.process = process;

- ✅ Usage Example
- ✅ Open multiple browser tabs
- ✅ Enter usernames
- ✅ Start chatting
- ✅ Messages appear instantly across all clients


### Screenshots

### 1️⃣ Chat Interface

Add your screenshot here

### 2️⃣ Real-Time Messaging

Multiple users chatting simultaneously

### 3️⃣ WebSocket Connection Active

Show connection logs or console

### 4️⃣ Message Broadcast

Display messages received across clients

### 5️⃣ Application Running

Show backend + frontend running

### Learning Outcomes

- Learned how WebSockets enable real-time communication
- Implemented STOMP protocol for messaging
- Integrated React frontend with Spring Boot backend
- Built real-time UI updates without refresh


### 👨‍💻 Author

**Aaryan Gill** – 23BAI70473

Email: 23BAI70473@cuchd.in
GitHub: https://github.com/aaryangill
