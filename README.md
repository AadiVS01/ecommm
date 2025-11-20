# E-Commerce App  
**Built with Next.js · Prisma · SQLite · Stripe**

![Next.js](https://img.shields.io/badge/Next.js-000?logo=next.js)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?logo=prisma)
![Stripe](https://img.shields.io/badge/Stripe-626CD9?logo=stripe)
![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)

---

## Overview
A modern full-stack **e-commerce application** built using **Next.js (App Router)**, **Prisma ORM**, **SQLite**, and **Stripe**.  
Includes product pages, cart system, checkout flow, and secure payments.

---

## Tech Stack

- **Next.js 14** – App Router, Server Components  
- **Prisma ORM**  
- **SQLite Database**  
- **Stripe Checkout**  
- **Tailwind CSS**  
- **TypeScript**

---
## Features

- Product listing & product details  
- Cart with persistent state  
- Stripe Checkout integration  
- Order creation & webhook verification  
-  Admin panel 
- Fast server-side rendering  

---


---

## Installation & Setup

### 1. Clone the repository

```bash
git clone <your-repo-url>
cd ecommerce-app
2. Install dependencies
bash

npm install
3. Create .env file
ini

DATABASE_URL="file:./dev.db"

STRIPE_SECRET_KEY=your_stripe_secret_key
STRIPE_WEBHOOK_SECRET=your_webhook_secret
NEXT_PUBLIC_STRIPE_PUBLIC_KEY=your_public_key
4. Setup Prisma
bash

npx prisma migrate dev
5. Run the app
bash

npm run dev
🧪 Stripe Webhooks (Local Testing)
bash

stripe listen --forward-to localhost:3000/api/stripe/webhook
🏗️ Production Build
bash

npm run build
npm start
