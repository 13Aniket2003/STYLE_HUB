# 🛒 StyleHub — Full-Stack E-Commerce Platform

---

## 📅 Project Overview

**StyleHub** is a modern **full-stack e-commerce application** developed using **Django 6.0**, **Django REST Framework**, and **PostgreSQL**.
The project focuses on **real-world system design**, **clean architecture**, and **scalable workflows**, similar to production-level applications.

The goal was not only to build features, but to understand **how a real e-commerce system works internally**.

---

<img width="2879" height="1384" alt="552804972-d017469b-4843-428f-bb4d-2f241a9cb487" src="https://github.com/user-attachments/assets/ee7bca5e-a6e4-4527-b13c-ffdf4ad7600d" />

<img width="2879" height="1534" alt="552805421-8aa784b8-d195-4d7e-91e3-e05a3266b8c2" src="https://github.com/user-attachments/assets/3b186c13-e3ff-43a0-846b-d6bc8fc83d4c" />

<img width="2879" height="1526" alt="552805101-94e95b7e-529a-4183-bb51-6cceab79a3c2" src="https://github.com/user-attachments/assets/a4c7319c-12d7-409c-9b82-d8aa826cce46" />


<img width="2879" height="1540" alt="552804741-38020464-0304-451c-8806-a719fca16493" src="https://github.com/user-attachments/assets/2c3ffd55-b25a-4130-a81c-fe3b63b0293f" />


<img width="2879" height="1214" alt="552805867-6c733056-60b2-4ff3-a867-6e982658ce9f" src="https://github.com/user-attachments/assets/88d2ddf2-48bb-4562-8ed0-5e0ed21e25b4" />

<img width="2870" height="1538" alt="552806033-1e170f7d-c8cf-40b3-845f-53051f83e752" src="https://github.com/user-attachments/assets/d61fd06c-befb-4e27-8408-2bbba51e287c" />

<img width="2879" height="1535" alt="552805542-06af2804-9101-4ef6-bce4-abe7980a2078" src="https://github.com/user-attachments/assets/dc849f54-bb26-4488-b028-517b4c4d4ece" />

<img width="2879" height="1533" alt="552806290-45aabe53-9b42-4227-8e4c-6b41d192ddc4" src="https://github.com/user-attachments/assets/abf91830-92bb-47ab-8a00-18721eb5c8e7" />

<img width="2879" height="1508" alt="552805691-e0b55321-40bf-47a1-a5d3-d62cdf7e6e92" src="https://github.com/user-attachments/assets/cb2c001d-4e10-4871-a9c9-5adefb3369e1" />

<img width="2871" height="1441" alt="552806164-95cb92d3-c005-46a8-957e-221fe2a3aae7" src="https://github.com/user-attachments/assets/78de6e01-cbdc-49cc-8dcb-15100084fbc3" />

## 🧠 What is StyleHub?

StyleHub is a **complete shopping platform** where users can:

* Browse products
* Add items to cart
* Place orders
* Track purchases
* Manage profiles
* Experience a premium UI with light & dark themes

Admins can manage products, stock, and orders from a powerful backend dashboard.

---

## 🚀 Core Features Implemented

### 🎨 Modular UI Design

* Page-specific CSS loading
* 11 optimized stylesheets
* Clean, minimal, Apple-inspired layout
* Faster load times and better maintainability

---

### 🌓 Light & Dark Theme Support

* Theme preference stored in browser
* Automatically applied on page load
* Instant toggle without refresh
* Implemented using CSS variables

---

### ⚡ Real-Time User Interactions

* AJAX-powered “Add to Cart”
* No page reload during cart updates
* Smooth slide-in notifications
* Better user experience and responsiveness

---

### 🔐 Secure Authentication System

* Session-based authentication for users
* Token-based authentication for APIs
* Protected routes for orders, cart, and profile
* Secure access control across the platform

---

### 👤 Automated User Profile Creation

* User profile generated instantly on signup
* Implemented using Django Signals
* Eliminates manual profile handling
* Ensures consistent user data

---

## 🧩 Core Functional Modules

### 🛍️ Product Management

* Product categories
* Product images & descriptions
* Price and stock handling
* Admin-controlled visibility

---

### 🛒 Cart System

* Add/remove products dynamically
* Quantity management
* Cart persists per user
* Seamless checkout flow

---

### 📦 Order Management

* Order creation after checkout
* Order status tracking
* User-specific order history
* Admin approval and cancellation

---

### 🔄 Inventory Automation

* Stock reduces automatically after order placement
* Stock restores when order is cancelled
* Prevents over-selling
* Maintains data integrity

---

## 🗂️ Project Architecture Explained

### 🧠 Backend Configuration (stylehub/)

Acts as the **brain of the project**.

* Global settings and configurations
* Secure environment-based variables
* URL routing for all modules
* Serializer layer for API communication

---

### 🏪 Store Application (store/)

Handles **all business logic**.

Includes:

* Product & category models
* Cart and order logic
* User profiles & wishlist
* Views managing user journeys

---

