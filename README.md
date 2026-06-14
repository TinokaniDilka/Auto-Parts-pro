
# AutoParts Pro - Vehicle Spare Parts Management System

A full-stack MERN (MongoDB, Express.js, React, Node.js) web application for managing vehicle spare parts, services, and customer operations.

## Screenshots
<img width="1789" height="837" alt="image" src="https://github.com/user-attachments/assets/cb31e1bb-f300-4219-8c11-eb19458f73b5" />

## 1. Sign Up Page
<img width="1882" height="869" alt="image" src="https://github.com/user-attachments/assets/cbdd87a4-7a62-4892-8cbd-f30eee11e31f" />
<img width="1834" height="834" alt="image" src="https://github.com/user-attachments/assets/f8bfeb60-2cb6-4be0-b0b7-3e162c7cd1aa" />

## 2. Login Page
<img width="1804" height="872" alt="image" src="https://github.com/user-attachments/assets/9682ceaa-4fcf-411b-9fc0-fdca79237930" />

## 3. Customer Dashboard
<img width="1794" height="830" alt="image" src="https://github.com/user-attachments/assets/566996ef-14ce-474c-9164-c7d3c1796d2e" />

## Products
<img width="1809" height="916" alt="image" src="https://github.com/user-attachments/assets/f7379c3c-2bae-4944-bbf0-75b1dc927b6f" />
<img width="1819" height="852" alt="image" src="https://github.com/user-attachments/assets/b6a91407-2996-4775-a0f2-85219054defc" />
<img width="1800" height="885" alt="image" src="https://github.com/user-attachments/assets/c7c2862e-8976-4b7d-8c79-86bf290474fa" />
<img width="1766" height="867" alt="image" src="https://github.com/user-attachments/assets/0b5cee3e-0390-44d8-beb4-3998ba05c6ca" />

## Services
<img width="1824" height="902" alt="image" src="https://github.com/user-attachments/assets/c794d486-9b9b-49aa-a130-1a2269634c2d" />
<img width="1790" height="857" alt="image" src="https://github.com/user-attachments/assets/48655074-935d-456f-9239-c276cef0c987" />
<img width="1779" height="730" alt="image" src="https://github.com/user-attachments/assets/1f76685a-0bff-4509-8a89-d85620ecf493" />
<img width="1793" height="728" alt="image" src="https://github.com/user-attachments/assets/b1458fc3-c354-4c66-8baa-4e3c0f0a783a" />

## My Orders
<img width="1805" height="887" alt="image" src="https://github.com/user-attachments/assets/d7f69246-3719-4818-835c-1b3c7512702c" />

## Order History
<img width="1730" height="699" alt="image" src="https://github.com/user-attachments/assets/9fdd7ddb-f699-4ca3-86a4-11f76f3f1579" />

## My Bookings
<img width="1773" height="840" alt="image" src="https://github.com/user-attachments/assets/c53829c3-1d97-464d-9523-e355de708dbd" />

## My Wishlist
<img width="1751" height="861" alt="image" src="https://github.com/user-attachments/assets/e62d21a6-addb-45d9-9514-1a4faa34e710" />



## Modules

| Module |
|--------|
| Order and Delivery Management
| Feedback and Warranty Management
| Supplier Management 
| Spare Parts/Product Management
| Service and Booking Management 
| Stocks and Inventory Management

## Features

### Customer Features
- Browse and search spare parts by category, vehicle type, brand
- Add products to cart and checkout
- Track orders and delivery status
- Book vehicle services online
- Submit product reviews and ratings
- File warranty claims

### Admin Features
- Manage products, inventory, and suppliers
- Process orders and update delivery status
- Manage service bookings
- Moderate customer reviews
- Handle warranty claims
- View dashboard with business insights

## Prerequisites

- Node.js (v18 or higher)
- MongoDB (local installation or MongoDB Atlas)
- npm or yarn

## Installation

### 1. Clone the repository
```bash
cd "my project"
```

### 2. Install Backend Dependencies
```bash
cd backend
npm install
```

### 3. Install Frontend Dependencies
```bash
cd ../frontend
npm install
```

### 4. Configure Environment Variables

Edit the `backend/.env` file:
```env
PORT=5000
MONGODB_URI=mongodb://localhost:27017/autoparts_db
JWT_SECRET=your_super_secret_key_change_this
NODE_ENV=development
```

For MongoDB Atlas, use your connection string:
```env
MONGODB_URI=mongodb+srv://username:password@cluster.mongodb.net/autoparts_db
```

## Running the Application

### Start MongoDB (if using local installation)
```bash
mongod
```

