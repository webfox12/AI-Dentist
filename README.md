# Dentwise

A modern dental care platform for appointment booking, subscriptions, and AI-powered patient support.

## Overview

Dentwise is a full-stack healthcare application designed for dental clinics. It includes patient-friendly appointment booking, secure login, admin management, automated email communication, and AI voice assistance.

The project is built to demonstrate practical product development, modern frontend design, and backend integration for a college placement portfolio.

## Key Features

- Appointment booking flow for patients
- Authentication and user management with Clerk
- Email verification and confirmation notifications
- Admin dashboard for managing doctors and appointments
- AI voice assistant integration
- Subscription plans with upgrade logic
- PostgreSQL database using Prisma
- Responsive UI built with Tailwind CSS and Shadcn
- Client-side data handling with TanStack Query

## Tech Stack

| Category       | Stack                      |
| -------------- | -------------------------- |
| Frontend       | Next.js, React, TypeScript |
| Styling        | Tailwind CSS, Shadcn UI    |
| Backend        | Next.js API routes         |
| Database       | PostgreSQL, Prisma ORM     |
| Authentication | Clerk                      |
| Emails         | Resend                     |
| Voice AI       | Vapi                       |
| Data Fetching  | TanStack Query             |
| Deployment     | Sevalla                    |

## How It Works

1. Users browse the platform and explore available services.
2. Patients sign in or create an account.
3. They select a doctor, time slot, and confirm an appointment.
4. Confirmation emails are sent automatically.
5. Admins manage bookings and clinic data from the dashboard.
6. Premium users can access the AI voice assistant for guided support.

## Environment Setup

Create a `.env.local` file and add the following:

```bash
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
CLERK_SECRET_KEY=your_clerk_secret_key

DATABASE_URL=your_postgres_database_url

NEXT_PUBLIC_VAPI_ASSISTANT_ID=your_vapi_assistant_id
NEXT_PUBLIC_VAPI_API_KEY=your_vapi_api_key

ADMIN_EMAIL=your_admin_email

RESEND_API_KEY=your_resend_api_key

NEXT_PUBLIC_APP_URL=your_app_url
```

## Run Locally

```bash
npm install
npm run dev
```

Open the app in your browser at:

```bash
http://localhost:3000
```

## Project Structure

```bash
.
├── src/
│   ├── app/
│   ├── components/
│   ├── hooks/
│   └── lib/
├── prisma/
├── public/
├── package.json
├── next.config.ts
├── tsconfig.json
├── README.md
└── .env.local
```

## Project Highlights

- Built as a modern SaaS-style healthcare product
- Focused on user experience and operational workflow
- Includes both patient and admin perspectives
- Demonstrates full-stack development and product thinking

## Future Improvements

- Add patient dashboard and appointment history
- Integrate a payment gateway for real transactions
- Expand AI voice workflows for reminders and triage
- Add analytics and reporting for clinic performance

## Conclusion

Dentwise is a polished full-stack application that demonstrates practical product building, UI design, backend logic, and AI integration. It is suitable for showcasing your technical skills during college placements or internship interviews.

---

Dentwise Project
