# Shopsify (Snapcart)

A full-stack e-commerce platform featuring real-time delivery tracking, live chat with AI suggestions, and comprehensive role-based dashboards.

##  Key Features

- ** E-commerce:** Full cart and checkout functionality with Stripe payments.
- ** Role-Based Access:** Distinct dashboards for **Admin**, **User**, and **Delivery Boy**.
- ** Real-Time Tracking:** Live delivery location updates using Leaflet maps and Socket.io.
- ** Live Chat:** Real-time messaging system with AI-powered response suggestions.
- ** Authentication:** Secure login via NextAuth (Google & Credentials).

##  Tech Stack

- **Frontend:** Next.js 15 (App Router), TypeScript, Tailwind CSS, Redux Toolkit.
- **Backend:** Next.js API Routes, Node.js (Socket Server), Express.
- **Database:** MongoDB (Mongoose).
- **Real-time:** Socket.io.
- **External Services:** Cloudinary (Media), Stripe (Payments), Google Gemini (AI).

##  Project Structure

- **`1.snapcart/`**: The main Next.js application containing the frontend and API routes.
- **`socketServer/`**: A dedicated Node.js/Express server handling real-time socket connections.

##  Getting Started

### 1. Setup Frontend (Next.js)
Navigate to the main app folder and install dependencies:
```bash
cd 1.snapcart
npm install
```
Create a `.env.local` file in `1.snapcart/` and add your environment variables (MongoDB, Stripe, Cloudinary, NextAuth).

Run the development server:
```bash
npm run dev
```

### 2. Setup Socket Server
Navigate to the socket server folder:
```bash
cd socketServer
npm install
```
Create a `.env` file in `socketServer/` with:
```env
PORT=5000
NEXT_BASE_URL=http://localhost:3000
```
Run the socket server:
```bash
npm run dev
```

##  Deployment

- **Frontend:** Deploy the `1.snapcart` directory to **Vercel**.
- **Socket Server:** Deploy the `socketServer` directory to **Render** or similar platforms.

---
Built with ❤️ by Vinishvats14
