
# Go + Next.js Fullstack Application

This is a **Fullstack CRUD Application** built with a Go backend and a Next.js frontend. It demonstrates fundamental CRUD operations (Create, Read, Update, Delete) with a seamless integration of modern backend and frontend technologies.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation and Setup](#installation-and-setup)
  - [Requirements](#requirements)
  - [Steps](#steps)
- [Endpoints](#endpoints)
- [Usage](#usage)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)

---

## Project Overview

This application allows users to perform CRUD operations on a database. It uses a **Go backend** for handling API requests and a **Next.js frontend** for rendering the user interface.

---

## Features

- User management with full CRUD functionality.
- RESTful API implementation.
- Clean and modular code structure.
- Dockerized setup for easy deployment.

---

## Technologies Used

### Backend
- **Go**: For building a high-performance REST API.
- **Fiber**: A Go web framework inspired by Express.js.
- **Redis**: For in-memory data storage and caching.

### Frontend
- **Next.js**: A React framework with server-side rendering and static site generation.
- **TailwindCSS**: For styling the UI.

### DevOps
- **Docker**: Containerized development and deployment.
- **Docker Compose**: Multi-container orchestration.

---

## Installation and Setup

### Requirements
- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)
- [Node.js](https://nodejs.org/)
- [Go](https://golang.org/)

### Steps

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/razyneko/go-next-fullstack-app.git
   cd go-next-fullstack-app
   ```

2. **Set Up Environment Variables**:
   - Create a `.env` file in the root directory.
   - Add variables like:
     ```env
     APP_PORT=3000
     DB_CONNECTION=your_database_connection_string
     ```

3. **Build and Start the Application**:
   - Using Docker Compose:
     ```bash
     docker-compose up --build
     ```
   - Alternatively, manually start backend and frontend:
     ```bash
     cd backend
     go run main.go

     cd frontend
     npm install
     npm run dev
     ```

4. **Access the Application**:
   Open `http://localhost:3000` in your browser.

---

## Endpoints

### Backend API

| Method | Endpoint       | Description              |
|--------|----------------|--------------------------|
| GET    | `/api/v1/users` | Fetch all users         |
| POST   | `/api/v1/users` | Create a new user       |
| PUT    | `/api/v1/users/:id` | Update user details |
| DELETE | `/api/v1/users/:id` | Delete a user       |

---

## Usage

1. Visit the application in your browser at `http://localhost:3000`.
2. Perform CRUD operations via the user interface.
3. View logs and monitor API activity in the Docker or terminal logs.

---

## Contributing

Contributions are welcome! Feel free to fork the repository and submit pull requests.

### Steps
1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add a new feature"
   ```
4. Push to the branch:
   ```bash
   git push origin feature-name
   ```
5. Submit a pull request.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

--- 

Let me know if you need help updating your repository with this file!
