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


<img width="463" height="468" alt="image" src="https://github.com/user-attachments/assets/b3c1b952-24b8-4034-9be3-667b411ba1f2" />


### 2️⃣ Real-Time Messaging


<img width="475" height="385" alt="image" src="https://github.com/user-attachments/assets/9758c216-789f-4e89-ac83-e3afb4680256" />


### 3️⃣ WebSocket Connection Active


<img width="1035" height="616" alt="image" src="https://github.com/user-attachments/assets/ea54f86c-058a-4277-aa1b-5f1b488723de" />


### 4️⃣ Message Broadcast

Display messages received across clients

### 5️⃣ Application Running


<img width="1364" height="712" alt="image" src="https://github.com/user-attachments/assets/0626df5f-a852-4b7b-832a-37196a5c25ca" />


### Learning Outcomes

- Learned how WebSockets enable real-time communication
- Implemented STOMP protocol for messaging
- Integrated React frontend with Spring Boot backend
- Built real-time UI updates without refresh


### 👨‍💻 Author

**Aaryan Gill** – 23BAI70473

Email: 23BAI70473@cuchd.in
GitHub: https://github.com/aaryangill
