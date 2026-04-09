# 🚀 Big Data Analytics - Course Laboratory

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Apache Spark](https://img.shields.io/badge/Apache_Spark-E25A1C?style=for-the-badge&logo=apache-spark&logoColor=white)
![Apache Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=for-the-badge&logo=apache-kafka&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

## 📌 Overview
This repository contains all laboratory exercises, projects, and assignments for the **Big Data** course. It demonstrates practical implementations of distributed data processing, real-time data streaming, and scalable analytics using modern big data architectures.

## 🛠️ Technology Stack
* **Data Processing:** PySpark (Apache Spark API)
* **Message Broker / Streaming:** Apache Kafka (KRaft mode)
* **Containerization:** Docker & Docker Compose
* **Environment:** WSL (Ubuntu), Python Virtual Environment
* **Development Tool:** Jupyter Lab / Jupyter Notebook

## 👥 The Team
* **Trần Trung Kiên**
* **Huỳnh Hữu Nhật**

---

## 📂 Repository Structure

The repository is organized by laboratory modules. Each folder contains its own specific instructions, datasets, and source code.

```text
.
├── Lab_01/
│   ├── docker-compose.yaml     # Kafka Cluster containerization
│   ├── setup.ipynb             # Kafka topic creation & data ingestion
│   ├── lab_01_exercise.ipynb   # PySpark data analysis & processing
│   ├── input/                  # Raw sample datasets (Movies, Ratings, Tags)
│   └── output_exercise/        # Processed data output (JSON format)
│
├── Lab_02/                     # (Upcoming module)
├── Lab_03/                     # (Upcoming module)
│
├── .gitignore                  # Ignored files (venv, checkpoints, etc.)
├── requirements.txt            # Python dependencies
└── README.md                   # This file

## 🚀 Getting Started

### 1. Prerequisites

Ensure you have the following installed on your local machine:
* **Docker Desktop** (with WSL 2 enabled if on Windows)
* **Python 3.10+**
* **Git**

### 2. Installation & Setup

Clone this repository to your local machine:

'''bash
    git clone <YOUR_GITHUB_REPO_URL_HERE>
    cd big_data_course
'''

Set up the virtual environment and install required dependencies:

'''bash
    python -m venv .venv_wsl
    source .venv_wsl/bin/activate  # On Linux/WSL
    pip install -r requirements.txt
'''

### 3. Running a specific Lab

Navigate to the specific lab directory and follow its workflow. For instance, to run Lab 01 (Kafka & Spark integration):

'''bash
    cd Lab_01

    # 1. Start the local Kafka Cluster (3 Brokers in KRaft mode)
    docker compose --profile kafka up -d

    # 2. Launch Jupyter Lab to execute the notebooks
    jupyter lab
'''

*Note: Always remember to shut down Docker containers after finishing the lab to free up memory*