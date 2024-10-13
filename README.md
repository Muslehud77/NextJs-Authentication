

# NextJs-Authentication

This project demonstrates the basics of authentication in a Next.js application using **NextAuth.js**. The app includes Google, GitHub, and custom credentials authentication providers, and it covers protecting routes using middleware in Next.js.

## Features

- **NextAuth.js** for easy authentication management
- Google provider for Google sign-in
- GitHub provider for GitHub sign-in
- Custom credentials provider for manual authentication
- Protected routes using middleware in Next.js

## Technologies Used

- [Next.js](https://nextjs.org/) – The React Framework for Production
- [NextAuth.js](https://next-auth.js.org/) – Authentication for Next.js
- [React](https://reactjs.org/) – JavaScript library for building user interfaces
- [Node.js](https://nodejs.org/) – JavaScript runtime for backend services

## Getting Started

### Prerequisites

- Node.js installed on your local machine.
- A Google Developer account for setting up the Google OAuth provider.
- A GitHub account for setting up the GitHub OAuth provider.

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/NextJs-Authentication.git
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file in the root directory and add the following environment variables:

   ```bash

        GITHUB_SECRET=Github_secret
        GITHUB_ID=Github_id

        GOOGLE_SECRET=Google_secret
        GOOGLE_ID=Google_id

        BACKEND_URL=http://localhost:5001/api/v1

        NEXTAUTH_SECRET=your-secret-key
        NEXTAUTH_URL=http://localhost:3000

   
   ```

4. Run the development server:
   ```bash
   npm run dev
   ```

5. Open your browser and navigate to `http://localhost:3000`.

### Authentication Providers

This project supports the following authentication providers:

1. **Google Provider** – You can sign in using your Google account.
2. **GitHub Provider** – You can sign in using your GitHub account.
3. **Credentials Provider** – Allows users to sign in with a custom email and password.

### Protecting Routes with Middleware

Certain routes in this application are protected and can only be accessed by authenticated users. Next.js middleware is used to handle this protection, ensuring a smooth user experience across both the server and client.

### Learning Notes

- Learned to implement and configure multiple providers (Google, GitHub, credentials) with NextAuth.js.
- Explored session management and redirection using Next.js's built-in `getSession()` and `useSession()` hooks.
- Middleware integration to protect routes by checking for user authentication.

## License

This project is licensed under the MIT License.
```

You can customize this as needed based on additional features or details you add to your project!