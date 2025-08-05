# UserManagement API

A simple Node.js REST API for managing products using Express and MongoDB.

## Features

- Add, update, delete, and fetch products
- MongoDB integration via Mongoose
- Error handling middleware
- Environment variable support

## Project Structure

```
UserManagement/
  package.json
  server/
    .env
    constants.js
    index.js
    package.json
    controller/
      productController.js
    middleware/
      connectDb.js
      errorHandler.js
    model/
      productModel.js
    routes/
      productRoutes.js
```

## Setup

1. **Clone the repository**
2. **Install dependencies**
   ```sh
   cd UserManagement/server
   npm install
   ```
3. **Configure environment variables**

   Edit `server/.env` with your MongoDB connection string and desired port.

4. **Run the server**
   ```sh
   npm run dev
   ```
   or
   ```sh
   npm start
   ```

## API Endpoints

- `GET /api/stores/` — Get all products
- `POST /api/stores/` — Add a new product
- `GET /api/stores/:id` — Get a single product
- `PUT /api/stores/:id` — Update a product
- `DELETE /api/stores/:id` — Delete a product
