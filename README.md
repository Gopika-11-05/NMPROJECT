PRODUCT CATALOG WITH MONGODB
A simple yet powerful Product Catalog application built with Node.js, Express, and MongoDB.
It allows users to manage products — including creating, reading, updating, and deleting (CRUD) product entries — stored in a MongoDB database.

Features:
Product Management (CRUD) — Add, view, update, and delete products
Search & Filter — Find products by name, category, or price range
MongoDB Integration — Efficient, scalable data storage
RESTful API — Easy to connect with any frontend (React, Vue, Angular, etc.)

Validation & Error Handling — Clean, predictable responses

JSON-based API — Lightweight and flexible

Tech Stack
Layer	Technology
Backend	Node.js, Express.js
Database	MongoDB (Mongoose ORM)
Environment	dotenv
API Testing	Postman / cURL
Installation
1️⃣ Clone the Repository
git clone https://github.com/yourusername/product-catalog-mongodb.git
cd product-catalog-mongodb

2️⃣ Install Dependencies
npm install

3️⃣ Set Up Environment Variables

Create a .env file in the project root:

PORT=5000
MONGO_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/catalog

 Start the Server
npm start
Server will run on http://localhost:5000
 API Endpoints
Method	Endpoint	Description
GET	/api/products	Get all products
GET	/api/products/:id	Get a product by ID
POST	/api/products	Add a new product
PUT	/api/products/:id	Update a product
DELETE	/api/products/:id	Delete a product
Example Product Object
{
  "name": "Wireless Headphones",
  "description": "Noise-cancelling Bluetooth headphones",
  "category": "Electronics",
  "price": 99.99,
  "stock": 25
}

 Project Structure:
product-catalog-mongodb/
├── models/
│   └── Product.js
├── routes/
│   └── productRoutes.js
├── config/
│   └── db.js
├── .env
├── server.js
├── package.json
└── README.md

 Future Enhancements:
 Add product categories & subcategories
 Image uploads using Cloudinary or AWS S3
 User authentication & roles (Admin / Viewer)
 Pagination & sorting
