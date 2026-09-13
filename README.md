# Dentwise

An AI-powered dental care platform offering seamless appointment scheduling, subscription management, and real-time voice assistance for patients and clinics.

---

## Overview

**Dentwise** is a full-stack SaaS solution built to modernize dental clinic operations. It bridges the gap between healthcare providers and patients by providing intuitive self-service appointment booking, role-based admin controls, transactional email alerts, and an intelligent voice assistant for oral health guidance.

---

## Features

- **AI Voice Assistant**: Interactive, real-time voice assistance powered by Vapi AI for patient queries and oral healthcare advice.
- **Smart Appointment Booking**: Streamlined patient booking flow with doctor selection, date-and-time slots, and instant confirmation.
- **Admin Dashboard**: Comprehensive administration portal to manage doctors, view bookings, and monitor clinic activity.
- **Secure Authentication**: User management, protected routes, and session handling powered by Clerk.
- **Subscription Management**: Tier-based plan access (`Basic`, `Pro`) gating premium AI capabilities.
- **Automated Notifications**: Transactional emails and appointment confirmations sent via Resend and React Email.
- **Responsive & Accessible UI**: Clean, accessible design system built with Tailwind CSS, Shadcn UI, and Radix primitives.

---

## Tech Stack

| Category | Technology |
| :--- | :--- |
| **Framework** | [Next.js 15](https://nextjs.org/) (App Router, Turbopack) |
| **Frontend** | [React 19](https://react.dev/), [TypeScript](https://www.typescriptlang.org/) |
| **Styling & UI** | [Tailwind CSS v4](https://tailwindcss.com/), [Shadcn UI](https://ui.shadcn.com/), [Lucide React](https://lucide.dev/) |
| **State & Fetching** | [TanStack Query v5](https://tanstack.com/query), Server Actions |
| **Database & ORM** | [PostgreSQL](https://www.postgresql.org/), [Prisma ORM](https://www.prisma.io/) |
| **Authentication** | [Clerk](https://clerk.com/) |
| **Voice AI** | [Vapi AI](https://vapi.ai/) |
| **Email Service** | [Resend](https://resend.com/) with [React Email](https://react.email/) |
| **Code Quality** | [Biome](https://biomejs.dev/) |

---

## Getting Started

### Prerequisites

Ensure you have the following installed on your machine:
- **Node.js**: `v18.18.0` or higher
- **npm**, **pnpm**, or **yarn**
- **PostgreSQL** instance (local or hosted via Supabase, Neon, etc.)

### 1. Clone & Install Dependencies

```bash
git clone https://github.com/your-username/dentwise.git
cd dentwise
npm install
```

### 2. Environment Configuration

Copy the example environment file:

```bash
cp .env.example .env.local
```

Fill in your configuration details in `.env.local`:

```env
# Clerk Authentication
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=pk_test_...
CLERK_SECRET_KEY=sk_test_...
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/dashboard
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/dashboard

# Database (PostgreSQL)
DATABASE_URL="postgresql://username:password@localhost:5432/dentwise?schema=public"

# Vapi AI (Voice Assistant)
NEXT_PUBLIC_VAPI_ASSISTANT_ID=your_vapi_assistant_id
NEXT_PUBLIC_VAPI_API_KEY=your_vapi_api_key

# Admin & Notifications
ADMIN_EMAIL=admin@example.com
RESEND_API_KEY=re_...
NEXT_PUBLIC_APP_URL=http://localhost:3000
```

### 3. Database Migration

Generate the Prisma client and push the database schema:

```bash
npx prisma generate
npx prisma db push
```

### 4. Run the Application

Start the local development server:

```bash
npm run dev
```

Visit [`http://localhost:3000`](http://localhost:3000) in your browser.

---

## Project Structure

```text
dentwise/
├── prisma/               # Database schema & migrations
│   └── schema.prisma
├── public/               # Static assets & icons
├── src/
│   ├── app/              # Next.js App Router (pages & API routes)
│   │   ├── admin/        # Admin management dashboard
│   │   ├── appointments/ # Appointment booking flow
│   │   ├── dashboard/    # Patient dashboard
│   │   ├── voice/        # AI voice consultation module
│   │   └── pro/          # Subscription & upgrade page
│   ├── components/       # Reusable UI components & layouts
│   ├── hooks/            # Custom React hooks
│   └── lib/              # Utility functions, Prisma client, server actions
├── biome.json            # Biome linter & formatter configuration
└── package.json
```

---

## Available Scripts

| Command | Description |
| :--- | :--- |
| `npm run dev` | Runs the Next.js development server with Turbopack |
| `npm run build` | Generates Prisma client and creates production build |
| `npm run start` | Runs the compiled production application |
| `npm run lint` | Checks code formatting and lints with Biome |
| `npm run format` | Automatically formats codebase using Biome |

---

## License

This project is licensed under the [MIT License](LICENSE).
