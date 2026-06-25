# Hestia 🍔🍕

Welcome to **Hestia**, a full-stack food ordering and delivery web application. The project is separated into a modern, responsive frontend built with **React** and a robust backend API powered by **Django**. It features a complete menu, user authentication, a functional shopping cart, and order history tracking.

## 📸 Demo Images

Here is a quick look at some of the delicious items available on Hestia:

<p align="center">
  <img src="imgs/medu-vada-1.jpg" alt="Medu Vada" width="30%">
  <img src="imgs/c1.jpg" alt="Food Image 1" width="30%">
  <img src="imgs/s1.webp" alt="Snack Image" width="30%">
</p>

## 🚀 Key Features

- **User Authentication:** Secure registration, login, and user profile management.
- **Dynamic Menu:** Browse different categories including Snacks and Beverages.
- **Shopping Cart:** Add, remove, and review items in the cart before checking out.
- **Order History:** Users can view their recent orders.
- **Responsive UI:** Clean, scroll-friendly interfaces tailored for a great user experience.

## 🛠️ Technology Stack

### Frontend (`Group Project/hestia`)
- **React.js (v18)** - Component-based UI creation.
- **React Router DOM** - Smooth, seamless navigation between pages.
- **Axios** - Handling REST API requests to the backend.
- **Icons:** A mix of FontAwesome, Lucide React, and React Icons for visual elements.

### Backend (`Group Project/hestiabackend`)
- **Django** - High-level Python web framework.
- **Django REST Framework (DRF)** - Building powerful Web APIs.
- **SQLite3** - Default database for quick setup and testing.
- **django-cors-headers** - Cross-Origin Resource Sharing handling.

## 📁 Project Structure

```text
Hestia/
├── Group Project/
│   ├── hestia/             # React Frontend codebase (src, public, package.json)
│   └── hestiabackend/      # Django Backend codebase (manage.py, apps)
│       ├── beverages/      # App handling beverages
│       ├── snacks/         # App handling snacks
│       ├── recentorder/    # App handling order history
│       └── user1/          # App handling user data and auth
└── imgs/                   # Image assets and demo images
```

## ⚙️ Local Development Setup

To run Hestia locally, you need to start both the backend server and the frontend application.

### Prerequisites
- [Node.js & npm](https://nodejs.org/) installed
- [Python 3.x](https://www.python.org/) installed

### 1. Backend Setup (Django)

1. Navigate to the backend directory:
   ```bash
   cd "Group Project/hestiabackend"
   ```
2. (Optional but recommended) Create and activate a virtual environment:
   ```bash
   # Windows
   python -m venv venv
   venv\Scripts\activate
   ```
3. Install the required Python packages (make sure Django, DRF, and CORS headers are installed):
   ```bash
   pip install django djangorestframework django-cors-headers
   ```
4. Apply database migrations:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```
5. Start the development server:
   ```bash
   python manage.py runserver
   ```
   *The backend API will run on `http://127.0.0.1:8000/`.*

### 2. Frontend Setup (React)

1. Open a new terminal and navigate to the frontend directory:
   ```bash
   cd "Group Project/hestia"
   ```
2. Install the Node modules:
   ```bash
   npm install
   ```
3. Start the React development server:
   ```bash
   npm start
   ```
   *The frontend will run on `http://localhost:3000/`.*

## 📌 Main API Endpoints
- `/api/` - User authentication and data.
- `/hestia/snacks/` - Snacks menu items.
- `/hestia/beverages/` - Beverages menu items.
- `/hestia/history/` - Recent user orders.
