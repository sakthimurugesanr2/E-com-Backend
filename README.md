# 🧠 E-Commerce Backend API

A scalable, secure, and production-ready backend API built for a full-stack e-commerce platform using **Node.js, Express, and MongoDB**.  
This backend follows **industry-standard architecture**, **clean code practices**, and **performance optimization** principles.

---

## 🚀 Features

### 🔐 Authentication & Authorization
- JWT-based authentication
- Secure password hashing using bcrypt
- Role-based access control (Admin / User)
- Protected routes with middleware
- Token validation on every request

### 🛍️ Product Management
- Create / Update / Delete products (Admin only)
- Fetch products with:
  - Search
  - Filter
  - Sort
  - Pagination
- Product details view
- Related products
- Optimized MongoDB queries

### 🛒 Cart & Orders
- Add to cart
- Update item quantity
- Remove items from cart
- Create orders
- Order history per user
- Order status management

### 💳 Payment Gateway
- Secure payment initiation
- Payment verification
- Failed and cancelled payment handling
- Order status update after payment
- Edge case handling

---

## 🛠️ Tech Stack

- Node.js
- Express.js
- MongoDB(atlas) | supabase
- Mongoose
- JWT
- bcrypt
- dotenv
- ESLint

---

## 📁 Folder Structure

```bash
backend/
│
├── controllers/
│   ├── auth.controller.js
│   ├── product.controller.js
│   ├── order.controller.js
│
├── routes/
│   ├── auth.routes.js
│   ├── product.routes.js
│   ├── order.routes.js
│
├── models/
│   ├── User.model.js
│   ├── Product.model.js
│   ├── Order.model.js
│
├── middleware/
│   ├── auth.middleware.js
│   ├── error.middleware.js
│
├── utils/
│   ├── asyncHandler.js
│   ├── apiError.js
│
├── config/
│   ├── db.js
│
├── app.js
├── server.js
└── README.md
```

##.env

```

PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
JWT_EXPIRE=7d
PAYMENT_SECRET_KEY=your_payment_key
NODE_ENV=development
```

## install
```
npm install
npm run back
```

## git 
```
git clone <repo-url>
git checkout dev
git pull origin dev

git checkout -b feature/backend-feature
git commit -m "feat: added secure authentication"
git push origin feature/backend-feature
```
