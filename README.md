To successfully deploy this **Odoo Docker Lab**, we recommend to have **Git, Visual Studio Code, and Docker Desktop** installed. Each tool plays a crucial role in setting up, managing, and deploying your environment. Here’s why each prerequisite is important:

---

## **1. Git – Version Control System**
**Why is Git needed?**
- Git allows you to **store, track, and collaborate** on your code.
- Helps in **cloning** the repository from GitHub to your local machine.
- Allows you to **push updates** back to GitHub for future modifications.

**Commands Used:**
- `git clone <repo-url>` → Copies the project from GitHub to your local machine.
- `git add .` → Stages all modified files.
- `git commit -m "message"` → Saves the changes locally.
- `git push origin main` → Uploads changes to GitHub.

**Installation:**
- Download and install from: [https://git-scm.com/](https://git-scm.com/)

---

## **2. Visual Studio Code (VS Code) – Code Editor**
**Why is VS Code needed?**
- Provides a **user-friendly interface** for editing and managing your project files.
- The **integrated terminal** allows you to run `git` and `docker` commands without switching applications.
- The **Docker extension** helps you manage containers visually.

**Key Features Used:**
- **Terminal for running Docker & Git commands.**
- **Syntax highlighting for Docker & YAML files.**
- **Extensions support** (e.g., Docker extension for better integration).

**Installation:**
- Download from: [https://code.visualstudio.com/](https://code.visualstudio.com/)

---

## **3. Docker Desktop – Containerization Platform**
**Why is Docker needed?**
- Docker **creates and runs isolated environments (containers)** for your Odoo app.
- Ensures **consistent deployment** across different machines.
- Simplifies dependency management (e.g., PostgreSQL setup is handled via Docker).

**Key Features Used:**
- **Docker Engine** runs the containers.
- **Docker Compose** (`docker-compose.yml`) manages multi-container setup (Odoo + PostgreSQL).
- **Volumes** help persist Odoo & database data.

**Installation:**
- Download from: [https://www.docker.com/products/docker-desktop/](https://www.docker.com/products/docker-desktop/)
- Ensure **WSL 2 (for Windows)** or **Linux kernel support (for Mac/Linux)** is enabled.

---

## **Deployment Workflow Using These Tools**
1. **Git:** Clone the project from GitHub → `git clone <repo-url>`.
2. **VS Code:** Open project and edit files (`docker-compose.yml`, `Dockerfile`).
3. **Docker:** Run the app with `docker-compose up -d`.
4. **Access Odoo:** Open `http://localhost:8070` in your browser.

---

### **Conclusion**
Without **Git**, you won’t be able to clone and track your code.  
Without **VS Code**, managing and editing the setup will be harder.  
Without **Docker Desktop**, you can’t run Odoo in an isolated environment.  
