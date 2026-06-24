# xrwvm-fullstack_developer_capstone

## Project Name: Car Dealership Evaluation and Review Portal

Welcome to the **Car Dealership Evaluation and Review Portal**, the final capstone project for the Full Stack Web Developer program. This application is a fully integrated web platform that allows users to view car dealerships across the United States, read authentic customer reviews, submit their own dealership feedback, and leverage an AI-driven sentiment analysis microservice.

---

## 🚀 Project Overview
The application is built using a modern full-stack architecture, featuring a robust Django backend framework combined with a dynamic React user interface. To provide scalability, dealer and review data are managed via a NoSQL database, while a containerized IBM Watson/Sentiment Analysis microservice processes user reviews on the fly.

### Key Features
* **User Authentication:** Complete registration, login, and logout capabilities using Django sessions and React components.
* **Dealership Directory:** Dynamic lookup and filtering of nationwide car dealerships by state (e.g., Kansas).
* **Review & Sentiment Analytics:** Integration with an external sentiment microservice to classify user review text as positive, neutral, or negative.
* **Car Model Management:** Built-in Django models handling complex relationships between Car Makes and Car Models.
* **CI/CD Pipeline:** Automated testing and build workflows executed seamlessly via GitHub Actions.

---

## 🛠️ Tech Stack & Architecture

* **Frontend:** React.js, Vite, HTML5, CSS3 (Bootstrap)
* **Backend:** Django Framework (Python)
* **Database:** SQLite (for Django Admin & Car Inventory), NoSQL/Cloudant (for Dealers and Reviews)
* **Microservices:** Python-based Sentiment Analysis API containerized with Docker
* **CI/CD:** GitHub Actions

---

## 📂 Project Structure

```text
xrwvm-fullstack_developer_capstone/
├── djangoproj/                 # Main Django project configuration
├── djangoapp/                  # Django application backend (Views, Models, Controllers)
│   ├── models.py               # Car Make and Car Model definitions
│   ├── urls.py                 # API endpoints and routing
│   └── views.py                # Request handling logic & proxying to microservices
├── server/
│   └── frontend/
│       ├── src/                # React source code
│       │   └── components/     # UI Components (Register, Login, Dealers)
│       └── static/             # Static pages (About.html, Contact.html)
└── .github/
    └── workflows/              # GitHub Actions CI/CD configuration
