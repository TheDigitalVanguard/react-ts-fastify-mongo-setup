# 🚀 Full-Stack Boilerplate: React TypeScript + Fastify MongoDB

This boilerplate provides a modern and efficient full-stack setup for web applications, combining a **React TypeScript** frontend with a **Fastify MongoDB** backend. It is designed for scalability, maintainability, and developer productivity, featuring best practices for coding standards, testing, and internationalization.

## 🌟 Key Features

### 🖥️ Frontend (React + TypeScript + Chakra UI)

- **React with TypeScript** – Ensures type safety and better developer experience.
- **Chakra UI** – A flexible and accessible component library for styling.
- **i18n Support** – Internationalization is pre-configured with translation files.
- **ESLint & Prettier** – Enforces consistent code quality and formatting.
- **Jest & React Testing Library** – Unit and integration testing setup for reliability.

### ⚡ Backend (Fastify + MongoDB)

- **Fastify** – A lightweight and high-performance Node.js framework.
- **MongoDB** – NoSQL database integration with Mongoose for schema management.
- **ESLint** – Code linting for better maintainability.
- **Jest** – Pre-configured for backend unit and integration testing.

## 📌 Additional Features

- **End-to-End Type Safety** – TypeScript used across both frontend and backend.
- **Pre-configured API Routes** – Fastify server setup with structured endpoints.
- **Environment Variable Support** – Easily configurable settings for different environments.
- **Scalable Architecture** – Modular and organized folder structure for long-term growth.

This boilerplate is perfect for developers looking to jumpstart a project with a solid foundation, reducing setup time while following industry best practices. 🚀

# Application Setup Guide

### Using Node v23.7.0 & NPM v10.9.2

## 1. Set Up Your Database (MongoDB)

- Create a **MongoDB account** and log in.
- Navigate to your **database management section** and create a new database named:  
  **`users`**
- Inside the `users` database, create a new **collection** named:  
  **`articles`**
- Add the following JSON object as an entry in the `articles` collection:

  ```json
  {
    "_id": "ba0880b2-49c0-4abd-9aa5-3f3a784a4fd0",
    "user_id": "2cc2d264-020a-4690-be0f-2ad84a729942",
    "articles": [
      {
        "id": "1b8f723c-a2cf-46e2-bf38-b1d874103950",
        "article_name": "How The Digital Vanguard was built",
        "url": "https://www.youtube.com/watch?v=_T9s2K4UWaA",
        "article_details": ["md_file_1", "md_file_2"]
      }
    ]
  }
  ```

## 2. Configure Environment Variables

- Locate the `.env.sample` files inside both the **client** and **server** directories.
- Use these as a reference to create `.env` files in their respective locations.
- Ensure all required variables (like database connection strings, API keys, etc.) are set properly.
- **_Note the 'USER_ID' in the server .env is the user_id for that single json object in the mongodb articles collection_**

## 3. Install Dependencies

- Open a terminal and navigate to the **client** directory:
  ```sh
  cd client
  npm install
  cd ..
  ```
- Then, navigate to the **server** directory and install dependencies there as well::
  ```sh
  cd client
  npm install
  cd ..
  ```
- Then, navigate back to the root directory
  ```sh
  cd ..
  ```

## 4. Start the Application

- Ensure you are in the **root directory**, then run:
  ```sh
  npm run start
  ```

## Your application should now be running! 🚀
