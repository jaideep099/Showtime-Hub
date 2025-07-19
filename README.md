# Showtime-Hub
A movie show platform with booking and movie exploration features. Tech Stack: MERN (MongoDB, Express.js, React.js, Node.js) Key Features:  Movie search, booking system, and user profiles  State management using Context API  Scalable MongoDB schema for users, movies, and bookings
# 🎬 BookMyShow Backend API

This is the backend of a simple **Movie Ticket Booking API** using **Node.js**, **Express.js**, and **MongoDB**. It supports movie slot selection, seat reservation, and viewing the last booked ticket.

---

## 🚀 Features

- 🎟️ Create a movie ticket booking
- 📋 Retrieve the latest booking
- 🌐 CORS enabled for cross-origin requests
- 🧩 Modular routing and MongoDB schema

---

## 🛠️ Tech Stack

- **Node.js**
- **Express.js**
- **MongoDB** (with Mongoose)
- **CORS**
- **Nodemon** (for development)

---

## 📁 Project Structure

```
├── dbConnection.js      # MongoDB connection logic
├── schema.js            # Mongoose schema for ticket data
├── routes.js            # API routes (POST and GET for bookings)
├── server.js            # Server setup and middleware configuration
├── package.json         # Dependencies and scripts
```

---

## 📦 Installation

```bash
# Clone the repository
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

# Install dependencies
npm install
```

---

## 🧪 Usage

### Start the server

```bash
npm start
```

Server will run at: `http://localhost:8080`

---

## 📡 API Endpoints

### POST `/api/booking`

Create a new booking.

**Request Body:**

```json
{
  "movie": "Inception",
  "slot": "6:00 PM",
  "seats": {
    "A1": 1,
    "A2": 1,
    "A3": 0,
    "A4": 0,
    "D1": 0,
    "D2": 0
  }
}
```

---

### GET `/api/booking`

Get the last booking details.

**Example Response:**

```json
{
  "data": {
    "_id": "...",
    "movie": "Inception",
    "slot": "6:00 PM",
    "seats": {
      "A1": 1,
      "A2": 1,
      "A3": 0,
      "A4": 0,
      "D1": 0,
      "D2": 0
    }
  }
}
```

---

## 🔌 MongoDB Configuration

Ensure MongoDB is running locally on:

```
mongodb://127.0.0.1:27017/bookMyShow
```

To change this, update the connection string in `dbConnection.js`.

---



