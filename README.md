# Mini Message Board ✉️

A full-stack, server-rendered message board application built with **Node.js**, **Express**, and **PostgreSQL**. This project follows the **MVC (Model-View-Controller)** architecture and features persistent data storage with robust server-side validation.

## 🚀 Live Demo
**[View Live Demo on Render](https://mini-messaging-board-ur7s.onrender.com)** *(Note: Initial load may take ~50s as the free instance spins up.)*

## ✨ Features
* **Real-time Persistence:** Messages are stored in a cloud PostgreSQL database.
* **Dynamic Routing:** View all messages on the home feed or click individual messages for a detailed view.
* **Input Validation:** Secure form handling using `express-validator` to prevent empty or malicious posts.
* **MVC Pattern:** Clean separation of concerns between database queries, logic controllers, and EJS views.
* **Security:** Implements parameterized SQL queries to protect against SQL injection.

## 🛠️ Tech Stack
* **Backend:** Node.js, Express.js
* **Database:** PostgreSQL (Hosted on Neon DB)
* **Templating:** EJS (Embedded JavaScript)
* **Validation:** Express-Validator
* **Deployment:** Render

## 💻 Run Locally

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/WAnubhavGoel/mini-messaging-board.git](https://github.com/WAnubhavGoel/mini-messaging-board.git)
   cd mini-messaging-board
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Set up Environment Variables:**
   Create a `.env` file in the root directory:
   ```env
   PORT=8080
   DB_CONNECTION_STRING=your_postgresql_connection_string
   ```

4. **Initialize the Database:**
   ```bash
   node db/populatedb.cjs "your_postgresql_connection_string"
   ```

5. **Start the server:**
   ```bash
   npm start
   ```
   The app will run on: `http://localhost:8080`

## 📂 Project Structure
```text
.
├── controllers/      # Request handling & logic
├── db/               # Pool configuration & SQL queries
├── public/           # Static assets (CSS/Images)
├── routes/           # URL routing
├── views/            # EJS templates (UI)
└── app.cjs           # Entry point
```
