# 🛠️ Feedback Collector System (FCS) - API

A lightweight RESTful API built with Spring Boot for collecting, managing, and organizing user feedback into defined categories. It powers the backend of the **Feedback Collector System**.

---

## 🔗 Live Deployment

- **Base API URL:** [`https://feedback-collector-system.onrender.com`](https://feedback-collector-system.onrender.com)
- **Frontend App:** [`https://feedback-collector-system.vercel.app`](https://feedback-collector-system.vercel.app)

---

## 🚀 API Endpoints

### ➕ Submit Feedback

- **POST** `/api/feedback/submit`
- **Request Body:**
```json
{
  "name": "John Doe",
  "category": "BUG",
  "message": "There’s a glitch in the UI."
}
```
**Response**: 201 Created

### 📥View Feedback
- **GET** `/api/feedback/view`
- **Query Param (Optional)**: `?category=PRAISE | BUG | FEATURE_REQUEST | COMPLAINT | OTHER`

**Response**: List of feedback objects

### 🔍 View Feedback by ID
- **GET**  `/api/feedback/{id}`

**Response**: Specific feedback or 404 Not Found

### ❌ Delete Feedback
- **DELETE** /api/feedback/{id}

**Response**: 200 OK on successful deletion

🧾 Supported Categories
-PRAISE
- BUG
- FEATURE_REQUEST
- COMPLAINT
- OTHER

⚙️ Tech Stack
- Java
- Spring Boot
- Maven
- H2 (In-Memory Database)
- Deployed on: Render

### 👨‍💻 Author
Built with 💡 and ☕ by Vedant Jain
