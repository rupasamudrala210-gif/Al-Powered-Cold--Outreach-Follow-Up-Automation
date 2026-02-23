🚀 Installation & Configuration Guide

This guide explains how to install, configure, and run the project locally.

🛠️ Prerequisites

Make sure you have the following installed:

Node.js (v18 or higher)

npm (comes with Node.js)

Git

Check versions:

node -v
npm -v
git --version
📦 Installation Steps
1. Clone the Repository
git clone https://github.com/your-username/your-repository-name.git
cd your-repository-name
2. Install Dependencies
npm install
🔑 Environment Variables Setup

Create a .env file in the root folder:

touch .env

Add the following:

PORT=3000
NODE_ENV=development

DATABASE_URL=your_database_url

JWT_SECRET=your_secret_key

OPENAI_API_KEY=your_api_key

⚠️ Important:

Do NOT commit your .env file.

Make sure .env is added to .gitignore.

🗄️ Database Setup (If Required)

Example for PostgreSQL:

createdb your_database_name

Update .env:

DATABASE_URL=postgres://username:password@localhost:5432/your_database_name

Run migrations (if available):

npm run migrate
▶️ Running the Application
Development Mode
npm run dev
Production Mode
npm start

App will run on:

http://localhost:3000
🧪 Run Tests
npm test
🔐 API Keys Setup

Create required API keys (OpenAI, Google, AWS, etc.).

Add them inside the .env file.

Restart the server after adding keys.

✅ Setup Checklist

 Node.js installed

 Project cloned

 Dependencies installed

 .env file created

 Database configured

 App running successfully
