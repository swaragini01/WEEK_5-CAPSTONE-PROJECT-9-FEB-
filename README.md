📘 Blog App Frontend

This is the frontend of the Blog Application built using modern web technologies. It provides an interactive UI for users to create, read, update, and delete blog posts, along with authentication features.

🚀 Tech Stack
React.js – Frontend library for building UI
Axios – For API requests
React Router DOM – For navigation
Context API / Redux (if used) – State management
CSS / Tailwind CSS / Bootstrap – Styling
📂 Project Structure
Frontend/
│── src/
│   ├── components/     # Reusable UI components
│   ├── pages/          # Page components (Home, Login, Register, etc.)
│   ├── services/       # API calls using Axios
│   ├── context/        # State management (if used)
│   ├── App.js          # Main app component
│   ├── index.js        # Entry point
│
│── public/
│── package.json
│── README.md
⚙️ Installation & Setup
1️⃣ Clone the repository
git clone https://github.com/swaragini01/Blog-App.git
2️⃣ Navigate to frontend folder
cd Blog-App/Frontend
3️⃣ Install dependencies
npm install
▶️ Running the Application
npm start
App will run on:
👉 http://localhost:3000
🔗 Backend Connection

Make sure your backend server is running:

http://localhost:4000

Update API base URL in your frontend (usually inside Axios config or services file):

const API = axios.create({
  baseURL: "http://localhost:4000"
});
✨ Features
🔐 User Authentication (Login/Register)
📝 Create Blog Posts
📖 View All Blogs
✏️ Edit Blogs
❌ Delete Blogs
👤 User Dashboard (if implemented)
📡 API Integration

Frontend communicates with backend using Axios.

Example API Calls:
Register User
POST /api/auth/register
Login User
POST /api/auth/login
Get Blogs
GET /api/blogs
Create Blog
POST /api/blogs
📌 Environment Variables (Optional)

Create a .env file:

REACT_APP_API_URL=http://localhost:4000
🛠️ Scripts
Command	Description
npm start	Run the app
npm build	Build for production
npm test	Run tests
