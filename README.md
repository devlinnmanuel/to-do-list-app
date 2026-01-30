# To Do List App (Simple Task Application)

This project is a **Simple Task Application** built using **Vue.js** as the Front End and **REST API** as the Back End.  
The application was developed as a **Final Project (UAS)** for the course:

**UAS Pengembangan Aplikasi Berbasis Platform IBDA**  
Academic Year: **2024 / 2025**

The main purpose of this application is to help users manage daily tasks efficiently by organizing tasks based on day and priority level.

---

## Project Features

- Login & Logout (simple authentication)
- View and monitor tasks by day (Monday – Sunday)
- Add, edit, delete, and mark tasks as done
- Filter tasks by category (Important, Urgent, Regular)
- Simple, responsive and user-friendly interface

---

## Main Workflow

1. User logs into the system  
2. User views the task monitoring dashboard  
3. User adds or edits tasks through the Task Entry form  
4. User manages tasks (edit, delete, mark as done)  
5. User logs out

---

## Use Cases

### 1. Login & Logout
For authentication simulation, no user database is required.  

---

### 2. Task Monitoring

Users can view all tasks grouped by days: Monday - Sunday

Each task belongs to one of three categories:

- Important  
- Urgent  
- Regular  

Users can filter tasks based on category, and the task list will update automatically.

Each task card displays:

- Task Title  
- Task Description (partial or full)  
- Last Updated Time  
- Action buttons:
  - Edit  
  - Delete  
  - Mark as Done  

Rules:

- If no tasks exist on a specific day, the UI shows a button to add a new task.
- If a task is marked as **Done**, it can no longer be edited or deleted.

---

### 3. Task Entry

This screen is used to:

- Add a new task (empty form)
- Edit an existing task (form filled with data)

Form Fields:

- Title  
- Day  
- Description  
- Category (Important / Urgent / Regular)  
- Status (Active, Deleted, Done)  
- Last Updated Time  

Available Actions:

- **Save** → Save new task or update existing task  
- **Cancel** → Return to Task Monitoring screen  

---

## Technology Stack

### Front End
- Vue.js

### Back End
- REST API

### Database
- MySQL

---

## How to Run the Project

Before running the Vue.js application, make sure the backend server is already running.

1. Run the Flask backend server:

```bash
python appv2.py

```
Ensure that appv2.py is located in the same directory as the project.

2. Install dependencies and start the Vue application:
```bash
npm install
npm run dev
```

3. The authentication (login) process is hardcoded in the backend server.
```bash
Username: admin  
Password: abcdef
