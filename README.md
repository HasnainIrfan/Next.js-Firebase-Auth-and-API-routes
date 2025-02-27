Next.js Authentication System with Firebase Auth

📌 Project Goal

The goal of this project is to create a simple authentication system with protected API endpoints using Next.js, Firebase Authentication, and API routes.

🚀 Features

1️⃣ Authentication

Implement Firebase Authentication with the following methods:

Email/Password login

Google OAuth login

Add a logout function to securely sign users out.

2️⃣ API Implementation

Create a protected API endpoint that:

Returns "not authorized" for non-authenticated users.

Returns the userId and auth token for authenticated users.

🛠️ Tech Stack

Next.js (latest version) - Server-side rendering and API routes

Firebase Authentication - Secure authentication

Tailwind CSS - Simple and efficient styling

📦 Installation & Setup

1️⃣ Clone the Repository

git clone https://github.com/yourusername/your-repository.git
cd your-repository

2️⃣ Install Dependencies

npm install
# or
yarn install

3️⃣ Configure Firebase

Create a Firebase project at Firebase Console.

Enable Email/Password Authentication and Google OAuth in Firebase Authentication settings.

Get your Firebase config from Project Settings > General > Your Apps.

Create a .env.local file and add your Firebase credentials:

NEXT_PUBLIC_FIREBASE_API_KEY=your_api_key
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=your_auth_domain
NEXT_PUBLIC_FIREBASE_PROJECT_ID=your_project_id
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=your_storage_bucket
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=your_messaging_sender_id
NEXT_PUBLIC_FIREBASE_APP_ID=your_app_id

4️⃣ Run the Development Server

npm run dev
# or
yarn dev

Visit http://localhost:3000 to view the project.

🔐 Protected API Endpoint

The API endpoint can be accessed at:

/api/protected

Response Behavior:

If the user is not authenticated:

{ "error": "not authorized" }

If the user is authenticated:

{
  "userId": "user-id",
  "authToken": "auth-token"
}

🛠 Future Enhancements

Add role-based authentication

Implement a user dashboard

Enhance UI/UX with more styling and animations

🎯 Contributing

Feel free to fork this repository and submit pull requests! 🚀

📜 License

This project is licensed under the MIT License.

📩 Questions or Suggestions?

Open an issue or reach out via GitHub!

Happy coding! 🎉
