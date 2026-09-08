<h1 align="center">
  <br>
  <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4fac2fa5c924d4cb8bb189af91ea/topics/javascript/javascript.png" alt="PawPop Logo" width="100">
  <br>
  🐾 PawPop: Pet Health Management App
  <br>
</h1>

<h4 align="center">A comprehensive application to track, manage, and optimize your pet's health and wellness journey and finances.</h4>

<p align="center">
  <img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/username/pawpop/build.yml?style=flat-square&label=Build">
  <img alt="Version" src="https://img.shields.io/github/v/release/username/pawpop?style=flat-square">
  <img alt="GitHub issues" src="https://img.shields.io/github/issues/username/pawpop?style=flat-square">
  <img alt="License" src="https://img.shields.io/github/license/username/pawpop?style=flat-square">
  <img alt="PRs Welcome" src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square">
</p>

<p align="center">
  <a href="#key-features">Key Features</a> •
  <a href="#architecture-and-tech-stack">Tech Stack</a> •
  <a href="#installation--setup">Installation</a> •
  <a href="#usage-guide">Usage</a> •
  <a href="#api-reference">API</a> •
  <a href="#roadmap">Roadmap</a> •
  <a href="#contributing">Contributing</a>
</p>

---

## 🐶 About The Project

**PawPop** is a full-stack web and mobile-responsive application designed for pet owners, veterinarians, and animal caretakers. It centralizes all aspects of pet care, ensuring that medical records, vaccination schedules, dietary plans, and daily activity logs are always just a click away.

Whether you have one dog or a whole sanctuary of mixed animals, PawPop adapts to your needs with customizable profiles and dynamic reminders.

## ✨ Key Features

*   **Multi-Pet Profiles:** Create and manage individual profiles for different pets, complete with breed, age, weight tracking, and profile pictures.
*   **Medical Dashboard & Records:** Store digital copies of vet bills, prescriptions, and diagnosis reports securely.
*   **Dynamic Reminders:** Automated push notifications and email alerts for:
    *   💉 Upcoming vaccinations
    *   💊 Daily medication schedules
    *   🛁 Grooming appointments
*   **Diet & Activity Tracking:** Log daily meals, monitor caloric intake, and track exercise routines to ensure your pet stays fit.
*   **Vet Connect Module:** Share temporary, read-only access links to your pet’s health history with your veterinarian.
*   **Growth Charts:** Visual analytics (using Chart.js/Recharts) showing weight and growth trends over time.

## 🛠 Architecture and Tech Stack

PawPal is built using modern, scalable technologies to ensure a smooth user experience and secure data handling.

*   **Frontend:** React.js / React Native, Redux Toolkit, Tailwind CSS
*   **Backend:** Node.js, Express.js
*   **Database:** MongoDB (with Mongoose ORM), Redis for caching
*   **Authentication:** JSON Web Tokens (JWT) & OAuth 2.0 (Google/Apple Sign-in)
*   **Storage:** AWS S3 (for storing medical documents and images)
*   **Notifications:** Firebase Cloud Messaging (FCM) & SendGrid

## 🚀 Installation & Setup

To run a local instance of PawPal for development and testing, follow these steps:

### Prerequisites
*   Node.js (v16.x or higher)
*   MongoDB (Local instance or MongoDB Atlas cluster)
*   Git

### Steps

1.  **Clone the repository**
    ```bash
    git clone https://github.com/username/pawpal.git
    cd pawpal
    ```

2.  **Install dependencies**
    Navigate to both the client and server directories to install packages.
    ```bash
    # Install server dependencies
    cd server
    npm install

    # Install client dependencies
    cd ../client
    npm install
    ```

3.  **Environment Configuration**
    Create a `.env` file in the `server` directory and add the following dynamic configuration variables:
    ```env
    PORT=5000
    MONGO_URI=your_mongodb_connection_string
    JWT_SECRET=your_super_secret_jwt_key
    AWS_ACCESS_KEY_ID=your_aws_access_key
    AWS_SECRET_ACCESS_KEY=your_aws_secret_key
    SENDGRID_API_KEY=your_sendgrid_key
    ```

4.  **Run the application**
    ```bash
    # Run backend (from /server)
    npm run dev

    # Run frontend (from /client)
    npm start
    ```
    The frontend will be available at `http://localhost:3000` and the backend at `http://localhost:5000`.

## 📱 Usage Guide

1.  **Sign Up/Log In:** Create an account using email or social login.
2.  **Onboarding:** Add your first pet by filling out their basic details (Name, Species, Breed, DOB).
3.  **Dashboard:** Navigate to the main dashboard to view the health summary.
4.  **Logging Health Data:** Use the "+" button to add a new medical record, weight log, or vaccination entry.
5.  **Setting Reminders:** Go to the "Reminders" tab to set up repeating alerts for tick medication or feeding times.

## 📡 API Reference

Below is a brief overview of the RESTful API endpoints available. Detailed documentation is available via [Swagger UI](#) (running at `/api-docs` in development).

| Endpoint | Method | Description | Auth Required |
| :--- | :---: | :--- | :---: |
| `/api/auth/register` | `POST` | Register a new user | ❌ |
| `/api/pets` | `GET` | Get all pets for logged-in user | ✅ |
| `/api/pets/:id` | `GET` | Get detailed pet profile | ✅ |
| `/api/pets/:id/health`| `POST` | Add a new health record | ✅ |
| `/api/reminders` | `GET` | Get active reminders | ✅ |

## 🗺 Roadmap

- [x] Basic user authentication and pet profiles
- [x] Medical record uploading and cloud storage
- [x] Email reminders for vaccinations
- [ ] **Upcoming:** integration with smart pet collars (FitBark, Whistle)
- [ ] **Upcoming:** AI-powered symptom checker assistant
- [ ] **Upcoming:** Community forum for pet owners

## 🤝 Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

## 📬 Contact

**Project Maintainer:** TWISHA SHRIYAM  - hello@pawpalapp.com

**Project Link:** THIS REPO 

---
<p align="center">Made with ❤️ for pets everywhere.</p>
