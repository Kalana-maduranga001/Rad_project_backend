
## 👕 Clothing Brand Store – Backend

A RESTful backend API for the Clothing Brand e-commerce system, built using **Node.js, Express & TypeScript**.
Handles authentication, products, orders, and business logic.

---

## ⚙️ Core Features

* User authentication & authorization (JWT)
* Product management (CRUD)
* Order management system
* Product size handling
* Secure password hashing
* RESTful API architecture
* Role-based access control (Admin / User)
* Clean layered architecture

---

## 🛠️ Technologies Used

* **Node.js**
* **Express.js**
* **TypeScript**
* **MongoDB** with **Mongoose**
* **JWT (jsonwebtoken)**
* **bcryptjs**
* **dotenv**
* **CORS**
* **express-validator**

---

## 📸 Screenshots

* API testing using Postman
* MongoDB collections (Users, Products, Orders)

*(Optional but recommended for GitHub)*

---

## 🚀 Setup & Run Instructions

### 1️⃣ Clone the repository

```bash
git clone https://github.com/Kalana-maduranga001/Rad_project_backend.git
cd Rad_project_backend
```

### 2️⃣ Install dependencies

```bash
npm install
```

### 3️⃣ Configure environment variables

Create a `.env` file in the root directory:

```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
JWT_EXPIRE=7d
```

---

### 4️⃣ Start the server

#### Development

```bash
npm run dev
```

#### Production

```bash
npm run build
npm start
```

📍 Backend API will run at:
**[http://localhost:5000](http://localhost:5000)**

---

## 🔗 REST API Endpoints

### Authentication

| Method | Endpoint           | Description      |
| ------ | ------------------ | ---------------- |
| POST   | /api/auth/register | Register user    |
| POST   | /api/auth/login    | Login user       |
| GET    | /api/auth/me       | Get current user |

### Products

| Method | Endpoint          | Description            |
| ------ | ----------------- | ---------------------- |
| GET    | /api/products     | Get all products       |
| POST   | /api/products     | Create product (Admin) |
| PUT    | /api/products/:id | Update product         |
| DELETE | /api/products/:id | Delete product         |

### Orders

| Method | Endpoint        | Description            |
| ------ | --------------- | ---------------------- |
| POST   | /api/orders     | Create order           |
| GET    | /api/orders     | Get all orders (Admin) |
| GET    | /api/orders/:id | Get order by ID        |

---

## 📁 Project Structure

```
src/
 ├── controllers/       # Business logic
 ├── models/            # Mongoose schemas
 ├── routes/            # API routes
 ├── middleware/        # Auth & error handling
 ├── services/          # Business services
 ├── config/            # Database config
 └── server.ts          # Entry point
```

---

## 🔐 Security

* Password hashing with bcryptjs
* JWT-based authentication
* Protected routes using middleware
* Environment variables for sensitive data
* CORS configuration

---

## 📌 Notes

* Ensure MongoDB is running before starting the server
* Use strong JWT secrets in production
* Designed following RAD principles

---

## 👨‍💻 Author

**Kalana Maduranga**
Full Stack Developer
RAD Coursework Project

---

## 📄 License

This project is licensed under the **MIT License**
