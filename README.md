Inventory Management System
Overview
The Inventory Management System is a web application built with Django and Django REST Framework. It allows users to efficiently manage inventory, track stock levels, and generate reports.

Features
User Authentication: Secure login and registration for users.
Product Management: Admins can create, read, update, and delete products.
Stock Management: Track and manage stock levels for products.
Reporting: View total inventory value and filter products by category or stock level.
API Access: RESTful API for integration with other systems.


git clone https://github.com/yourusername/inventory-management-system.git
cd inventory-management-system


pip install -r requirements.txt

python manage.py migrate
python manage.py runserver



API Endpoints
Token Authentication:

POST /api-token-auth/ - Obtain authentication token.
Products:
GET /inventory/api/products/ - List all products.
POST /inventory/api/products/ - Create a new product.
GET /inventory/api/products/<id>/ - Retrieve a product by ID.
PUT /inventory/api/products/<id>/ - Update a product by ID.
DELETE /inventory/api/products/<id>/ - Delete a product by ID.
POST /inventory/api/products/<id>/add_stock/ - Add stock to a product.
POST /inventory/api/products/<id>/remove_stock/ - Remove stock from a product.
Stock Logs:

GET /inventory/api/stock_logs/ - List all stock logs.
POST /inventory/api/stock_logs/ - Create a new stock log.
