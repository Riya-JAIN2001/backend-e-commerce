### Backend README Summary

# E-commerce Backend

This backend supports an E-commerce application using the MERN stack (MongoDB, Express.js, React.js, Node.js). It handles user authentication, product management, shopping cart, and order processing.

## Technology Stack
- MongoDB: NoSQL database
- Express.js: Web framework
- Node.js: Server runtime
- JWT: Stateless authentication
- Bcrypt: Password hashing

## Setup and Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/ecommerce-backend.git
   cd ecommerce-backend
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Create a `.env` file:**
   ```
   MONGODB_URL=mongodb://localhost:27017/your_db_name
   JWT_SECRET=your_jwt_secret
   ```

4. **Start the MongoDB server:**
   ```bash
   mongod
   ```

5. **Start the Node.js server:**
   ```bash
   npm start
   ```

## API Endpoints

- **Auth Routes:**
  - `POST /api/auth/register`: Register user
  - `POST /api/auth/login`: Login user

- **Product Routes:**
  - `GET /api/products`: Get all products
  - `POST /api/products`: Add product (admin)
  - `PUT /api/products/:id`: Update product (admin)
  - `DELETE /api/products/:id`: Delete product (admin)

- **Cart Routes:**
  - `GET /api/cart`: Get user's cart
  - `POST /api/cart`: Add product to cart
  - `PUT /api/cart/:id`: Update cart item
  - `DELETE /api/cart/:id`: Remove product from cart

- **Order Routes:**
  - `POST /api/orders`: Create order
  - `GET /api/orders`: Get all orders (admin)
  - `GET /api/orders/:id`: Get specific order

## Environment Variables

Create a `.env` file:
```
MONGODB_URL=mongodb://localhost:27017/your_db_name
JWT_SECRET=your_jwt_secret
```

## Start the Server

```bash
npm start
```
