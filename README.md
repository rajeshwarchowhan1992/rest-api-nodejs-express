# REST API - Node.js & Express

A robust RESTful API built with Node.js and Express.js featuring JWT authentication, CRUD operations, and MongoDB integration.

## Features

- **User Authentication**: JWT-based authentication and authorization
- **CRUD Operations**: Complete Create, Read, Update, Delete functionality
- **Database Integration**: MongoDB with Mongoose ODM
- **Input Validation**: Request validation using express-validator
- **Error Handling**: Centralized error handling middleware
- **API Documentation**: Swagger/OpenAPI documentation
- **Security**: Helmet.js for security headers, CORS configuration
- **Rate Limiting**: Protection against brute-force attacks

## Technologies Used

- **Node.js** - JavaScript runtime
- **Express.js** - Web framework
- **MongoDB** - NoSQL database
- **Mongoose** - MongoDB object modeling
- **JWT** - JSON Web Tokens for authentication
- **bcrypt** - Password hashing
- **dotenv** - Environment variable management

## Project Structure

```
rest-api/
├── src/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   └── utils/
├── config/
├── tests/
├── .env.example
├── package.json
└── server.js
```

## API Endpoints

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - Login user
- `POST /api/auth/refresh` - Refresh access token

### Users
- `GET /api/users` - Get all users (Admin only)
- `GET /api/users/:id` - Get user by ID
- `PUT /api/users/:id` - Update user
- `DELETE /api/users/:id` - Delete user

## Getting Started

1. Clone the repository
2. Install dependencies: `npm install`
3. Create `.env` file with your configuration
4. Run development server: `npm run dev`
5. Run tests: `npm test`

## Environment Variables

```
PORT=3000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
JWT_EXPIRE=7d
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

MIT License
