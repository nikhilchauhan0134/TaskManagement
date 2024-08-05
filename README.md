# TaskManagement
# Sample Task Management
# Project Setup and Functionality Guide
# This document serves as a guide on how to set up the project, understand its functionalities, and utilize its endpoints effectively.
# Project Setup
# 1.	Create the Database:
  o	Create a database named Task.
# 2.	Change the Connection String:
   o	Update the connection string in the configuration file to reflect your server name and database name.
# 3.	Create Users:
    o	Use the Registration API to create users (Manager, Admin, Employee).
    o	Endpoint: api/Auth/Registration
# 4.	User Authentication:
    o	Use the Login API to authenticate users. The project uses JWT token-based authentication, although it is not implemented on every endpoint to avoid the necessity of 
     always adding the token.
# Functionality and Endpoints
# Task Management
# 5.	Create a Task:
    o	Managers can create tasks using the Create Task endpoint.
    o	Endpoint: api/Tasks/CreateTask
# 6.	Assign Tasks:
    o	Managers can assign tasks to respective employees using the Task Assignments endpoint.
    o	Endpoint: api/TaskAssignments/CreateTaskAssignments
# 7.	Update and Delete Tasks:
    o	Managers can update the task priority and delete tasks using the respective endpoints.
    o	Update Task Endpoint: api/Tasks/UpdateTask
    o	Delete Task Endpoint: api/Tasks/DeleteTask
# 8.	Employee Task Status Update:
    o	Employees can update their task status using the following endpoint:
    o	Endpoint: api/Tasks/TaskUpdateByEmployee
# 9.	Admin or CEO Task Review:
    o	Admins or CEOs can review assigned and unassigned tasks to employees and check which manager assigned the tasks using the following endpoint:
    o	Endpoint: api/Tasks/TaskReportsAccessByAdmin
# This guide provides an overview of setting up the project and utilizing its core functionalities. Ensure to follow the steps accurately for a seamless experience.
