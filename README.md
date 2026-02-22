# 🛒 StyleHub — Full-Stack E-Commerce Platform

---

## 📅 Project Overview

**StyleHub** is a modern **full-stack e-commerce application** developed using **Django 6.0**, **Django REST Framework**, and **PostgreSQL**.
The project focuses on **real-world system design**, **clean architecture**, and **scalable workflows**, similar to production-level applications.

The goal was not only to build features, but to understand **how a real e-commerce system works internally**.

---
<img width="1920" height="1080" alt="Screenshot (399)" src="https://github.com/user-attachments/assets/a18dd175-1ba0-45d0-ad10-c5f77f71b2d7" />

<img width="1920" height="1080" alt="Screenshot (400)" src="https://github.com/user-attachments/assets/254683f7-1ba9-43ed-8038-02fbedd75e0e" />



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
