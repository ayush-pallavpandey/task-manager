eam Task Manager (Full-Stack)
A production-ready task management application featuring a Java Spring Boot backend and a responsive Vanilla JavaScript frontend. This project demonstrates a decoupled architecture with cross-origin security and JWT-based authentication.  

🚀 Live Demo
Frontend (Netlify): [https://your-app-name.netlify.app](https://your-app-name.netlify.app)

Backend API (Railway): [https://your-api-name.up.railway.app](https://your-api-name.up.railway.app)

🛠 Tech Stack
Backend: Java 17, Spring Boot 3.x, Spring Security, JWT, JPA/Hibernate.  

Database: MySQL (Hosted on Railway).  

Frontend: HTML5, CSS3, JavaScript (ES6+), Fetch API.  

Deployment: Railway (Backend & DB) | Netlify (Frontend).

🏗 System Architecture
The project follows a Layered Architecture pattern to ensure scalability and maintainability:

Controller Layer: Handles HTTP requests and API versioning.  

Service Layer: Contains business logic and transactional boundaries.  

Repository Layer: Interacts with MySQL via Spring Data JPA.  

Security: Implements a Stateless JWT filter for secure cross-domain requests.
team-task-manager/
├── backend/                  # Spring Boot Application
│   ├── src/main/java/com/example/taskmanager/
│   │   ├── config/           # Security & CORS configuration
│   │   ├── controller/       # REST Endpoints
│   │   ├── entity/           # JPA Database Models
│   │   ├── repository/       # Data Access Layer
│   │   └── service/          # Business Logic
│   └── application.properties # Railway DB Config
└── frontend/                 # Netlify Deployment Folder
    ├── index.html            # Login/Landing Page
    ├── dashboard.html        # Task Management View
    ├── css/                  # Styling
    └── js/                   # API Integration (Fetch)

    Deployment Steps
Backend (Railway)
Connect your GitHub repo to Railway.

Add a MySQL Database plugin in the Railway dashboard[cite: 1].

Railway will automatically detect the pom.xml and deploy.

Frontend (Netlify)
Ensure your js/ files point to the Railway production URL.

Drag and drop the frontend/ folder into the Netlify upload zone.

Configure Redirects (if using a SPA) to handle clean URLs.

📄 License
Distributed under the MIT License.
