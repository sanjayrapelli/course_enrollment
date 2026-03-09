
# 🎓 Course Enrollment System

A full-stack application to manage course enrollments with a React frontend and a Node.js/Express backend. This system provides students with a user-friendly interface to browse courses, enroll, and view enrollment history, while administrators can manage courses and users through dedicated API routes.

---

## 🚀 Features

- **Frontend (React)**  
  - Browse and search available courses  
  - Enroll/unenroll in courses  
  - View current and past enrollments  
  - Basic UI for authentication and error handling

- **Backend (Node.js + Express)**  
  - RESTful API for CRUD operations on courses and enrollments  
  - Authentication middleware  
  - Mongoose models for Courses, Users, and Enrollments  
  - Error handling and environment configuration

---

## 🧰 Tech Stack

- **Frontend**  
  - React (Create React App)  
  - Axios for HTTP requests  
  - React Router for navigation

- **Backend**  
  - Node.js & Express  
  - MongoDB with Mongoose ODM  
  - dotenv for environment variables

---

## 📁 Repository Structure

```text
/
├── client/                 # React frontend
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── ...
└── course_enroll/          # Express backend
    ├── models/
    ├── routes/
    ├── middleware/
    ├── scripts/
    ├── server.js
    ├── package.json
    └── .env
```

---

## 💻 Setup & Installation

### 1. Clone the Repository

```bash
git clone https://github.com/sanjayrapelli/course_enrollment.git
cd course_enrollment
```

### 2. Backend Setup (`course_enroll/`)

```bash
cd course_enroll
npm install
cp .env.example .env
# Edit .env with your settings (e.g., MongoDB URI, JWT secret, PORT)
npm start
```


### 3. Frontend Setup (`client/`)

```bash
cd ../client
npm install
npm start
# App will run on http://localhost:3000
```


---

## 📦 Usage

1. Start both backend and frontend servers.
2. In the React app, browse available courses.
3. Click “Enroll” to join a course.
4. Visit your enrollment page to view or manage your courses.

---

## 📜 API Endpoints (Overview)

**Courses**

* `GET /api/courses` – List all courses
* `POST /api/courses` – Create a new course
* `GET /api/courses/:id` – Get a single course
* `PUT /api/courses/:id` – Update course
* `DELETE /api/courses/:id` – Remove course

**Enrollments**

* `POST /api/enroll` – Enroll a user in a course
* `GET /api/enrollments/:userId` – Get a user’s enrollments
* `DELETE /api/enroll/:id` – Cancel an enrollment

**Auth**

* `POST /api/auth/register` – Register new user
* `POST /api/auth/login` – Authenticate and get token

---

## 🧩 Environment Variables

Create and configure `.env` in the root of `course_enroll/`:

```env
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=a_very_secure_secret
PORT=5000
```


---

## 📝 Scripts

* **Backend**

  * `npm start` – Run the server
  * `npm run dev` – Run with nodemon (if configured)
* **Frontend**

  * `npm start` – Launch React development server
  * `npm run build` – Create production build

---

## 🤝 Contributing

Contributions are welcome!

1. Fork this repo
2. Create a feature branch: `git checkout -b feature-name`
3. Make changes and commit
4. Push to your fork and open a Pull Request

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 🙋‍♂️ Author

Built by Sanjay Rapelli. For questions, feel free to open an issue or contact me on GitHub!
