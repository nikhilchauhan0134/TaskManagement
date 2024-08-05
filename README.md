# TaskManagement
Sample Task Management
Project Setup and Functionality Guide
This document serves as a guide on how to set up the project, understand its functionalities, and utilize its endpoints effectively.

Project Setup
Create the Database:

Create a database named Task.
Change the Connection String:

Update the connection string in the configuration file to reflect your server name and database name.
Create Users:

Use the Registration API to create users (Manager, Admin, Employee).
Endpoint: api/Auth/Registration
User Authentication:

Use the Login API to authenticate users. The project uses JWT token-based authentication, although it is not implemented on every endpoint to avoid the necessity of always adding the token.
Functionality and Endpoints
Task Management
Create a Task:

Managers can create tasks using the Create Task endpoint.
Endpoint: api/Tasks/CreateTask
Assign Tasks:

Managers can assign tasks to respective employees using the Task Assignments endpoint.
Endpoint: api/TaskAssignments/CreateTaskAssignments
Update and Delete Tasks:

Managers can update the task priority and delete tasks using the respective endpoints.
Update Task Endpoint: api/Tasks/UpdateTask
Delete Task Endpoint: api/Tasks/DeleteTask
Employee Task Status Update:

Employees can update their task status using the following endpoint:
Endpoint: api/Tasks/TaskUpdateByEmployee
Admin or CEO Task Review:

Admins or CEOs can review assigned and unassigned tasks to employees and check which manager assigned the tasks using the following endpoint:
Endpoint: api/Tasks/TaskReportsAccessByAdmin
This guide provides an overview of setting up the project and utilizing its core functionalities. Ensure to follow the steps accurately for a seamless experience.
