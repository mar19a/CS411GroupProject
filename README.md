# Seekers Real Estate Application

![IMG_5177](https://github.com/mar19a/Seekers/assets/84360137/9c586d32-4ddf-4e20-b287-47fe25cc703f)

Seekers is a comprehensive real estate application designed to help users find homes and explore local businesses. Our platform offers seamless property search, agent information, and local business recommendations, providing a holistic approach to finding the perfect home.

Website made by Mariano Majano Amaya and Gary Dong.

You can find the demo here: https://youtu.be/PlX1SiR-Ezk

## Features

- **Property Search**: Users can search for properties based on city, address, or ZIP code.

![IMG_5178](https://github.com/mar19a/Seekers/assets/84360137/7b08a487-a899-4bba-ad5a-d195895393fa)

- **Interactive Map**: Google Maps integration to display property locations and details.

![IMG_5179](https://github.com/mar19a/Seekers/assets/84360137/5f470506-bac3-42cd-8556-18a8727677fa)

- **Local Business Search**: Users can explore local businesses in the area, enhancing their home search experience.

![IMG_5199](https://github.com/mar19a/Seekers/assets/84360137/d2453613-89a7-4c2f-92c0-7c26588a1609) ![IMG_5200](https://github.com/mar19a/Seekers/assets/84360137/489a6d74-6272-4b19-a899-43fd25280971)

- **News Feed**: Latest news based on your desired location.

![IMG_5180](https://github.com/mar19a/Seekers/assets/84360137/452bdfa3-11bb-445a-9388-454e165526e9)

- -**Market Insights**: Latest trends and data to the real estate market.

![IMG_5181](https://github.com/mar19a/Seekers/assets/84360137/d8d81ab5-5aef-4054-9517-89e429c942b3)

- **Agent Profiles**: Detailed information about real estate agents, including their specialties, experience, and contact information.

![IMG_5182](https://github.com/mar19a/Seekers/assets/84360137/08b9ced6-c56b-417f-962c-3e53beeafe25)

- **Contact Form**: Users can easily reach out for support or inquiries using FormSpree.

![IMG_5191](https://github.com/mar19a/Seekers/assets/84360137/594b61ff-80ea-4232-b049-db62d0e3e73b)![IMG_5192](https://github.com/mar19a/Seekers/assets/84360137/8736d115-6256-4490-9e6a-a354ed5e5102) ![IMG_5193](https://github.com/mar19a/Seekers/assets/84360137/e88a18d3-c8e3-4817-81c2-e4be6a06f1e1)

- **User Authentication**: Secure signup and login functionality using MySQL or Google OAuth.

![IMG_5195](https://github.com/mar19a/Seekers/assets/84360137/82353d95-2abb-4cd2-afcb-2b4a68ae9997) ![IMG_5196](https://github.com/mar19a/Seekers/assets/84360137/d5bede68-85b0-4a16-a882-93d1d2729097) ![IMG_5201](https://github.com/mar19a/Seekers/assets/84360137/004f9502-9d36-4b4a-866d-6060c6d142a0)

## Technologies Used

- **Frontend**: React, React Router, Google Maps API, Axios
- **Backend**: Node.js, Express.js
- **Database**: MySQL
- **Styling**: CSS, TailwindCSS
- **Authentication**: Google OAuth, Formspree
- **APIs** Zillow API, Local Business Data from RapidAPI, and News API.
- **Others**: gapi-script, React Icons

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/mar19a/seekers.git
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
