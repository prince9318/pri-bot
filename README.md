# Chat AI Application

## Overview

This is a Chat AI application built with React on the frontend and Node.js/Express on the backend. It allows users to sign up, log in, and engage in conversations.

## Features

- **User Authentication:** Secure signup and login functionality.
- **Chat Interface:** A user-friendly interface for chatting.
- **Notification System:** In-app notifications to guide users.
- **Routing:** Implemented using React Router for seamless navigation.
- **Responsive Design:** The application is designed to be responsive and work on different screen sizes.

## Technologies Used

- **Frontend:**
  - React
  - React Router
  - JSX
  - CSS
- **Backend:**
  - Node.js
  - Express
- **Database:**
  - Mongoose
  - MongoDB

## Setup Instructions

1.  **Clone the repository:**

    ```bash
    git clone <repository-url>
    ```

2.  **Navigate to the project directory:**

    ```bash
    cd chat-ai
    ```

3.  **Install dependencies for the frontend:**

    ```bash
    cd chat-ai
    npm install
    ```

4.  **Install dependencies for the backend:**

    ```bash
    cd backend
    npm install
    ```

5.  **Configuration:**

    - Create a `.env` file in the `backend` directory.
    - Add the following environment variables:

      ```
      PORT=5555
      MONGODB_URI=<your_mongodb_connection_string>
      ```

6.  **Running the application:**

    - **Start the backend server:**

      ```bash
      cd backend
      npm run dev
      ```

    - **Start the frontend development server:**

      ```bash
      cd chat-ai
      npm start
      ```

    - The frontend will be accessible at `http://localhost:3000`.

## Important Notes

- The application is hosted on a free server (OnRender), so it may take a few seconds to initialize if the server hasn't been in use.
- A notification message is displayed to inform users about this potential delay.

## Project Structure

```
chat-ai
├── backend
│   ├── config
│   ├── controllers
│   ├── middleware
│   ├── models
│   ├── routes
│   ├── .env
│   ├── package.json
│   └── server.js
└── chat-ai
    ├── public
    ├── src
    │   ├── components
    │   ├── pages
    │   ├── App.js
    │   ├── index.js
    │   └── reportWebVitals.js
    ├── .env
    ├── package.json
    └── vite.config.js
```

## API Endpoints

| Method | Endpoint              | Description                      |
| ------ | --------------------- | -------------------------------- |
| POST   | /api/auth/signup      | Register a new user              |
| POST   | /api/auth/login       | Log in an existing user          |
| GET    | /api/users/me         | Get the current user's profile   |
| POST   | /api/messages/send    | Send a new message               |
| GET    | /api/messages/:chatId | Get messages for a specific chat |

## Future Enhancements

- **Search Functionality:** Allow users to search through chat history.
- **File Sharing:** Enable users to share files and images in chats.
- **Dark Mode:** Add a dark mode theme for better accessibility.
- **Performance Optimization:** Improve performance for larger datasets and more concurrent users.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Inspired by various open-source projects and tutorials.
- Special thanks to the contributors and the community for their support and feedback.
