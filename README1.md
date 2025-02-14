# Reports Materials Microservice

## 📌 Overview
The `reports_materials` microservice is responsible for generating reports based on materials retrieved from the `read_materials` microservice. It fetches material data through a **REST API**, stores reports in a **MariaDB database**, and provides endpoints for retrieving reports.

## 🚀 Features
- Fetches material data from the `read_materials` microservice.
- Stores generated reports in MariaDB.
- Provides an API endpoint to retrieve reports by subject.
- Implements logging using `loguru`.
- Supports Prometheus for monitoring and performance metrics.
- Dockerized for easy deployment.

## 📦 Requirements
- **Python 3.11+**
- **FastAPI** for API handling
- **SQLAlchemy** for database interactions
- **MariaDB** as the database
- **Docker** (optional, for containerized deployment)
- **Prometheus & Grafana** (optional, for monitoring)

## 📁 Project Structure
