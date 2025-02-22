
# User Management API

This API allows you to manage users through the following operations: adding a new user, retrieving a list of users, retrieving a specific user by ID, and updating user information.

## Endpoints

### 1. **Add a User**

- **Endpoint**: `POST /users`
- **Description**: Adds a new user.
- **Request Body**:

  ```json
  {
    "name": "gela",
    "email": "gela@gmail.com",
    "password": "gel100"
  }
  ```

- **Response**: Returns the created user.

---

### 2. **Get All Users**

- **Endpoint**: `GET /users`
- **Description**: Retrieves a list of all users.
- **Response**: Returns an array of users.

---

### 3. **Get a Specific User**

- **Endpoint**: `GET /users/<id>`
- **Description**: Retrieves a user by ID.
- **Parameters**:
  - `id` (required): The unique identifier of the user.
- **Response**: Returns the user object.

---

### 4. **Update User Information**

- **Endpoint**: `PUT /users/<id>`
- **Description**: Updates the information of an existing user.
- **Request Body**:

  ```json
  {
    "name": "gela",
    "email": "gela@gmail.com",
    "password": "gel100"
  }
  ```
  
- **Parameters**:
  - `id` (required): The unique identifier of the user to update.
- **Response**: Returns the updated user object.
