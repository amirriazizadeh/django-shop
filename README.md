# django-shop
A fully featured e-commerce web application built with Django.
🛍️ Django E-Commerce Shop

This repository contains the official Django backend for a classic e-commerce website (non-API version).
The project includes user authentication, product management, cart & order system, and a clean, extensible architecture.

🚀 Getting Started

Follow the steps below to set up and run the project locally for development or testing.

✅ Prerequisites

Make sure you have the following installed:

Python 3.8+

pip

Django

Git

(Optional) Docker & Docker Compose

⚙️ Installation & Local Setup
1. Clone the repository
git clone <repository-url>
cd django-ecommerce

2. Create & activate virtual environment
python -m venv venv
source venv/bin/activate   # macOS/Linux
venv\Scripts\activate      # Windows

3. Install dependencies
pip install -r requirements.txt

4. Apply database migrations
python manage.py migrate

5. Create superuser
python manage.py createsuperuser

6. Run the development server
python manage.py runserver


Your app will be available at:
👉 http://127.0.0.1:8000

🌍 Environment Variables

Create a .env file in the project root:

DEBUG=True
SECRET_KEY=your-secret-key
ALLOWED_HOSTS=localhost,127.0.0.1

# Database (if using PostgreSQL instead of SQLite)
DB_NAME=shopdb
DB_USER=postgres
DB_PASSWORD=yourpassword
DB_HOST=localhost
DB_PORT=5432


⚠️ Ensure .env is included in .gitignore.

🐳 Docker Support (Optional)
Build & run containers
docker-compose up --build


The website will be reachable at:
👉 http://localhost:8000

🧪 Running Tests
python manage.py test

📂 Project Structure
django-ecommerce/
│
├── accounts/        → ثبت‌نام، ورود، مدیریت پروفایل کاربران
├── cart/            → مدیریت سبد خرید
├── core/            → فایل‌های مشترک، کانفیگ‌های پایه، BaseModel
├── orders/          → سفارش‌ها، وضعیت سفارش، فاکتور
├── products/        → محصولات، دسته‌بندی‌ها، موجودی، تصاویر
│
├── templates/       → قالب‌های HTML پروژه
├── static/          → CSS ،JS ،Images
│
├── config/          → تنظیمات اصلی پروژه (settings, urls, wsgi, asgi)
└── manage.py

📌 Features

🔐 User Authentication (login, registration, sessions)

🛒 Shopping Cart

📦 Order Management

🏷️ Product & Category Management

🎨 Template-based Frontend

🗂️ Clean & modular structure

🐳 Optional Docker support

🧼 Customizable admin panel

🤝 Contributing

Pull requests are welcome!
For major updates, please open an issue first to discuss changes.

📜 License

This project is licensed under the MIT License.