# **🛍️ E-Commerce API** 🚀  

Welcome to the **E-Commerce API** – a powerful and flexible backend for managing products, categories, and orders! This **Django REST Framework (DRF)**-based API makes it easy to build and scale your online store.  

🔥 **Key Features:**  
✅ **Product & Category Management** – Add, update, delete, and retrieve products & categories effortlessly.  
✅ **Order Processing** – Create and manage customer orders with ease.  
✅ **Pagination** – Efficiently browse through large product and order lists.  
✅ **Automatic Category Assignment** – Assign or create categories dynamically.  

---

## **📂 Project Structure** 🏗️
```
ecommerce/
│── apps/
│   ├── models.py        # Database models for Category, Product, Order, OrderItem
│   ├── serializers.py   # DRF serializers for request/response handling
│   ├── views.py         # API views for handling requests
│   ├── urls.py          # URL routing for the API
│── config/
│   ├── settings.py      # Django project settings
│   ├── urls.py          # Main project URL configurations
│── manage.py
│── requirements.txt     # Project dependencies
│── README.md            # Project documentation
```

---

## **🚀 Getting Started**
### **1️⃣ Clone the Repository** 🔄
```bash
git clone https://github.com/rinkuo/Homework-3.git
cd config
```

### **2️⃣ Create a Virtual Environment** 🏗️
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### **3️⃣ Install Dependencies** 📦
```bash
pip install -r requirements.txt
```

### **4️⃣ Apply Database Migrations** 🗄️
```bash
python manage.py migrate
```

### **5️⃣ Run the Development Server** 🚀
```bash
python manage.py runserver
```

🎯 The API will be available at: **`http://127.0.0.1:8000/api/`**  

---

## **📌 API Endpoints** 🔗  
### **🛒 Products**
| Method | Endpoint | Description |
|--------|---------|-------------|
| 🟢 **GET** | `/api/products/` | List all products (paginated) |
| 🟡 **POST** | `/api/products/` | Create a new product |
| 🟢 **GET** | `/api/products/{id}/` | Retrieve a single product |
| 🔵 **PUT** | `/api/products/{id}/` | Update a product |
| 🔴 **DELETE** | `/api/products/{id}/` | Delete a product |

### **📦 Orders**
| Method | Endpoint | Description |
|--------|---------|-------------|
| 🟢 **GET** | `/api/orders/` | List all orders |
| 🟡 **POST** | `/api/orders/` | Create a new order |
| 🟢 **GET** | `/api/orders/{id}/` | Retrieve order details |

### **🚀 FUTURE UPDATE**
### **📂 Categories (Beta Test)**
| Method | Endpoint | Description |
|--------|---------|-------------|
| 🟢 **GET** | `/api/categories/` | List all categories |
| 🟡 **POST** | `/api/categories/` | Create a new category |
| 🔵 **PUT** | `/api/categories/{id}/` | Update a category |
| 🔴 **DELETE** | `/api/categories/{id}/` | Delete a category |

---

## **📝 Example API Requests**
### **🎯 Create a Product**
```json
{
    "name": "Smartphone X",
    "description": "Latest smartphone model",
    "price": 999.99,
    "stock": 50,
    "category": "Electronics"
}
```

### **🛍️ Create an Order**
```json
{
    "customer_name": "John Doe",
    "customer_email": "john@example.com",
    "customer_phone": "+1234567890",
    "shipping_address": "123 Main St, City, Country",
    "items": [
        {
            "product_id": 1,
            "quantity": 2
        }
    ]
}
```

---

## **⚙️ Technologies Used** 🛠️
🔹 **Django** – High-level Python web framework  
🔹 **Django REST Framework (DRF)** – API development  
🔹 **SQLite/PostgreSQL** – Database  
🔹 **Docker (Optional)** – Containerization  
🔹 **Gunicorn & Nginx (Optional)** – Production-ready setup  

---

## **🌟 Future Enhancements**
✨ **Authentication & User Roles** (Admin, Customer)  
✨ **Product Image Uploads** 📸  
✨ **Stripe/PayPal Integration** 💳  
✨ **Order Tracking & Notifications** 📬  

---

## **💬 Contact & Support** 📩  
📧 **Email:** rinkusoft77@gmail.com 
🔗 **GitHub:** [Rinkuo](https://github.com/rinkuo)  
