# Local Problem Reporting System

A microservices-based web application developed using Django for reporting and managing local community issues. The system is containerized using Docker and supports automated deployment through Jenkins.

---

## Project Structure

```
.
├── authenticationApp/              # Authentication and user management service
├── reportingApp/                   # Problem reporting service
├── localProblemReportingSystemApp/ # Main Django project
├── docker-compose.yml              # Docker Compose configuration
├── Dockerfile                      # Docker image configuration
├── entrypoint.sh                   # Container startup script
├── Jenkinsfile                     # Jenkins CI/CD pipeline
├── requirements.txt                # Project dependencies
├── manage.py                       # Django management script
├── db.sqlite3                      # SQLite database
└── README.md
```

---

## Features

- User registration and authentication
- Report local issues
- View and manage reported problems
- REST API-based architecture
- Docker containerization
- Jenkins CI/CD pipeline
- Independent microservice modules
- Scalable deployment architecture

---

## Tech Stack

- **Backend:** Python, Django
- **API Framework:** Django REST Framework
- **Database:** SQLite
- **Containerization:** Docker, Docker Compose
- **CI/CD:** Jenkins
- **Version Control:** Git, GitHub

---

## Installation

### Clone the Repository

```bash
git clone https://github.com/<username>/<repository-name>.git
cd <repository-name>
```

### Create Virtual Environment

```bash
python -m venv venv
```

Activate the environment:

#### Windows

```bash
venv\Scripts\activate
```

#### Linux/macOS

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Database Migrations

```bash
python manage.py migrate
```

### Start the Application

```bash
python manage.py runserver
```

The application will run on:

```
http://127.0.0.1:8000/
```

---

## Docker Setup

### Build Docker Image

```bash
docker build -t local-problem-reporting-system .
```

### Run Using Docker Compose

```bash
docker-compose up --build
```

---

## CI/CD Pipeline

The project uses Jenkins for continuous integration and deployment.

Pipeline stages include:

- Source code checkout
- Dependency installation
- Unit testing
- Docker image build
- Deployment

Pipeline configuration is defined in:

```
Jenkinsfile
```

---

## Application Modules

### Authentication Service

Responsible for:

- User registration
- Login
- Authentication
- User management

### Reporting Service

Responsible for:

- Creating reports
- Viewing reports
- Updating report status
- Managing reported issues

---

## Useful Commands

### Create Migrations

```bash
python manage.py makemigrations
```

### Apply Migrations

```bash
python manage.py migrate
```

### Run Tests

```bash
python manage.py test
```

### Create Superuser

```bash
python manage.py createsuperuser
```

---


## Author

**Subin George**

MSc Cloud Computing  
National College of Ireland

---

## License

This project is intended for educational and learning purposes.