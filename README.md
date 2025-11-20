# 🏢 The Whispering Walls: Intelligent IoT Facility Monitor

> **"If walls could talk, what would they say?" This project gives them a voice.**

### 🚀 Overview
**The Whispering Walls** is a Digital Twin solution that solves the operational "blind spot" in facility management. In a traditional building, facility managers are reactive—waiting for equipment to break.

This system changes the paradigm to **predictive monitoring**. By simulating a network of **100+ environmental sensors**, the "walls" continuously stream real-time health data (Temperature, Humidity, Power), allowing the system to "whisper" alerts about anomalies before they become critical failures.

### 🛠️ Tech Stack
* **Backend Logic:** Python 3.10, Pandas (Data Analysis)
* **API Layer:** FastAPI (Asynchronous REST API)
* **Frontend:** React.js (Live Dashboard & Visualization)
* **DevOps & Deployment:** Docker (Containerization), GitHub Actions (CI/CD Pipeline)

### ⚡ Key Features
* **IoT Simulation Engine:** Generates realistic time-series data for multiple sensor nodes simultaneously, mimicking a living building.
* **"Whisper" Alert Logic:** Algorithmic monitoring that triggers immediate "CRITICAL" status alerts when safety thresholds (e.g., >80°C) are breached.
* **Containerized Architecture:** Fully Dockerized environment ensuring consistent behavior across development and production servers.
* **Automated Quality Control:** Integrated CI/CD pipeline via GitHub Actions to ensure the system remains reliable and bug-free.

### 🏗️ Architecture
The system follows a **Microservices-ready architecture**:
1.  **The Simulator (Python):** Acts as the physical infrastructure, generating raw telemetry.
2.  **The Interpreter (FastAPI):** Processes the signals and exposes endpoints (`GET /metrics`).
3.  **The Dashboard (React):** Visualizes the building's "voice" into actionable graphs for the user.