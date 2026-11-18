Backend-Assignment-3
Inventory and Data Management System
A RESTful Inventory Management System built using Node.js, Express.js, MongoDB, and Mongoose. This application helps manage product records, track stock levels, filter and sort products, generate low-stock alerts, and create category-wise inventory reports.

Features
Product Management (CRUD)

Create new products
Retrieve all products
Retrieve a single product by ID
Update product details
Delete products
Filtering, Sorting & Pagination

Filter products by category and brand
Search products by name or SKU
Filter products by minimum and maximum price
Sort products by name, price, quantity, and creation date
Retrieve products using pagination
Stock Management

Restock products
Record product sales
Prevent stock from becoming negative
Validate stock adjustment quantities
Inventory Reports

Low-stock alert report
Category-wise inventory summary
Total products and stock quantity
Total inventory value
Validation & Error Handling

Mongoose schema validation
Required fields and unique SKU
Price and quantity validation
Centralized error-handling middleware
Environment variable configuration using dotenv
Tech Stack
Technology	Purpose
Node.js	JavaScript runtime
Express.js	Backend framework
MongoDB	NoSQL database
Mongoose	MongoDB object modeling
dotenv	Environment configuration
Postman	API testing
Project Structure
Inventory-Data-Management-System/
│
├── config/
│   └── db.js
│
├── controllers/
│   └── productController.js
│
├── middleware/
│   └── errorMiddleware.js
│
├── models/
│   └── Product.js
│
├── routes/
│   └── productRoutes.js
│
├── .env
├── .gitignore
├── package.json
├── package-lock.json
├── server.js
└── README.md
Installation & Setup
1. Clone the Repository
git clone <YOUR_GITHUB_REPOSITORY_URL>
2. Navigate to the Project Folder
cd Inventory-Data-Management-System
3. Install Dependencies
npm install
4. Configure Environment Variables
Create a .env file in the root directory.

MONGO_URI=mongodb://127.0.0.1:27017/inventory_db
PORT=3000
Make sure MongoDB is running before starting the application.

5. Start the Server
Development mode:

npm run dev
Normal mode:

npm start
Server will run at:

http://localhost:3000
API Endpoints
Base URL:

http://localhost:3000/api/products
Product CRUD Operations
Method	Endpoint	Description
POST	/api/products	Create a product
GET	/api/products	Get all products
GET	/api/products/:id	
postman-get
5ef43093-4681-448a-9b8f-831f693fc821
postman-get-by_id
3b2b97e4-e34f-497c-87c3-c7629042466f
postman-post
76fbe7c3-81d1-4786-bea4-e6f4207dc5a5
postman-put
e5b59dbc-ad72-4513-b50a-dee6b90cc0af
postman-delete
2b827f22-43b2-4077-846f-df2b4d60eabe
postman-low-stock
32a5d324-5c10-4426-9cd8-b58344d6018a
postman-category-summery
42832e1d-8e15-4f96-84da-f7264e71206b
postman-patch
01a8e308-1f5a-4301-a38c-03f5378dcb80