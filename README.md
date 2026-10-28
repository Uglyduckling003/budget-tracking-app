# Next.js Budget Tracker

Welcome to the Next.js Budget Tracker application. Follow the guide below to set up your local development environment.

## 🚀 Prerequisites

Before you begin, ensure you have the following installed:
* **Node.js**: `v20.x` (LTS recommended)
* **Package Manager**: `npm` (v10.x or higher)

## 🛠️ Local Setup

### 1. Clone the Repository
```bash
git clone <your-repository-url>
cd nextjs-budget-tracker
```

### 2. Install Dependencies
Install the required project dependencies using the package manager:
```bash
npm install
```

### 3. Environment Configuration
The application requires environment variables to connect to external services (e.g., database, authentication).

1. Copy the example environment file to create a local environment file:
   ```bash
   cp .env.example .env.local
   ```
2. Open `.env.local` and populate the variables with your local or development credentials. **Do not commit your `.env.local` file to version control.**

Example of required variables:
* `DATABASE_URL`: Connection string for your local or cloud database (e.g., `postgresql://user:password@localhost:5432/budget_db`)
* `NEXTAUTH_SECRET`: A random string used to hash tokens for authentication.

---

## 💻 Development Commands

### Start the Development Server
Run the following command to start the application locally:
```bash
npm run dev
```
Open [http://localhost:3000](http://localhost:3000) in your browser to view the application.

### Code Linting
To check the codebase for syntax and formatting errors, run:
```bash
npm run lint
```

### Production Build
To verify that the application compiles correctly for a production deployment, run:
```bash
npm run build
```