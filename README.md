# Node.js Express API with MongoDB

This is a Node.js backend server using Express and MongoDB. It includes functionalities such as user authentication, course management, and watchlist management with JWT authentication.

## Features
- User authentication (Signup, Login, Change Password, Update Profile)
- Course Management (Add, Delete, Add Lecture, Remove Lecture)
- Watchlist Management (Add Course to Watchlist, Remove Course from Watchlist)
- Secure routes with JWT Authentication

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/courseHubServer
   cd your-repo
   ```

2. Install dependencies:
   ```sh
   npm install
   ```

3. Create a `.env` file and add the following variables:
   ```env
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   ```

4. Start the server in development mode:
   ```sh
   npm run dev
   ```

5. Start the server in production mode:
   ```sh
   npm start
   ```

## API Endpoints

### Authentication
| Method | Endpoint             | Description          |
|--------|----------------------|----------------------|
| POST   | `/api/v1/register` | Register new user   |
| POST   | `/api/v1/login`    | Login user & get JWT|
| PUT    | `/api/v1/password` | Update password     |

### User Management
| Method | Endpoint             | Description                |
|--------|----------------------|----------------------------|
| GET    | `/api/v1/users/:id`     | Get user details          |
| PUT    | `/api/v1/users/:id`     | Update user profile       |
| DELETE | `/api/v1/users/:id`     | Delete user account       |

### Course Management
| Method | Endpoint                   | Description             |
|--------|----------------------------|-------------------------|
| POST   | `/api/v1/courses`              | Add a new course       |
| DELETE | `/api/v1/courses/:id`          | Delete a course        |
| POST   | `/api/v1/courses/:id/lecture`  | Add a lecture          |
| DELETE | `/api/v1/courses/:id/lecture`  | Remove a lecture       |

### Watchlist Management
| Method | Endpoint                   | Description                     |
|--------|----------------------------|---------------------------------|
| POST   | `/api/watchlist`           | Add course to watchlist         |
| DELETE | `/api/watchlist/:id`       | Remove course from watchlist    |

## Project Structure
```
project-folder/
│── server.js
│── package.json
│── .env
│── routes/
│── controllers/
│── models/
│── middleware/
│── config/
```

## Scripts
| Command         | Description                  |
|----------------|------------------------------|
| `npm run dev`  | Run server with nodemon     |
| `npm start`    | Run server normally         |
| `npm run build`| No build required message   |

## Dependencies
- **Express.js** - Web framework
- **MongoDB & Mongoose** - Database
- **jsonwebtoken** - JWT authentication
- **bcryptjs** - Password hashing
- **nodemon** - Auto-restart in development mode

## License
This project is licensed under the MIT License.


## For login PlZ use email:rinku@gmail.com , password:123456
