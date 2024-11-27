# Django_Project

[![CI](https://github.com/NoManNayeem/Django_Project/actions/workflows/ci.yml/badge.svg)](https://github.com/NoManNayeem/Django_Project/actions/workflows/ci.yml)

A sample Django application showcasing CI/CD implementation using GitHub Actions and AWS. This project demonstrates creating, containerizing, and automating deployments for a Python-based web application.

---

## **Project Structure**

```
Django_Project/
├── core/                  # Sample Django app
├── myapp/                 # Django project settings
├── Dockerfile             # Docker configuration
├── docker-compose.yml     # Docker Compose configuration
├── requirements.txt       # Project dependencies
├── manage.py              # Django management script
└── README.md              # Project documentation
```

---

## **Getting Started**

### **Prerequisites**
- Python 3.10+
- Docker and Docker Compose
- Git

### **Setup Instructions**

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/NoManNayeem/Django_Project.git
   cd Django_Project
   ```

2. **Set Up a Virtual Environment:**
   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Application Locally:**
   ```bash
   python manage.py runserver
   ```

5. **Run the Application in Docker:**
   ```bash
   docker-compose up --build
   ```

   Access the app at `http://127.0.0.1:8000`.

---

## **CI/CD Pipeline**

This project includes a CI/CD pipeline configured with GitHub Actions.

### **CI Pipeline**
- Automatically tests the application on every push to the `main` branch.
- Configuration file: `.github/workflows/ci.yml`

### **CD Pipeline**
- Automates deployment to AWS EC2.
- Configuration file: `.github/workflows/cd.yml`

---

## **Contributing**

Contributions are welcome! Feel free to open issues or submit pull requests to improve the project.

---

## **License**

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## **Contact**

For questions or support, please contact [NoManNayeem](https://github.com/NoManNayeem).
