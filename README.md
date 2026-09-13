# Dentwise

<div align="center">
  <img src="/public/screenshot-for-readme.png" alt="Dentwise app preview" width="1200" />
</div>

<p align="center">
  <img src="https://img.shields.io/badge/Next.js-15.5.0-black?logo=next.js&logoColor=white" alt="Next.js 15" />
  <img src="https://img.shields.io/badge/TypeScript-5-blue?logo=typescript&logoColor=white" alt="TypeScript 5" />
  <img src="https://img.shields.io/badge/Prisma-6.16.2-2D3748?logo=prisma&logoColor=white" alt="Prisma" />
  <img src="https://img.shields.io/badge/Tailwind-CSS-38B2AC?logo=tailwindcss&logoColor=white" alt="Tailwind CSS" />
  <img src="https://img.shields.io/badge/Clerk-Auth-6A5CFF?logo=clerk&logoColor=white" alt="Clerk" />
</p>

A modern dental care platform that helps patients book appointments, manage subscriptions, and interact with an AI-powered voice assistant for a seamless healthcare experience.

## ✨ Overview

Dentwise is a full-stack healthcare booking application built for dental clinics. It combines patient-friendly appointment flows, secure authentication, automated email communication, admin management, and AI support into a single platform.

This project was designed to showcase practical product thinking, full-stack development, and modern UI/UX execution for a college placement portfolio.

## 🚀 Key Features

- Smart appointment booking flow for patients
- Secure authentication with Clerk
- Email verification and booking confirmation emails
- Admin dashboard for managing appointments and doctors
- AI voice assistant integration for proactive support
- Subscription plans with upgrade logic
- PostgreSQL database integration using Prisma
- Responsive design with Tailwind CSS and Shadcn UI
- Real-time app experience using TanStack Query

## 🏗️ Tech Stack

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

## 📌 How It Works

1. Users browse the landing page and explore services.
2. They sign in or create an account using Clerk.
3. Patients choose a doctor, preferred time slot, and confirm the appointment.
4. Email notifications are sent automatically for confirmations.
5. Admins can monitor and manage bookings from the dashboard.
6. Pro users can access the AI voice assistant for guided support.

## 🧪 Environment Setup

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

## ▶️ Run Locally

```bash
npm install
npm run dev
```

Then open:

```bash
http://localhost:3000
```

## 📁 Project Structure

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

## 🎯 Project Highlights

- Built as a modern SaaS-style healthcare product
- Focused on customer experience and operational workflows
- Includes both user and admin perspectives
- Suitable for showcasing full-stack problem-solving skills

## 💡 Future Improvements

- Add patient dashboard and appointment history
- Integrate payment gateway for real transactions
- Expand AI voice workflows for triage and reminders
- Add analytics and reporting for clinics

## 🙌 Conclusion

Dentwise is a polished full-stack application that demonstrates practical product building, UI/UX design, backend logic, and AI integration. It is a strong project to present during college placements or internship interviews.

---

Made with care for a modern dental healthcare experience.
