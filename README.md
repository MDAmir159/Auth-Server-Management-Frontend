# Auth Server Frontend

Coding assessment for Nerdevs recruitment process.

See the backend repository [here](https://github.com/MDAmir159/Auth-Server-Backend).
## Features

- User authentication (login, signup)
- Account activation via email
- Conditional rendering based on user authentication
- Local storage management for user sessions
- Logout functionality

## Demo

Check out the demo of the project on YouTube:  
[Watch the Demo on YouTube](https://www.youtube.com/watch?v=9CyvyizvU6k)

## Installation

Follow these steps to get the project running locally.

### Prerequisites

Ensure you have the following installed:
- [Node.js](https://nodejs.org/en/) (v20 or higher)
- [npm](https://www.npmjs.com/)

### Clone the Repository

```bash
git clone https://github.com/MDAmir159/Auth-Server-Frontend.git
cd Auth-Server-Management-Task2
```

### Install Dependencies

```
npm install
```

### Run the aplicaiton

```
npm run dev
```

The application will be running on `http://localhost:5173`.

### Local Storage
The project uses local storage to keep track of user authentication. The key-value pair saved is:
```
{
  "nerd-dev": {
    "isAuthenticated": true
  }
}

```

### Project Structure
A brief overview of the project structure (mentioned only the necessary ones):
```
.
├── public
├── src
│   ├── assets
│   ├── components
│   ├── router
│   │   ├── index.ts
│   ├── views
│   │   ├── HomeView.vue
│   │   ├── LoginView.vue
│   │   ├── SignupView.vue
│   │   ├── AboutView.vue
│   │   └── ActivateView.vue
│   ├── App.vue
│   └── main.ts
├── package.json
├── tsconfig.json
└── README.md

```
## Technologies Used

- **Vue.js** (with TypeScript)
- **Vue Router** for routing
- **Ant Design Vue** for UI components
- **Local Storage** for user session management
- **Node.js** (backend, if applicable)

## API Endpoints

- `POST /auth/login`: For user login
- `POST /auth/signup`: For user signup
- `GET /auth/activate/:token`: For account activation
