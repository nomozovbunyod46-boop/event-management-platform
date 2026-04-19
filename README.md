# Event Management Platform

A full-stack web application for creating, managing, and joining events with role-based features for participants, organizers, and admins.

## Overview

This project is an event management platform built with a separate **frontend** and **backend** architecture.

Users can register, log in, browse events, view event details, join events, and manage their profiles. Organizers can create and manage events, while admins have access to additional dashboard controls.

## Features

### Authentication
- User registration and login
- JWT-based authentication
- Email verification code support
- Role-based access control

### User Features
- Browse all events
- Search, filter, and sort events
- View event details
- Join events
- View joined events
- Manage personal profile
- Upload avatar
- View public organizer profiles

### Organizer Features
- Create new events
- Edit and delete events
- Upload event images
- View event participants
- Check in participants using ticket codes
- Manage waitlist
- Create and manage promo codes

### Admin Features
- Admin dashboard
- Organizer-level event management access
- Elevated control over platform content

### Event System
- Event categories
- Event images
- Event location and schedule
- Event view tracking
- Participant ticket codes
- Check-in system
- Waitlist support
- Promo code support

## Tech Stack

### Frontend
- React
- TypeScript
- Vite
- Axios
- Radix UI
- Lucide React
- Recharts

### Backend
- Node.js
- Express
- MySQL
- JWT
- bcryptjs
- Nodemailer
- Multer
- Zod

## Project Structure

```bash
event-management-platform/
├── backend/
│   ├── src/
│   │   ├── config/
│   │   ├── controllers/
│   │   ├── middlewares/
│   │   ├── repositories/
│   │   ├── routes/
│   │   ├── scripts/
│   │   ├── services/
│   │   ├── utils/
│   │   └── validators/
│   ├── .env.example
│   └── package.json
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── lib/
│   │   ├── styles/
│   │   └── assets/
│   ├── .env.example
│   └── package.json
│
└── README.md

# 1. Clone the repository
git clone <repo-link>
cd event-management-platform

# 2. Start backend
cd backend
npm install
cp .env.example .env
npm run dev

# 3. Start frontend (open a new terminal)
cd ../frontend
npm install
npm run dev
