# Women Safety Emergency Alert Assistant

A web app for sending emergency alerts with location details, optional voice/video evidence, and contact notifications.

## Features

- Emergency alert form with live latitude and longitude capture
- Optional media upload for voice or video evidence
- Contact list for emergency recipients
- Backend API for sending alerts and storing records
- Email notification support for emergency contacts
- React + Vite frontend with a Node.js backend

## Tech Stack

- Frontend: React, TypeScript, Vite
- Backend: Node.js, Express
- Email/Storage: Nodemailer, Cloudinary, MongoDB
- AI integration: Gemini API

## Project Structure

- `emergency-alert-assistant/` - frontend application
- `emergency-alert-assistant/backend/` - backend API and services

## Prerequisites

- Node.js 18+
- npm
- A MongoDB Atlas database
- A Gmail app password or SMTP email credentials
- A Cloudinary account
- A Gemini API key for frontend AI features

## 1) Install frontend dependencies

```bash
cd emergency-alert-assistant
npm install
```

## 2) Install backend dependencies

```bash
cd emergency-alert-assistant/backend
npm install
```

## 3) Configure environment variables

Create a `.env.local` file in the frontend folder if required by your app configuration.

For the backend, copy the sample file and replace the values:

```bash
cd emergency-alert-assistant/backend
copy .env.example .env
```

Then update the values in `.env` with your own:

- `MONGODB_URI`
- `GMAIL_CLIENT_EMAIL`
- `GMAIL_PASSWORD`
- `CLOUDINARY_CLOUD_NAME`
- `CLOUDINARY_API_KEY`
- `CLOUDINARY_API_SECRET`
- `PORT`

## 4) Run the backend

```bash
cd emergency-alert-assistant/backend
npm start
```

The API will run on:

- http://localhost:5000

## 5) Run the frontend

Open a new terminal and run:

```bash
cd emergency-alert-assistant
npm run dev
```

Then open the local Vite URL shown in the terminal, usually:

- http://localhost:5173

## 6) Use the app

- Enter the emergency message and location details
- Add recipient email addresses
- Optionally attach a media file
- Send the alert to notify emergency contacts

## Notes

- Keep your `.env` files private and never commit real credentials.
- The backend uses Gmail and Cloudinary, so make sure those services are configured before testing.
- If a feature fails due to missing credentials, verify the secret values in your environment files.

## Repository

- GitHub: https://github.com/ABDULANEEF/WOMEN_SAFETY.git
