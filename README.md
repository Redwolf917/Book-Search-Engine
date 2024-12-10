# Book Search Engine

## Description

The **Book Search Engine** is a web application built with the **MERN stack** (MongoDB, Express.js, React, Node.js) and **GraphQL**. It allows users to search for books using the Google Books API, save books to their personal library, and manage saved books through an easy-to-use interface.

The app features user authentication (signup and login), persistent user data with JWT tokens, and integrates **MongoDB Atlas** for cloud storage. The frontend is built with React, and the backend uses GraphQL for querying and managing user data.

## Features

- **User Authentication**: Secure signup and login using JWT tokens.
- **Search for Books**: Use the Google Books API to search for books by title, author, or keyword.
- **Save Books**: Add books to your personal library, with detailed information such as title, authors, description, and image.
- **Manage Saved Books**: View, remove, and manage saved books in your account.
- **GraphQL API**: Replace REST API with GraphQL for querying and mutating user data.
- **MongoDB Atlas**: Store user data and saved books in MongoDB Atlas for cloud scalability.

## Technologies Used

- **Frontend**: React, Apollo Client, Bootstrap
- **Backend**: Node.js, Express.js, Apollo Server, GraphQL
- **Database**: MongoDB (MongoDB Atlas)
- **Authentication**: JWT (JSON Web Tokens)

## Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/book-search-engine.git
   ```

2. **Install dependencies**:
   - For the backend (Node.js):
     ```bash
     cd server
     npm install
     ```
   - For the frontend (React):
     ```bash
     cd client
     npm install
     ```

3. **Create a `.env` file**:
   In the root of the project, create a `.env` file and add the following:
   ```env
   MONGODB_URI='your_mongodb_connection_string_here'
   JWT_SECRET_KEY='your_jwt_secret_key_here'
   ```

4. **Start the application**:
   - To run the application locally, first start the backend:
     ```bash
     cd server
     npm run start
     ```
   - Then, start the frontend:
     ```bash
     cd client
     npm run start
     ```

   The app should now be running on `http://localhost:3000` (React frontend) and `http://localhost:3001/graphql` (GraphQL endpoint).

## Deployment

This project can be deployed to platforms like **Render** or **Heroku** with MongoDB Atlas for cloud hosting.

1. **Deploy Backend**: Set up the backend on Render or Heroku, linking the MongoDB Atlas cluster and setting the environment variables for `MONGODB_URI` and `JWT_SECRET_KEY`.
2. **Deploy Frontend**: Deploy the React app using **Netlify** or **Vercel**.

## User Stories

- **As an avid reader**, I want to search for new books to read so that I can keep a list of books to purchase.
- **As a logged-in user**, I want to save books to my account so that I can manage my reading list.
- **As a user**, I want to remove books from my saved library when I no longer wish to keep track of them.

## Contributing

Feel free to fork this project and submit pull requests. Contributions are always welcome!

## License

This project is licensed under the MIT License.
