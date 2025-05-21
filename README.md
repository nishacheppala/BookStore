# BookStoreApp

A MERN stack application for browsing and managing books/courses, featuring user authentication, a responsive frontend, and a RESTful backend.

## Features

- User signup and login with hashed passwords
- Browse all books/courses and filter free courses
- Responsive UI with React, Tailwind CSS, and DaisyUI
- Protected routes for authenticated users
- MongoDB for data storage

## Tech Stack

- **Frontend:** React, Vite, Tailwind CSS, DaisyUI, React Router, Axios, React Hook Form, React Hot Toast, React Slick
- **Backend:** Node.js, Express.js, MongoDB, Mongoose, bcryptjs, dotenv, cors

## Folder Structure

```
Backend/
├── controller/        # Controllers handle business logic and route actions
├── model/             # Database schemas/models (e.g., Book, User)
├── route/             # API route definitions (e.g., bookRoutes.js, userRoutes.js)
├── .env               # Environment variables for config (DB, secrets)
├── index.js           # Main server entry point (Express app setup)
└── package.json       # Backend dependencies and scripts

Frontend/
├── public/            # Static assets (images, favicon, etc.)
├── src/
│   ├── components/    # Reusable React components (e.g., Header, BookCard)
│   ├── context/       # React context for global state management
│   ├── courses/       # If this is a bookstore, maybe rename this to something relevant? (e.g., pages/, features/)
│   ├── home/          # Homepage related components or screens
│   ├── App.jsx        # Root React component
│   ├── main.jsx       # React DOM render & app bootstrap
│   └── index.css      # Global styles including Tailwind directives
├── index.html         # Main HTML file for the React app
├── package.json       # Frontend dependencies and scripts
├── tailwind.config.js # Tailwind CSS configuration
└── vite.config.js     # Vite build & dev server config

```

## Getting Started

### Prerequisites

- Node.js
- npm
- MongoDB Atlas account (or local MongoDB)

### Backend Setup

1. Go to the `Backend` folder:
    ```sh
    cd Backend
    ```
2. Install dependencies:
    ```sh
    npm install
    ```
3. Create a `.env` file (already present) and set your MongoDB URI and port:
    ```
    PORT=4001
    MongoDBURI="your-mongodb-uri"
    ```
4. Start the backend server:
    ```sh
    npm start
    ```

### Frontend Setup

1. Go to the `Frontend` folder:
    ```sh
    cd Frontend
    ```
2. Install dependencies:
    ```sh
    npm install
    ```
3. Start the frontend development server:
    ```sh
    npm run dev
    ```
4. Open [http://localhost:5173](http://localhost:5173) in your browser.

## API Endpoints

- `POST /user/signup` - Register a new user
- `POST /user/login` - Login user
- `GET /book` - Get all books/courses

## License

This project is licensed under the ISC License.

---

Made with ❤️ by Ratnesh
