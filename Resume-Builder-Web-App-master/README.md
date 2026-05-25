# Resume Builder Web App

A React-based resume builder web application with live preview, customizable color presets, form-guided input, Firebase authentication, and print/download support.

## Overview

This project provides an interactive resume creation experience. Users can enter personal details, education, experience, skills, certifications, projects, and more on the left side and see a live resume preview on the right. The app supports email/password signup and Google authentication via Firebase.

## Key Features

- Landing page with Hero, About, Features, Templates, Review, Contact, and Footer sections
- Email/password registration and login
- Google sign-in with Firebase authentication
- Resume builder page with live preview
- Download/print resume using `react-to-print`
- Prebuilt resume sections for contact, objective, education, experience, certifications, skills, tools, interests, projects, workshops, activities, languages, and references
- Color preset selection for resume styling

## Technologies

- React
- React Router
- React Hook Form
- Firebase Authentication
- Bootstrap 4
- SCSS
- react-to-print

## Installation

From the project root:

```bash
cd "c:\Users\shiwa\OneDrive\Desktop\resume builder web app\Resume-Builder-Web-App-master"
npm install
```

## Development

Start the development server:

```bash
npm start
```

## Build

Create a production build:

```bash
npm run build
```

## Project Structure

- `public/` — static HTML and metadata
- `src/` — application source code
  - `App.js` — main router and page layout
  - `data.json` — default resume data model
  - `components/` — reusable UI and page components
  - `styles/` — SCSS styles

## Authentication

The app uses Firebase Authentication for:

- Email/password sign up
- Email/password sign in
- Google sign in

> Note: The Firebase configuration file is not included in this repo. Create `src/firebase.config.js` with your Firebase project settings.

Example:

```js
const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_AUTH_DOMAIN",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_STORAGE_BUCKET",
  messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
  appId: "YOUR_APP_ID"
};

export default firebaseConfig;
```

## Usage

1. Open the landing page at `/`
2. Go to `/login` to sign in or register
3. Visit `/resume-builder` to create your resume
4. Use the `Download / Print` button to export the resume

