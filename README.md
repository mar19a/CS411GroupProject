# Seekers Real Estate Application

Seekers is a comprehensive real estate application designed to help users find homes and explore local businesses. Our platform offers seamless property search, agent information, and local business recommendations, providing a holistic approach to finding the perfect home.

Website made by Mariano Majano Amaya and Gary Dong.

You can find the demo here: https://youtu.be/PlX1SiR-Ezk

## Features

- **User Authentication**: Secure signup and login functionality using MySQL.
- **Agent Profiles**: Detailed information about real estate agents, including their specialties, experience, and contact information.
- **Property Search**: Users can search for properties based on city, address, or ZIP code.
- **Local Business Search**: Users can explore local businesses in the area, enhancing their home search experience.
- **Interactive Map**: Google Maps integration to display property locations and details.
- **News Feed**: Latest news updates relevant to the real estate market.
- **Contact Form**: Users can easily reach out for support or inquiries.

## Technologies Used

- **Frontend**: React, React Router, Google Maps API, Axios
- **Backend**: Node.js, Express.js
- **Database**: MySQL
- **Styling**: CSS, TailwindCSS
- **Authentication**: Google OAuth, Formspree
- **Others**: gapi-script, React Icons

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/seekers.git
    ```
2. Navigate to the project directory:
    ```bash
    cd seekers
    ```
3. Install the dependencies for the frontend:
    ```bash
    npm install
    ```
4. Navigate to the server directory and install backend dependencies:
    ```bash
    cd server
    npm install
    ```
5. Set up your MySQL database and update the connection details in `server.js`:
    ```javascript
    const con = mysql.createConnection({
        user: "root",
        host: "localhost",
        password: "",
        database: "register"
    })
    ```
6. Start the backend server:
    ```bash
    node server.js
    ```
7. Start the frontend development server:
    ```bash
    npm start
    ```

## Usage

### User Signup and Login

The backend provides endpoints for user registration and login:

- **Signup**: `POST /signup`
    - Request body: `{ "email": "user@example.com", "username": "user", "password": "password" }`
    - Response: Success or error message
- **Login**: `POST /login`
    - Request body: `{ "username": "user", "password": "password" }`
    - Response: User details or error message

### Property Search

Users can search for properties by entering a city, address, or ZIP code in the search bar. The search results are displayed with detailed property information and locations marked on an interactive map.

### Agent Profiles

Detailed profiles of real estate agents are displayed, including their contact information, specialties, and a brief bio.

### Local Business Search

Users can explore local businesses by entering a city in the search bar. The results include business names, addresses, phone numbers, and websites.

### News Feed

The latest news articles relevant to the real estate market are displayed, providing users with current information and trends.

### Contact Form

Users can fill out a contact form to get in touch with the Seekers team for any inquiries or support.

## Contributing

We welcome contributions from the community. To contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a new Pull Request.

## License

This project is licensed under the MIT License.

## Acknowledgements

- Our team for their hard work and dedication.
- The open-source community for providing valuable tools and resources.
