# University Identity & Directory Platform

Backend microservices for Group 5: Identity & Directory Platform.

## Microservices Architecture

- **Identity Service**: Source of truth for Users, Roles, Account Status, User-Role relationships, and Authentication/Authorization.
- **Directory Service**: Source of truth for Faculties, Departments, Service Units, and Organizational Responsibilities.

## Setup & Running

### Requirements
- Python 3.10+
- FastAPI
- Pytest

### Identity Service
```bash
cd backend/identity-service
pip install -r requirements.txt
uvicorn app.main:app --port 8001 --reload
```

### Directory Service
```bash
cd backend/directory-service
pip install -r requirements.txt
uvicorn app.main:app --port 8002 --reload
```

### API Documentation (Swagger)
- Identity Service: http://localhost:8001/docs
- Directory Service: http://localhost:8002/docs

### Running Tests
```bash
cd backend/identity-service
pytest
```