### Start Backend Server
```bash
cd backend
npm run dev
```
The server will run on http://localhost:5000

### Start Frontend Development Server
```bash
cd frontend
npm run dev
```
The frontend will run on http://localhost:3000

## Project Structure

```
my project/
├── backend/
│   ├── config/
│   │   └── db.js
│   ├── controllers/
│   │   ├── authController.js
│   │   ├── productController.js
│   │   ├── orderController.js
│   │   ├── supplierController.js
│   │   ├── inventoryController.js
│   │   ├── serviceController.js
│   │   ├── bookingController.js
│   │   ├── reviewController.js
│   │   └── warrantyController.js
│   ├── middleware/
│   │   └── authMiddleware.js
│   ├── models/
│   │   ├── User.js
│   │   ├── Product.js
│   │   ├── Order.js
│   │   ├── Supplier.js
│   │   ├── Inventory.js
│   │   ├── Service.js
│   │   ├── Booking.js
│   │   ├── Review.js
│   │   └── Warranty.js
│   ├── routes/
│   │   └── [all route files]
│   ├── server.js
│   └── package.json
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── layout/
│   │   │   │   ├── Navbar.jsx
│   │   │   │   └── Footer.jsx
│   │   │   ├── ProtectedRoute.jsx
│   │   │   └── AdminRoute.jsx
│   │   ├── context/
│   │   │   ├── AuthContext.jsx
│   │   │   └── CartContext.jsx
│   │   ├── pages/
│   │   │   ├── Home.jsx
│   │   │   ├── Products.jsx
│   │   │   ├── ProductDetail.jsx
│   │   │   ├── Cart.jsx
│   │   │   ├── Checkout.jsx
│   │   │   ├── Login.jsx
│   │   │   ├── Register.jsx
│   │   │   ├── Profile.jsx
│   │   │   ├── Orders.jsx
│   │   │   ├── OrderDetail.jsx
│   │   │   ├── Services.jsx
│   │   │   ├── Bookings.jsx
│   │   │   ├── Reviews.jsx
│   │   │   ├── Warranty.jsx
│   │   │   └── admin/
│   │   │       ├── Dashboard.jsx
│   │   │       ├── Products.jsx
│   │   │       ├── Orders.jsx
│   │   │       ├── Services.jsx
│   │   │       ├── Bookings.jsx
│   │   │       ├── Inventory.jsx
│   │   │       ├── Suppliers.jsx
│   │   │       ├── Reviews.jsx
│   │   │       └── Warranty.jsx
│   │   ├── services/
│   │   │   └── api.js
│   │   ├── App.jsx
│   │   ├── main.jsx
│   │   └── index.css
│   ├── index.html
│   ├── package.json
│   ├── vite.config.js
│   └── tailwind.config.js
│
└── README.md
```

## API Endpoints

### Authentication
- POST `/api/auth/register` - Register new user
- POST `/api/auth/login` - Login user
- GET `/api/auth/profile` - Get user profile
- PUT `/api/auth/profile` - Update profile

### Products
- GET `/api/products` - Get all products
- GET `/api/products/:id` - Get single product
- POST `/api/products` - Create product (Admin)
- PUT `/api/products/:id` - Update product (Admin)
- DELETE `/api/products/:id` - Delete product (Admin)

### Orders
- POST `/api/orders` - Create order
- GET `/api/orders/myorders` - Get user's orders
- GET `/api/orders/:id` - Get order details
- PUT `/api/orders/:id/status` - Update order status (Admin)
- PUT `/api/orders/:id/cancel` - Cancel order

### Services & Bookings
- GET `/api/services` - Get all services
- POST `/api/bookings` - Create booking
- GET `/api/bookings/mybookings` - Get user's bookings

### Reviews & Warranty
- POST `/api/reviews` - Submit review
- POST `/api/warranty` - Submit warranty claim

## Creating Admin User

To create an admin user, register a normal user first, then update the role in MongoDB:

```javascript
// In MongoDB shell or Compass
db.users.updateOne(
  { email: "admin@example.com" },
  { $set: { role: "admin" } }
)
```

## Technologies Used

### Backend
- Node.js & Express.js
- MongoDB & Mongoose
- JWT for authentication
- bcryptjs for password hashing

### Frontend
- React 18 with Vite
- React Router v6
- Tailwind CSS
- Axios for API calls
- React Hot Toast for notifications
- React Icons

## Discount Codes (for testing)
- `SAVE10` - 10% discount
- `SAVE20` - 20% discount

# Auto-Parts-pro
A complete web application for managing vehicle spare parts, inventory, customer records, and service appointments.

