This is the frontend of the Blog Application built using modern web technologies. It provides an interactive user interface for performing blog-related operations such as creating, reading, updating, and deleting posts, along with authentication features.

Tech Stack
React.js – Component-based UI library
Axios – HTTP client for API communication
React Router DOM – Client-side routing
Context API / Redux (if used) – State management
CSS / Tailwind CSS / Bootstrap – Styling
Project Structure
Frontend/
│
├── src/
│   ├── components/      # Reusable UI components
│   ├── pages/           # Page-level components (Home, Login, Register, etc.)
│   ├── services/        # API integration using Axios
│   ├── context/         # Global state management (if implemented)
│   ├── App.js           # Root component
│   └── index.js         # Entry point
│
├── public/
├── package.json
└── README.md
System Flow (Frontend–Backend Interaction)
User Interaction (UI)
        │
        ▼
React Components (Pages / Components)
        │
        ▼
Axios Service Layer (API Calls)
        │
        ▼
HTTP Request to Backend Server
        │
        ▼
Backend API (Node.js / Express)
        │
        ▼
MongoDB Database
        │
        ▼
JSON Response
        │
        ▼
React State Update
        │
        ▼
UI Re-render (Updated View)
Installation and Setup
Step 1: Clone the Repository
git clone https://github.com/swaragini01/Blog-App.git
Step 2: Navigate to Frontend Directory
cd Blog-App/Frontend
Step 3: Install Dependencies
npm install
Running the Application
npm start

The application will run on:

http://localhost:3000
Backend Connection

Ensure the backend server is running at:

http://localhost:4000

Configure Axios base URL (typically in a service file):

const API = axios.create({
  baseURL: "http://localhost:4000"
});
Features
User authentication (login and registration)
Create blog posts
View all blogs
Edit existing posts
Delete blog posts
User dashboard (if implemented)
API Integration

The frontend communicates with the backend using Axios.

Example API Calls

Register User

POST /api/auth/register

Login User

POST /api/auth/login

Get Blogs

GET /api/blogs

Create Blog

POST /api/blogs
Environment Variables (Optional)

Create a .env file in the root directory:

REACT_APP_API_URL=http://localhost:4000
Scripts
Command	Description
npm start	Run the application
npm build	Build for production
npm test	Run tests
