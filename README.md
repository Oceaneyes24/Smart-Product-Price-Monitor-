
# Smart-Product-Price-Monitor-
Smart Price Monitor is a FastAPI-based competitor pricing platform that helps businesses track, compare, and analyze product prices across marketplaces. It features JWT authentication, product management, price history tracking, and interactive analytics dashboards.
# Smart Price Monitor

Smart Price Monitor is a FastAPI-based competitor pricing platform that helps businesses track, compare, and analyze product prices across marketplaces. It features JWT authentication, product management, price history tracking, and interactive analytics dashboards.

---

## Features

### Authentication

* User Registration
* User Login
* JWT-Based Authentication
* Protected Routes
* Logout Functionality

### Product Management

* Add Products
* Edit Products
* Delete Products
* View Product Catalog

### Price Monitoring

* Track Your Product Price
* Monitor Amazon Prices
* Monitor Flipkart Prices
* Compare Competitor Pricing
* Identify Better Pricing Opportunities

### Price Analytics

* Historical Price Tracking
* Automatic Price History Updates
* Interactive Trend Visualization
* Competitor Comparison Charts

### Dashboard

* Responsive Interface
* Product Statistics
* Analytics Widgets
* Interactive Charts

---

## Screenshots

### Login Page

![Login Page](screenshots/login.png)

### Registration Page

![Registration Page](screenshots/signup.png)

### Dashboard

![Dashboard](screenshots/dashboard.png)

### Add Product

![Add Product](screenshots/add-product.png)

### Edit Product

![Edit Product](screenshots/edit-product.png)

### Price Analytics

![Price Analytics](screenshots/chart.png)

---

## Technology Stack

### Backend

* FastAPI
* Python
* SQLAlchemy
* SQLite
* JWT Authentication
* Passlib

### Frontend

* HTML
* CSS
* JavaScript
* Jinja2
* Chart.js

### Tools

* VS Code
* Git
* GitHub

---

## Project Structure

```text
smart-price-monitor/
│
├── main.py
├── auth.py
├── database.py
├── models.py
├── schemas.py
├── requirements.txt
│
├── templates/
│   ├── login.html
│   ├── signup.html
│   ├── index.html
│   └── edit.html
│
├── static/
│   └── style.css
│
└── screenshots/
```

## Installation

### Clone Repository

```bash
git clone https://github.com/<username>/smart-price-monitor.git
cd smart-price-monitor
```

### Create Virtual Environment

Windows

```bash
python -m venv venv
venv\Scripts\activate
```

Linux/macOS

```bash
python3 -m venv venv
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Application

```bash
uvicorn main:app --reload
```

### Open Browser

```text
http://127.0.0.1:8000
```

---

## Database Schema

### Users

| Field           | Type    |
| --------------- | ------- |
| id              | Integer |
| username        | String  |
| hashed_password | String  |

### Products

| Field          | Type    |
| -------------- | ------- |
| id             | Integer |
| product_name   | String  |
| your_price     | Float   |
| amazon_price   | Float   |
| flipkart_price | Float   |

### Price History

| Field          | Type    |
| -------------- | ------- |
| id             | Integer |
| product_id     | Integer |
| day            | String  |
| your_price     | Float   |
| amazon_price   | Float   |
| flipkart_price | Float   |

---

## Workflow

1. User registers or logs in.
2. JWT authentication validates access.
3. User adds products and pricing details.
4. Product data is stored in the database.
5. Price history is automatically recorded.
6. Updates generate new historical entries.
7. Analytics charts visualize pricing trends.

---

## Future Enhancements

* Automated Web Scraping
* Email Price Alerts
* AI-Based Price Prediction
* Product Search and Filtering
* CSV/PDF Export
* PostgreSQL Integration
* Cloud Deployment
* Multi-User Product Ownership

---

## Contributors

* Sneha Pawar
* Sneha Gadhave
* Swayambhu Swami
* Manavi Tamkhane
* Rohit Arya
* Nupur Patankar

MIT ADT University, Pune

---

## License

This project is developed for educational and academic purposes.
