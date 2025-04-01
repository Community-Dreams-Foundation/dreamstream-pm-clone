# Jira Clone - Fullstack Application

This project is a fullstack application inspired by Jira, built with modern web technologies.

## Tech Stack

- **Frontend:**
  - [Next.js](https://nextjs.org/)
  - [React](https://reactjs.org/)
  - [Tailwind CSS](https://tailwindcss.com/)
  - [Shadcn UI](https://ui.shadcn.com/)
- **Backend:**
  - [Prisma](https://www.prisma.io/)
  - [Neon (PostgreSQL Serverless)](https://neon.tech/)
- **Authentication:**
  - [Clerk](https://clerk.com/)

## Getting Started

1. **Clone the repository:**

    ```bash
    git clone <repository_url>
    cd <repository_name>
    ```

2. **Install dependencies:**

    ```bash
    npm install
    # or
    yarn install
    # or
    pnpm install
    ```

3. **Set up environment variables:**

    Create a `.env.local` file in the root directory and add the following variables:

    ```plaintext
    DATABASE_URL=your_neon_database_url
    NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
    CLERK_SECRET_KEY=your_clerk_secret_key
    NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
    NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
    NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/onboarding
    NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/onboarding
    ```

    **Note:** Replace `your_neon_database_url`, `your_clerk_publishable_key`, and `your_clerk_secret_key` with your actual values.

4. **Run Prisma migrations:**

    ```bash
    npx prisma migrate dev
    ```

5. **Start the development server:**

    ```bash
    npm run dev
    # or
    yarn dev
    # or
    pnpm dev
    ```

    Open your browser and navigate to `http://localhost:3000`.

## Environment Variables

- `DATABASE_URL`: The connection string for your Neon PostgreSQL database.
- `NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY`: Your Clerk publishable key.
- `CLERK_SECRET_KEY`: Your Clerk secret key.
- `NEXT_PUBLIC_CLERK_SIGN_IN_URL`: The URL for the sign-in page.
- `NEXT_PUBLIC_CLERK_SIGN_UP_URL`: The URL for the sign-up page.
- `NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL`: The URL to redirect to after successful sign-in.
- `NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL`: The URL to redirect to after successful sign-up.

## Contributing

Contributions are welcome! Please feel free to submit a pull request.
