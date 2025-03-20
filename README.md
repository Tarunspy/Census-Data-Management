Census Data Management System on Heroku

Project Overview

This project is designed to manage demographic and income data using a PostgreSQL relational database. It includes a predictive model to determine if an individual earns more than $50,000 annually based on socio-economic attributes. The system includes:

🖥️ A RESTful API for CRUD operations

📊 An interactive Streamlit dashboard for data visualization

☁️ Deployment on Heroku for accessibility

1️⃣ Overview

🎯 Objective

The primary goal of this system is to store, process, and analyze census data to understand income trends and disparities. PostgreSQL ensures efficient data management with high scalability.

🛢️ Why Use a Database?

Scalability – Handles large datasets efficiently

Data Integrity – Ensures accuracy and consistency

Concurrency – Supports multiple user access

Advanced Queries – Enables powerful SQL-based data retrieval

👥 Target Users

Data Analysts & Researchers – To analyze income distribution patterns

NGOs & Policymakers – For socio-economic policy development

2️⃣ Database Architecture (PostgreSQL)

The system's database schema is structured into interrelated tables to capture various aspects of demographic and income data.

🔑 Key Tables

Individuals – Stores personal demographic details

Employment – Captures financial data (capital gains/losses)

JobDetails – Contains work class and occupation details

EducationDetails – Tracks educational background

RelationshipDetails – Manages marital status & family ties

IncomeDetails – Categorizes income (>50K or <=50K)

🔗 Database Design Features

BCNF Normalization – Eliminates redundancy for efficient storage

Foreign Key Constraints – Maintains data integrity using individual_id

📥 Bulk Data Processing – The system processes over 215K records using Python scripts for optimized insertion and management.

3️⃣ API Endpoints (CRUD Operations) 🛠️

The system supports RESTful API calls for seamless database interaction.

⚡ CRUD Operations

Create – Insert new records

Read – Retrieve data insights (e.g., income classification by demographics)

Update – Modify existing records

Delete – Remove records (with constraints on core tables)

🔌 API Implementation

FastAPI / Flask for API development

PostgreSQL as the backend database

Error Handling & Validation to ensure robust data integrity

4️⃣ Interactive Streamlit Dashboard 📊

A web-based interactive dashboard built with Streamlit provides real-time visualization and data management capabilities.

🎛️ Dashboard Features

Overview Panel – Displays income distribution statistics

Filter Options – Select datasets between 5K – 50K rows

Data Export – Allows exporting results to Excel

Visualization Tools – Graphs & bar charts for income analysis

📡 Technologies Used

Streamlit – UI development

Pandas – Data processing

Matplotlib & Seaborn – Data visualization

🚀 Deployment & Execution

🏗️ Steps to Run the Project

1️⃣ Database Setup – Install and configure PostgreSQL

2️⃣ Install Dependencies – Python libraries: psycopg2, streamlit, requests

3️⃣ Run API & App – Launch the Streamlit dashboard

4️⃣ Deploy on Heroku – Ensure a live production environment

☁️ Deployment Stack

Heroku – Cloud hosting

PostgreSQL – Database backend

GitHub – Version control & collaboration

🏁 Conclusion

This project offers a scalable, interactive, and efficient approach to managing census data. By integrating a PostgreSQL database, a RESTful API, and a Streamlit dashboard, it provides a robust tool for data-driven decision-making. With Heroku deployment, the system remains accessible and scalable for real-world applications.

🔗 Reference

📜 Census Income Dataset: https://archive.ics.uci.edu/dataset/20/census+income
