# 🎵 Concert Management System

A full-featured concert event management system built with **Node.js**, **Express**, and **MongoDB**. It includes role-based access control for users and admins, ticket booking, reviews, categories, and more.

## 🚀 Features

- **User & Admin Authentication** (JWT-based)
- **Concert Listings and Bookings**
- **Categories and Subcategories**
- **Concert Reviews**
- **Role-based Routing and Middleware**
- **Modular Architecture (MVC + Service/Repository Pattern)**

## 📁 Project Structure

```
concert-management/
├── config/                # Database & JWT configuration
├── controllers/           # Request handlers for admin and user routes
├── middleware/            # Custom middleware (auth, error handling)
├── models/                # Mongoose schemas (User, Concert, Booking, etc.)
├── repositories/          # Data access layer
├── routes/                # Express route definitions
├── services/              # Business logic
├── utils/                 # Reusable utility functions
├── views/                 # Frontend templates (if applicable)
└── app.js                 # Main application entry point
```

## 🛠️ Tech Stack

- **Backend:** Node.js, Express.js
- **Database:** MongoDB, Mongoose
- **Authentication:** JWT (JSON Web Token)
- **Templating (optional):** EJS or any templating engine
- **Tools:** Postman, Nodemon, Dotenv

## 📦 Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/concert-management.git
   cd concert-management
   ```

2. **Install dependencies:**

   ```bash
   npm install
   ```

3. **Set up environment variables:**

   Create a `.env` file in the root with the following content:

   ```env
   PORT=3000
   MONGO_URI=mongodb://localhost:27017/concert-management
   JWT_SECRET=your_jwt_secret
   ```

4. **Start the server:**

   ```bash
   npm run dev
   ```

5. **Test API endpoints:**

   Use Postman or any API testing tool. Example POST body for creating a concert:

   ```json
   {
     "name": "Coldplay Live",
     "date": "2025-07-15",
     "time": "19:30",
     "venue": "Madison Square Garden",
     "ticketPrice": 120,
     "availableTickets": 500,
     "image": "https://example.com/concert.jpg"
   }
   ```

## 📌 API Endpoints Overview

| Method | Endpoint                    | Description                    |
|--------|-----------------------------|--------------------------------|
| POST   | `/api/user/auth/register`   | Register a new user            |
| POST   | `/api/user/auth/login`      | Login user                     |
| GET    | `/api/user/concerts`        | Get all concerts               |
| POST   | `/api/user/concerts`        | Create a concert               |
| POST   | `/api/user/bookings`        | Book a concert                 |
| POST   | `/api/user/reviews`         | Post a review                  |
| POST   | `/api/admin/auth/login`     | Admin login                    |
| ...    | `/api/admin/*`              | Admin routes for categories    |

📖 Full API documentation can be generated using tools like Swagger or Postman collections.

## ✅ To Do

- [ ] Add Swagger API documentation
- [ ] Implement pagination and filters
- [ ] Add image upload (e.g. Cloudinary)
- [ ] Unit testing with Jest

## 🤝 Contribution

Contributions are welcome! Please fork the repository and create a pull request.

## 📝 License

This project is licensed under the MIT License.