### 🖥️ Frontend Templates (templates/)

* 19 structured HTML templates
* Built using Django Template Language
* Marketing pages, cart pages, dashboards
* Reusable layout components

---

### 🎯 Static Assets (static/)

* Modular CSS architecture
* JavaScript for:

  * Theme switching
  * Animations
  * Secure background requests
* Only required assets load per page

---

## ⚙️ Environment & Security Design

### 🔐 Environment Variables

All sensitive data is stored securely using environment variables:

* Database credentials
* Secret keys
* Debug configuration
* Email credentials

This ensures:

* Security
* Clean codebase
* Safe deployment
* Easy team collaboration

---

## ✉️ Email Integration

* Gmail SMTP configured
* Ready for notifications and alerts
* Credentials managed securely
* Extendable for future features

---

## 🧪 Reliability & Best Practices

* Django Signals for automation
* Clean separation of concerns
* Defensive checks for data consistency
* Admin-level control for safety

---

## 🛠️ Development Philosophy

* Clean & readable structure
* Modular and scalable design
* Production-oriented mindset
* Real-world workflows over demo logic

This project is structured like a **company-level codebase**, not a basic tutorial.

---
## ✨ Key Features

### 🛒 Customer Experience

* **🌓 Adaptive Theming:** Native Dark/Light mode support with persistent user preferences.
* **⚡ Dynamic Discovery:** JavaScript-powered filtering by price, size, and category with zero page reloads.
* **💳 Secure Checkout:** Fully integrated with **Stripe API** for secure, PCI-compliant payment processing.
* **📦 Order Lifecycle:** Full checkout simulation, real-time order tracking, and automated email notifications.
* **❤️ Wishlist & Cart:** Persistent storage for user favorites and a seamless multi-item checkout flow.

### ⚙️ Custom Admin Dashboard (`/custom-admin/`)

* **📊 Business Intelligence:** Real-time metrics for total revenue, order volume, and product inventory.
* **🚀 Bulk Operations:** Quickly categorize inventory with comma-separated tag inputs.
* **🎯 Visibility Control:** One-click toggles to feature products on the Homepage, New Arrivals, or the Main Shop.

---

## 🛠️ Tech Stack

* **Backend:** Python 3.11+, Django 6.0+
* **Payments:** Stripe API (Python Library)
* **Database:** PostgreSQL (Production), SQLite (Development/CI)
* **Frontend:** HTML5, CSS3 (Modular CSS Variables), Vanilla JavaScript
* **Auth & Security:** Django Identity & GitHub Actions CI/CD
* **Communications:** SMTP Integration for transactional emails

---

## 🚀 Installation & Setup

### 1. Clone & Environment

```bash
git clone https://github.com/yourusername/stylehub.git
cd stylehub
python -m venv venv
source venv/bin/activate  # Mac/Linux
# venv\Scripts\activate  # Windows

```

### 2. Dependencies & Environment Variables

Install the core requirements:

```bash
pip install -r requirements.txt

```

Create a `.env` file in the root directory and add your credentials (do not commit this file!):

```env
DEBUG=True
SECRET_KEY=your_secret_key

# Database
DB_NAME=stylehub_db
DB_USER=postgres
DB_PASSWORD=your_password

# Stripe Keys
STRIPE_PUBLIC_KEY=pk_test_your_public_key
STRIPE_SECRET_KEY=sk_test_your_secret_key

# Email
EMAIL_USER=your-email@gmail.com
EMAIL_PASSWORD=your-app-password

```

### 3. Database Initialization

```bash
python manage.py makemigrations
python manage.py migrate
python manage.py createsuperuser

```

### 4. Launch

```bash
python manage.py runserver

```

---

## 📁 Project Architecture

```text
├── core/               # Project settings & WSGI
├── store/              # Main application logic
│   ├── models.py       # Product, Cart, Order, UserProfile
│   ├── views.py        # Logic for Storefront, Stripe Checkout & Admin
│   └── templates/      # Split into /shop and /admin_custom
├── static/
│   ├── css/            # Modular style1.css to style11.css
│   └── js/             # Filtering, Stripe Elements, & Theme logic
└── .github/workflows/  # CI/CD Pipeline configuration

```

---

## 👥 Core Team

* **Sadgyan ji Jaiswal** — *Frontend Architect*
* **P.V.S Narayana Murthy** — *Backend Systems*
* **Bhanu Teja Sangula** — *Database & Admin Logic*
* **Aniket Dutta** — *DevOps & Deployment*

---

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](https://www.google.com/search?q=LICENSE) file for details.

---

## 📈 Future Enhancements

* Online payment gateway
* Order tracking system
* Product reviews & ratings
* Admin analytics dashboard
* Docker & CI/CD integration
* Mobile-ready API expansion

---

## 🏁 Final Note

**StyleHub** demonstrates a complete understanding of:

* Backend development with Django
* API design using DRF
* Database handling with PostgreSQL
* UI/UX structuring
* Secure, scalable system design

It is **deployment-ready** and designed with **industry standards** in mind.
