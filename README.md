# Parcel Delivery System (Full-Stack Simulation)

## Project Overview
The Parcel Delivery System is a full-stack web application designed to simulate a modern, automated locker-based delivery system (like Posti or Matkahuolto in Finland). The project is composed of four interconnected applications built on a centralized RESTful API infrastructure, showcasing complex, real-time communication between multiple Node.js backends and React frontends.

## ⚙️ Technical Architecture
The system comprises four separate applications and a shared database, connected via a single RESTful API.

| Component | Technology | Description |
|-----------|------------|-------------|
| Backend API | Node.js (Express) | Handles all data persistence, business logic, and API endpoints for the entire system. |
| Frontend UI | React / JavaScript | Developed the user interfaces for the Driver App and the Locker Simulator. |
| Database | MySQL | Stores all parcel, user, and locker status data. |
| Cloud/Deployment | Microsoft Azure | Successfully deployed the Locker Simulator frontend and MySQL database. |

##  My Core Responsibilities
As the primary developer, I was responsible for the architectural design, implementation, and deployment of 3 out of the 4 core applications:

- **Architectural Design & Integration**: Co-developed the MySQL database schema and designed/implemented the core RESTful API contract, handling all full-stack API integration for the Node.js backends and React frontends of the Driver App and Locker Simulator.

- **Module Implementation & Automation**: Solely implemented the full-stack development of the Delivery Driver App and Locker Simulator, as well as the backend Parcel Generator "Robot" (Node.js Express) for system automation and mock parcel creation.

- **Cloud Deployment**: Managed the successful deployment of the Locker Simulator frontend and MySQL database to Microsoft Azure.

## Key Functional Deliverables

### 1. Delivery Driver Application (React / Node.js)
- **Real-time Management**: Allows drivers to view available cabinets, mark parcels as picked up, and manage delivery status updates.
- **Authentication**: Secure driver login and management.

### 2. Parcel Locker Touchscreen Simulator (React / Node.js)
- **Secure Code Validation**: Frontend UI simulates pickup and delivery operations using validation of unique parcel codes.
- **Real-time Status**: Automatically updates parcel and locker availability status via the central API.

### 3. Parcel Generator "Robot" (Node.js Express)
- **Automated Data Creation**: Backend-only service designed to generate new parcel data for consumer users, ensuring fresh data for testing and simulation.

### 4. Consumer User Application
- **Account & History**: Features user-friendly signup, authentication, and detailed parcel history tracking.
- **Sending Workflow**: Enables users to send parcels and receive a secure pickup code.

## Installation and Usage

To get started with Parcel App, follow these simple steps:

1. **Clone the repositories:**
   - [Consumer User Application](https://github.com/Parcel-Delivery-System/user-app): `git clone https://github.com/Parcel-Delivery-System/user-app.git`
   - [Delivery Driver Application](https://github.com/Parcel-Delivery-System/delivery-driver-app.git): `git clone https://github.com/Parcel-Delivery-System/delivery-driver-app.git`
   - [Locker Simulator](https://github.com/Parcel-Delivery-System/locker-simulator.git): `git clone https://github.com/Parcel-Delivery-System/locker-simulator.git`
   - [Parcel Generator "Robot"](https://github.com/Parcel-Delivery-System/parcel-generator-robot.git): `git clone https://github.com/Parcel-Delivery-System/parcel-generator-robot.git`

2. **Install dependencies in every repository:** `npm install` 

3. **Configure the backend settings:** !! Remember to directly set/change the database credentials based on your local database.!!
         STEPS: Launch MySQL Workbench.
               Log in and connect to your MySQL database server.
               Go to "File" -> "Open SQL Script..."
               Choose your SQL file and click "Open."
               Click the lightning bolt icon or select "Query" -> "Execute."
               You can also use MySQL Client.

               Return to the backend and edit the user, password, and database name to connect to your local database.

4. **Run the applications:** `npm start`   !! RUN THE CONSUMER USER APPLICATION FIRST BEFORE THE OTHER APPS!!

