
# FastAPI Todo Project with MongoDB

## Table of Contents

- [FastAPI Todo Project with MongoDB](#fastapi-todo-project-with-mongodb)
  - [Table of Contents](#table-of-contents)
  - [Features](#features)
  - [Technologies Used](#technologies-used)
  - [Backend Installation](#backend-installation)
    - [MongoDB Setup](#mongodb-setup)
    - [FastAPI Setup](#fastapi-setup)
  - [Frontend Installation](#frontend-installation)
  - [Usage](#usage)
    - [Example Commands](#example-commands)
  - [API Endpoints](#api-endpoints)
    - [**GET** /api/tasks](#get-apitasks)
    - [**POST** /api/tasks](#post-apitasks)
    - [**GET** /api/tasks/{id}](#get-apitasksid)
    - [**PUT** /api/tasks/{id}](#put-apitasksid)
    - [**DELETE** /api/tasks/{id}](#delete-apitasksid)

## Features

- Basic CRUD operations for managing tasks
- Frontend runs on port 8000, Backend runs on port 8001
- Dockerized application for easy deployment

## Technologies Used

- **Frontend:** React
- **Backend:** FastAPI
- **Database:** MongoDB
- **API:** RESTful API

## Backend Installation

### MongoDB Setup
1. Install MongoDB on your system. Refer to the MongoDB official website for installation instructions.

### FastAPI Setup
1. Navigate to the backend directory in the command line.
2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # for Linux/macOS
   venv\Scripts\activate.bat  # for Windows
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Frontend Installation

1. Navigate to the frontend directory in the command line.
2. Install npm if it is not already installed:
   ```bash
   npm install
   ```

## Usage

### Example Commands

- To create a new task:
  ```bash
  curl -X POST http://localhost:8001/api/tasks -H "Content-Type: application/json" -d '{"title": "New Task"}'
  ```

- To retrieve all tasks:
  ```bash
  curl -X GET http://localhost:8001/api/tasks
  ```

## API Endpoints

### **GET** /api/tasks

### **POST** /api/tasks

**Request Body:**
```json
{
  "title": "string"
}
```

### **GET** /api/tasks/{id}

### **PUT** /api/tasks/{id}

**Request Body:**
```json
{
  "title": "string"
}
```

### **DELETE** /api/tasks/{id}
