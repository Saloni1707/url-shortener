# URL Shortener

## 🚀 Project Overview
The **URL Shortener** is a web application that allows users to shorten long URLs into more manageable, compact links. This project is built using the **MERN stack** (MongoDB, Express.js, React.js, and Node.js) with a **distributed architecture** to ensure scalability and performance.

## 📌 Features
- Generate short URLs for long links
- Redirect users to the original URL when they access the short link
- Track the number of clicks per short URL
- User authentication (optional)
- Custom short URL aliases (optional)
- API endpoints for URL shortening and retrieval

## 🛠️ Tech Stack
### Frontend
- React.js (Vite for fast development)
- Tailwind CSS (for styling)
- Axios (for API requests)

### Backend
- Node.js & Express.js (API server)
- MongoDB (Database for storing URLs)
- Redis (Optional: for caching and improving performance)

### Deployment
- Frontend: Vercel/Netlify
- Backend: Render/Heroku
- Database: MongoDB Atlas

## 📂 Project Structure
```
url-shortener/
│-- frontend/        # React.js frontend
│-- backend/         # Express.js backend
│-- README.md        # Project documentation
```

## 🚀 Getting Started
### Prerequisites
Ensure you have the following installed:
- Node.js (v16+)
- MongoDB (local or Atlas)
- Git

### Setup Instructions
#### 1️⃣ Clone the Repository
```sh
git clone https://github.com/Saloni1707/url-shortener.git
cd url-shortener
```

#### 2️⃣ Install Dependencies
##### Frontend
```sh
cd frontend
npm install
```
##### Backend
```sh
cd ../backend
npm install
```

#### 3️⃣ Set Up Environment Variables
Create a **.env** file in the `backend` directory and add:
```
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
BASE_URL=http://localhost:5000
```

#### 4️⃣ Run the Application
##### Start Backend
```sh
cd backend
npm run dev
```
##### Start Frontend
```sh
cd frontend
npm run dev
```
Open **http://localhost:5173/** in your browser.

## 📖 API Endpoints
| Method | Endpoint        | Description                |
|--------|---------------|----------------------------|
| POST   | /api/url       | Shorten a long URL         |
| GET    | /:shortId      | Redirect to original URL   |
| GET    | /api/stats     | Get analytics (click count)|

## 🛠️ Future Enhancements
- User authentication for managing links
- Custom short URL aliases
- QR code generation for shortened URLs
- Rate limiting to prevent abuse

## 💡 Contributing
Contributions are welcome! Feel free to fork the repo and submit a pull request.

## 📜 License
This project is licensed under the **MIT License**.

---
**Made with ❤️ by Saloni1707**

