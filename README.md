E-Commerce App

A modern, full-stack e-commerce application built with Next.js, Prisma, SQLite, and Stripe.
Supports product browsing, cart management, checkout, and secure online payments.

Tech Stack

Next.js – App Router, server actions, API routes

Prisma ORM – Database modeling & migrations

SQLite – Lightweight, file-based database

Stripe – Secure payments & webhooks

Tailwind CSS – UI styling

TypeScript – Full type safety

Features

User authentication (optional, depends on implementation)

Product listing, filtering & single product page

Add to cart, cart persistence

Stripe checkout integration

Order creation & payment verification

Admin support for adding/editing products (if included)

Project Structure
/app
  /api
    /products
    /checkout
  /cart
  /product/[id]
/prisma
  schema.prisma

Setup & Installation
1. Clone the project
git clone <repo-url>
cd ecommerce-app

2. Install dependencies
npm install

3. Configure environment variables

Create .env:

DATABASE_URL="file:./dev.db"
STRIPE_SECRET_KEY=<your-secret-key>
STRIPE_PUBLIC_KEY=<your-public-key>
STRIPE_WEBHOOK_SECRET=<your-webhook-secret>
NEXT_PUBLIC_STRIPE_PUBLIC_KEY=<your-public-key>

4. Setup Prisma
npx prisma migrate dev

5. Run the development server
npm run dev

Stripe Local Testing

Use Stripe CLI:

stripe listen --forward-to localhost:3000/api/stripe/webhook

Production Build
npm run build
npm start
