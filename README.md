# EmailAuthPro - React + Vite + Firebase Authentication Starter

A minimal, production-ready starter for email/password authentication using React, Vite, Firebase Auth, and Tailwind CSS. This repo demonstrates clean routing, form validation, and email verification flows - ideal for showcasing authentication work to clients or hiring managers.

## Highlights

- Email/password sign up with validation, display name update, and verification email (see [`Resister`](src/component/Resister/Resister.tsx)).
- Login with validation and password reset (see [`Login`](src/component/Login/Login.tsx)).
- Central layout and routing using React Router (see [`Main`](src/Layout/Main.tsx) and [`src/main.tsx`](src/main.tsx)).
- TypeScript typings for core shapes (see [`User`](src/index.ts), [`AuthState`](src/index.ts), [`FormData`](src/index.ts)).
- Tailwind CSS + optional Bootstrap utilities for fast UI.
- ESLint configured for React | TypeScript | React Refresh.

## Quick demo

- Sign up flow sends email verification: see [`sendVerificationEmail`](src/component/Resister/Resister.tsx).
- Update user's display name after registration: see [`updateUserData`](src/component/Resister/Resister.tsx).
- Reset password flow from login: see [`handleResetPassword`](src/component/Login/Login.tsx).

## Tech stack

- Vite - build and dev tooling ([vite.config.ts](vite.config.ts))
- React 18 - UI
- TypeScript - types and safety
- Firebase Auth - authentication ([firebase.config.ts](src/firebase/firebase.config.ts))
- Tailwind CSS - utility-first styling ([tailwind.config.js](tailwind.config.js), [postcss.config.js](postcss.config.js))
- ESLint - linting ([.eslintrc.cjs](.eslintrc.cjs))

## Project Structure

- Entry and routing: [`src/main.tsx`](src/main.tsx)
- Layout: [`src/Layout/Main.tsx`](src/Layout/Main.tsx) + [`src/Layout/Main.css`](src/Layout/Main.css)
- Components:
  - [`Header`](src/component/Header/Header.tsx) (styles: [`Header.css`](src/component/Header/Header.css))
  - [`Home`](src/component/Home/Home.tsx)
  - [`Login`](src/component/Login/Login.tsx)
  - [`Resister` (Register)](src/component/Resister/Resister.tsx)
- Firebase config: [`src/firebase/firebase.config.ts`](src/firebase/firebase.config.ts)
- Types: [`src/index.ts`](src/index.ts)
- Styles: [`src/index.css`](src/index.css)

## Full File Listing:

- [index.html](index.html)
- [package.json](package.json)
- [vite.config.ts](vite.config.ts)
- [postcss.config.js](postcss.config.js)
- [tailwind.config.js](tailwind.config.js)
- [tsconfig.json](tsconfig.json)
- [.eslintrc.cjs](.eslintrc.cjs)
- [.gitignore](.gitignore)
- [public/vite.svg](public/vite.svg)
- [src/main.tsx](src/main.tsx)
- [src/index.ts](src/index.ts)
- [src/index.css](src/index.css)
- [src/App.jsx](src/App.jsx)
- [src/assets/react.svg](src/assets/react.svg)
- [src/firebase/firebase.config.ts](src/firebase/firebase.config.ts)
- [src/Layout/Main.tsx](src/Layout/Main.tsx)
- [src/Layout/Main.css](src/Layout/Main.css)
- [src/component/Header/Header.tsx](src/component/Header/Header.tsx)
- [src/component/Header/Header.css](src/component/Header/Header.css)
- [src/component/Home/Home.tsx](src/component/Home/Home.tsx)
- [src/component/Login/Login.tsx](src/component/Login/Login.tsx)
- [src/component/Resister/Resister.tsx](src/component/Resister/Resister.tsx)

## Installation

1. **Clone the repo and install dependencies:**

```bash
git clone https://github.com/md-abu-kayser/EmailAuthPro-React-and-Firebase-Starter.git
```

```bash
npm install

```

2. **Run dev server:**
   npm run dev

### Available scripts

npm run dev - start dev server
npm run build - production build
npm run preview - preview build
npm run lint - run ESLint
npm run type-check - TypeScript type-check only

### Firebase configuration

The Firebase app is created in src/firebase/firebase.config.ts. Replace the config object with your own Firebase project values to avoid exposing credentials in public projects.

### Primary exported API used in the app:

default export app from src/firebase/firebase.config.ts

### Project Register | Sign In

create user: createUserWithEmailAndPassword used in Resister
sign in: signInWithEmailAndPassword used in Login
send verification: sendEmailVerification
reset password: sendPasswordResetEmail
update profile: updateProfile

### Forms and validation

### Validation logic is embedded in the components:

- SignUp validation: Resister
- Login validation: Login
  "These are intentionally simple and client-side only. For production, pair them with backend checks and stronger password policies."

### Styling

- Tailwind entry: src/index.css
- Tailwind config: tailwind.config.js
- Bootstrap included from CDN via package: see import in src/main.tsx

#### Notes and Best Practices

- Do not commit real Firebase credentials in public repos. Use environment variables or a server-side proxy for production.
- Expand auth flows to use secure token handling and server-side rules for sensitive operations.
- Add unit and integration tests for auth flows and components.

### License

- This project is licensed under the terms of the **[MIT License](./LICENSE)**.
- You may replace or update the license as needed for client or proprietary projects.

---

### Contact and Maintainer

- **_Name:_** Md Abu Kayser - Full-Stack Engineer
- **_Project:_** EmailAuthPro-React-and-Firebase-Starter\_
- **_Maintainer:_** [md-abu-kayser](https://github.com/md-abu-kayser)
- **_GitHub:_** [github.com/abu.kayser-official](https://github.com/md-abu-kayser)
- **_Email:_** [abu.kayser.official@gmail.com](mailto:abu.kayser.official@gmail.com)

If you’d like this README tailored for a specific purpose - such as **hiring managers**, **open-source contributors**, or **client deliverables** - feel free to request a custom tone or format.

---

**Thank you for reviewing this project!**  
It’s designed to be **clean, well-structured**, and **pleasant to explore** - perfect for showcases, or professional demos.

---
