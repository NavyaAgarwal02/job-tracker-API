# 🚀 Job Tracker API

A secure and scalable RESTful API for managing job applications.  
Built with Node.js, Express, MongoDB, and JWT authentication, this project demonstrates real-world backend development practices including authentication, authorization, filtering, and user-based data isolation.



## 📌 Features

- 🔐 User Authentication (Register & Login)
- 🪪 JWT-based Authorization
- 🛡 Protected Routes using Middleware
- 👤 User-specific Data Ownership
- 📄 Full CRUD Operations for Job Applications
- 🔍 Search by Company, Role, and Notes
- 🧭 Filter by Status & Company
- 📊 Sorted Results (Latest First)
- ⚙️ RESTful API Architecture



## 🧰 Tech Stack

- Node.js  
- Express.js  
- MongoDB + Mongoose  
- JSON Web Token (JWT)  
- bcryptjs  
- Git & GitHub  



## 📁 Project Structure

```

src/
├── config/        # Database configuration
├── controllers/   # Business logic
├── middleware/    # Authentication middleware
├── models/        # Mongoose schemas
├── routes/        # API routes
└── app.js         # Application entry point

````



## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/NavyaAgarwal02/job-tracker-API.git
cd job-tracker-api
````

### 2️⃣ Install Dependencies

```bash
npm install
```

### 3️⃣ Configure Environment Variables

Create a `.env` file in the root directory:

```env
PORT=3000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_super_secret_key
```

### 4️⃣ Run the Server

```bash
npm start
```

or (for development)

```bash
npm run dev
```



## 🔑 API Endpoints

### 🔐 Authentication

| Method | Endpoint           | Description   |
| ------ | ------------------ | ------------- |
| POST   | /api/auth/register | Register user |
| POST   | /api/auth/login    | Login user    |

### 📄 Job Applications (Protected)

| Method | Endpoint              | Description           |
| ------ | --------------------- | --------------------- |
| POST   | /api/applications     | Create application    |
| GET    | /api/applications     | Get all applications  |
| GET    | /api/applications/:id | Get application by ID |
| PUT    | /api/applications/:id | Update application    |
| DELETE | /api/applications/:id | Delete application    |

> ⚠️ All application routes require a valid JWT token.



## 🔐 Authentication Flow

1. Register or login
2. Receive JWT token
3. Send token in request headers
4. Access protected routes

Example Header:

```http
Authorization: Bearer <token>
```



## 📌 Sample Request

### Create Job Application

```http
POST /api/applications
Authorization: Bearer <token>
Content-Type: application/json
```

```json
{
  "company": "Google",
  "role": "Software Engineer",
  "status": "Applied",
  "notes": "Applied via referral"
}
```



## 🚀 Future Enhancements

* 📈 Analytics Dashboard
* 📧 Email Notifications
* 🗂 Resume Upload Support
* 📅 Interview Scheduling
* 🌐 Cloud Deployment



## 👩‍💻 Author

**Navya Agarwal**
📧 Email: [27agarwalnavya@gmail.com](mailto:27agarwalnavya@gmail.com)
🔗 GitHub: [https://github.com/NavyaAgarwal02](https://github.com/NavyaAgarwal02)



## 📜 License

This project is licensed under the MIT License.
Free to use for learning and development.

```

---

If you’d like, I can next help you optimize this README for **resume + recruiter visibility**.
```



