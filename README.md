# Veggify Recipe App Server

This is the server-side application for the Veggify Recipe App. It uses Express.js for handling HTTP requests, Mongoose for MongoDB object modeling, and dotenv for environment variables.

## Getting Started

Follow these instructions to set up and run the server on your local machine for development and testing purposes.

### Prerequisites

- Node.js installed on your local machine. You can download it from [nodejs.org](https://nodejs.org/).
- MongoDB instance running. You can use [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) for a cloud-based MongoDB instance or run it locally.

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/recipe-app-server.git
   cd recipe-app-server
   ```

2. Install the dependencies:

   ```bash
   npm install
   ```

3. Create a `.env` file in the root directory and add your MongoDB URI and PORT:

   ```
   mongoURI=your_mongodb_uri
   PORT=your_port_number
   ```

   Replace `your_mongodb_uri` with your actual MongoDB connection string and `your_port_number` with the desired port number.

### Running the Server

Start the server by running:

```bash
npm start
```

The server will be running at `http://localhost:5000` (or the port you specified in the `.env` file).

### API Endpoints

- `GET /` - Check if the server is running.
- `POST /api/items` - Create a new item.
- `GET /api/items` - Get all items.
- `GET /api/items/:id` - Get a specific item by ID.
- `PUT /api/items/:id` - Update an item by ID.
- `DELETE /api/items/:id` - Delete an item by ID.
- `POST /api/categories` - Create a new category.
- `GET /api/categories` - Get all categories.
- `GET /api/categories/:id` - Get a specific category by ID.
- `PUT /api/categories/:id` - Update a category by ID.
- `DELETE /api/categories/:id` - Delete a category by ID.

### Built With

- [Express.js](https://expressjs.com/) - Web framework for Node.js.
- [Mongoose](https://mongoosejs.com/) - MongoDB object modeling tool.
- [dotenv](https://www.npmjs.com/package/dotenv) - Loads environment variables from a `.env` file.
- [cors](https://www.npmjs.com/package/cors) - Middleware for enabling CORS (Cross-Origin Resource Sharing).
