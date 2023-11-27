# Vender_Management
Vendor Management is a Django-based web application that allows users to manage vendors and purchase orders efficiently. It provides a RESTful API for performing CRUD operations on vendors and purchase orders, along with additional features such as vendor performance tracking and purchase order acknowledgment.

API Endpoints:
List all the API endpoints along with their functionalities. For example:

Vendors:

GET /api/vendors/: Get a list of all vendors.
POST /api/vendors/: Create a new vendor.
GET /api/vendors/{id}/: Get details of a specific vendor.
PUT /api/vendors/{id}/: Update details of a specific vendor.
DELETE /api/vendors/{id}/: Delete a specific vendor.

Purchase Orders:

GET /api/purchase-orders/: Get a list of all purchase orders.
POST /api/purchase-orders/: Create a new purchase order.
GET /api/purchase-orders/{id}/: Get details of a specific purchase order.
PUT /api/purchase-orders/{id}/: Update details of a specific purchase order.
DELETE /api/purchase-orders/{id}/: Delete a specific purchase order.

Vendor Performance:

GET /api/vendors/{id}/performance/: Get performance metrics for a specific vendor.
Purchase Order Acknowledgment:

POST /api/purchase-orders/{id}/acknowledge/: Acknowledge a purchase order.

Installation:
Provide instructions on how to install and set up your project. Include information on dependencies and how to run migrations. For example:

# Clone the repository
git clone https://github.com/yourusername/Vendor_Management.git

# Navigate to the project directory
cd Vendor_Management

# Install dependencies
pip install -r requirements.txt

# Run migrations
python manage.py migrate

mention the need to configure the database settings or API authentication.

Running the Application:
Provide information on how to run the Django development server:
python manage.py runserver

 use postman for get the details with url and  token number // to use all the properties put patch get delete can use on Postman
 http://127.0.0.1:8000/api/vendors/  Authorization  token c26c28fcb187d88c00bae4adcb3da7f3db95fa33

 To create new vender
 curl -X POST -H "Content-Type: application/json" -d '{"name": "Vendor XYZ", "location": "City"}' http://127.0.0.1:8000/api/vendors/
 
 Create super User to login admin panel 
 http://127.0.0.1:8000/admin/             //id = admin   ,   password = admin  You can also login from  this id password 
 OR create New Id to  run the  following command 
 python manage.py createsuperuser
