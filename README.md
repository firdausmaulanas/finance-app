# Finance Tracker - Personal Finance Management Application

A complete financial tracking application built with Next.js, TypeScript, PostgreSQL, and Prisma.

## Features

- **Authentication**: Register, login, password hashing
- **Transactions**: Create, read, update, delete with filtering and search
- **Categories**: Default categories on signup + user management
- **Dashboard**: Analytics with charts, statistics, and recent transactions
- **Security**: Rate limiting, validation, security headers

## Tech Stack

- **Framework**: Next.js 14 (App Router)
- **Language**: TypeScript
- **Styling**: Tailwind CSS + shadcn/ui
- **Database**: PostgreSQL + Prisma ORM
- **Auth**: NextAuth.js v5
- **Validation**: Zod
- **Charts**: Recharts
- **Notifications**: Sonner
- **Date Utils**: date-fns (Indonesia locale)

## Setup

```bash
# Clone project
cd finance-app

# Install dependencies
npm install

# Setup environment variables
cp .env.example .env
# Edit .env with your database credentials

# Generate Prisma client
npm run prisma:generate

# Push schema to database
npm run prisma:push

# Seed database
npm run prisma:seed

# Run development
npm run dev
```

## Deployment

### Requirements

- Node.js 18+
- PostgreSQL 14+
- Redis (optional, for rate limiting)

### Environment Variables

```env
# Database
DATABASE_URL=postgresql://username:password@localhost:5432/finance_db

# NextAuth
NEXTAUTH_SECRET=your-secret-key
NEXTAUTH_URL=https://finance.ipmo.my.id/ap

# Security
NODE_ENV=production
```

### Quick Start Commands

| Command | Description |
|---------|-------------|
| `npm dev` | Start development server |
| `npm build` | Build for production |
| `npm start` | Start production server |
| `npm lint` | Run ESLint |
| `npm type-check` | TypeScript type checking |
| `npm prisma:generate` | Generate Prisma client |
| `npm prisma:push` | Push schema changes |
| `npm prisma:seed` | Seed database |

---

*Finance Tracker - Take control of your personal finances!*
