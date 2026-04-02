# 📹 Elderly AI Companion – Video Calling Module

A real-time video calling system designed to connect elderly users with caregivers, family members, or emergency contacts — built using modern web technologies for **low latency, simplicity, and reliability**.

---

## 🚀 Overview

This module enables **seamless peer-to-peer video communication** within the Elderly AI Companion ecosystem.

It ensures that in moments of need, users can:

* Instantly connect with loved ones
* Receive visual assistance
* Feel safe and supported

---

## ✨ Key Features

### 📞 Real-Time Video Calling

* Peer-to-peer communication using WebRTC
* Low latency and high-quality video/audio

---

### 🔗 Unique Room-Based Calling

* Users can create/join rooms using a Room ID
* Simple and intuitive connection flow

---

### 🎤 Audio + Video Controls

* Toggle microphone
* Enable/disable camera
* Mute/unmute easily

---

### ⚡ Fast Signaling with Socket.IO

* Real-time exchange of:

  * Offer / Answer
  * ICE Candidates
* Ensures quick connection setup

---

### 🧓 Elderly-Friendly Design

* Large buttons
* Minimal UI complexity
* One-click call experience

---

## 🏗️ Tech Stack

### Frontend

* React.js
* WebRTC API
* Socket.IO Client

### Backend (Signaling Server)

* Node.js
* Express.js
* Socket.IO

---

## 📂 Project Structure

```id="q7t6hb"
video-call/
 ├── frontend/
 │   ├── src/
 │   │   ├── App.js
 │   │   ├── VideoCall.js
 │   │   ├── Controls.js
 │   │   └── socket.js
 │
 ├── backend/
 │   ├── server.js
```

---

## ⚙️ Setup Instructions

### 1️⃣ Clone Repository

```bash id="7y1lrf"
git clone <your-video-call-repo-url>
cd video-call
```

---

### 2️⃣ Backend Setup (Signaling Server)

```bash id="o3w0ha"
cd backend
npm install
node server.js
```

Server runs on:

```id="c8ubfi"
http://localhost:5000
```

---

### 3️⃣ Frontend Setup

```bash id="k6c2jr"
cd frontend
npm install
npm start
```

App runs on:

```id="ixx9q1"
http://localhost:3000
```

---

## 🔄 How It Works

1. User opens the app

2. Creates or joins a **room ID**

3. Frontend captures:

   * Camera stream
   * Microphone stream

4. WebRTC flow:

   * Offer → Answer
   * ICE candidate exchange

5. Direct peer-to-peer connection established

6. Live video + audio begins

---

## 🔌 Core Concepts Used

### 🧠 WebRTC

* Enables direct browser-to-browser communication
* No need for heavy media servers

---

### 🔄 Signaling (Socket.IO)

* Used to exchange connection metadata
* Not used for actual video streaming

---

### 🌐 STUN Servers

* Helps devices discover public IP addresses
* Required for NAT traversal

Example:

```javascript id="4a7zpx"
const pc = new RTCPeerConnection({
  iceServers: [{ urls: "stun:stun.l.google.com:19302" }]
});
```

---

## 🎯 Use Cases

* 👨‍👩‍👧 Family communication
* 🏥 Remote health assistance
* 🚨 Emergency video support
* 🧓 Daily check-ins for elderly

---

## 🔮 Future Enhancements

* 📲 One-tap emergency call
* 🤖 AI-triggered auto video call (panic detection)
* 🌐 Multi-user group calls
* 📡 Screen sharing for doctor consultations
* 🔒 End-to-end encryption

---

## 🏆 Why This Matters

Elderly individuals often struggle with:

* Loneliness
* Lack of immediate support
* Difficulty using complex apps

This module ensures:

* **Human connection in one click**
* **Visual reassurance in emergencies**
* **Simple and accessible communication**

---

## 🤝 Contributing

Feel free to fork, improve, and submit pull requests.

---

## 📜 License

MIT License

---

## 💡 Final Note

Technology should not feel complicated — especially for those who need it the most.

This video calling system is built to be:
**Simple. Fast. Human.**
