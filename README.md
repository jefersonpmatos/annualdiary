# Annual Diary

A simple way to track your mood throughout the year.

Annual Diary is a personal diary focused on visualizing how your mood changes over time. Instead of writing long journal entries, you record how you felt each day and build a visual representation of your year.

The project was built as a fullstack application to explore authentication, data persistence, server-side rendering and the relationship between a simple UI and a relational data model.

## ✨ Features

- 📅 Daily mood tracking
- 🎨 Visual representation of your year
- 🔐 User authentication
- 💾 Persistent data storage
- 📱 Responsive interface
- ⚡ Server-side rendering
- 🗄️ Relational database with Prisma

## 🛠️ Tech Stack

### Frontend

- Next.js
- React
- TypeScript
- Tailwind CSS
- shadcn/ui

### Backend & Data

- Next.js
- Prisma
- PostgreSQL

### Tooling

- ESLint
- Yarn
- Vercel

## 🧠 Why I Built It

Annual Diary started from a simple idea: what if you could look at an entire year and instantly understand how you felt throughout it?

The project was also an opportunity to work on a complete application instead of focusing exclusively on the frontend.

Some of the things explored during development:

- Designing the database around users and daily records
- Handling authentication and protected data
- Keeping the UI simple while making the data meaningful
- Structuring a Next.js application around server and client responsibilities
- Persisting and retrieving user-specific data
- Building a responsive interface without unnecessary complexity

## 🏗️ Architecture

The application is built with Next.js and follows a fullstack approach, keeping the frontend, server logic and database integration within the same project.

```text
┌─────────────────────┐
│       Next.js       │
│                     │
│  UI + Server Logic  │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│       Prisma        │
│                     │
│   Database Access   │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│     PostgreSQL      │
│                     │
│ Users / Diary Data  │
└─────────────────────┘
```

## 🚀 Getting Started

### Prerequisites

- Node.js
- PostgreSQL database
- Yarn

### Installation

Clone the repository:

```bash
git clone https://github.com/jefersonpmatos/annualdiary.git
cd annualdiary
```

Install dependencies:

```bash
yarn install
```

Create your environment file:

```bash
cp .env.example .env
```

Configure your database connection in `.env`:

```env
DATABASE_URL="postgresql://user:password@localhost:5432/annualdiary"
```

Run the Prisma migrations:

```bash
yarn prisma migrate dev
```

Start the development server:

```bash
yarn dev
```

The application will be available at:

```text
http://localhost:3000
```

## 📸 Preview

You can try the live application here:
https://annualdiary.vercel.app

## 📁 Project Structure

```text
annualdiary/
├── app/            # Application routes and pages
├── components/     # Reusable UI components
├── hooks/          # Custom React hooks
├── lib/            # Utilities and shared logic
├── prisma/         # Database schema and migrations
├── images/         # Project assets
└── public/         # Static assets
```

## 📌 Project Status

This is a personal project created to explore fullstack application architecture and experiment with different technical decisions in a controlled environment.

## 📄 License

This project is available under the MIT License.
