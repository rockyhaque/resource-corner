
# Resource-Corner

A comprehensive collection of links, notes, code snippets, and various other resources to support learning and development.

## Table of Contents
- [Introduction](#introduction)
- [Repository Overview](#repository-overview)
  - [Links](#links)
  - [Notes](#notes)
  - [Code](#code)
  - [Miscellaneous](#miscellaneous)
- [Contribution Guidelines](#contribution-guidelines)
- [Contact](#contact)

## Introduction

Welcome to **resource-corner**! This repository, curated by [Rocky Haque](https://www.linkedin.com/in/rockyhaque), serves as a comprehensive collection of diverse resources, including:

- **Links**: Curated links to valuable articles, tutorials, and external resources.
- **Notes**: Detailed notes on various topics to help with study and review.
- **Code**: A variety of code snippets and examples across different programming languages and frameworks.
- **And More**: Additional resources like diagrams, cheat sheets, and tools to aid in learning and development.

Feel free to explore and contribute to the **resource-corner**. Whether you're a student, professional, or hobbyist, this repository aims to be a one-stop resource hub for everyone.

## Repository Overview

### Links
- Technology Blogs
- Educational Videos
- Useful Websites

### Notes
- [How to Setup Google Sign Up Using Firebase](#Notes->1)

### Code
- Programming Snippets

### Miscellaneous
- Diagrams and Infographics



# Notes->1

## How to Setup Google Sign Up Using Firebase

## 1. Create Project
- Create a new Firebase project in the Firebase Console.

## 2. Register App with Web
- Register your app with Firebase.

## 3. Add Firebase SDK
- Run the following command to install Firebase SDK:
  ```bash
  npm install firebase
  ```
## 4. Add Firebase Config File
- Create a config file and add it to your project. Export the app from this file:

> Path: root-folder/src/firebase/firebase.init.js


`
firebase.init.js
`

```
import { initializeApp } from "firebase/app";

const firebaseConfig = {
  // your firebase config here
};

const app = initializeApp(firebaseConfig);

export default app;

```

- Important: Do not publish or publicize your Firebase config by pushing it to GitHub.

## 5. Set Up Firebase Authentication in Docs
- Go to Firebase Console > Docs > Build > Authentication > Web > Get Started

## 6. Create Login Page Component
- Go to Firebase Console > Docs > Build > Authentication > Web > Get Started

- Create a Login Page component:

> Path: root-folder/src/pages/LoginPage.js

`
LoginPage.jsx
`

```
import { getAuth } from "firebase/auth";

import app from "../firebase/firebase.init";

const Login = () => {
  const auth = getAuth(app);
  return (
    <>
    </>
  );
};

export default Login;

```

## 7. Create Login Page Component
- Go to Firebase Console > Docs > Build > Authentication > Web > Get Started

- Update the Login Page component to include Google authentication setup:

```
import { GoogleAuthProvider, getAuth, signInWithPopup } from "firebase/auth";
import app from "../firebase/firebase.init";

const Login = () => {
  const auth = getAuth(app);
  const provider = new GoogleAuthProvider();

  // Step: Create handleGoogleSignIn function
  const handleGoogleSignIn = () => {
    signInWithPopup(auth, provider)
      .then(result => {
        const user = result.user;
        console.log(user);
      })
      .catch(error => {
        console.log('Error', error.message);
      });
  };

  return (
    <>
      {/* Step: Add onClick handler to Google Sign-In button */}

      <button onClick={handleGoogleSignIn}>Sign in with Google</button>
    </>
  );
};

export default Login;

```

## 8. Enable Google Sign-In Provider
- Go to Firebase Console > Build > Authentication > Sign-in method
- Enable Google (and any other providers like Facebook, GitHub, etc...)

### Troubleshooting

If you encounter the error: Firebase: Error (auth/configuration-not-found), try restarting your server.






## Contact

For any inquiries or suggestions, connect with me on [LinkedIn](https://www.linkedin.com/in/rockyhaque).

---

By keeping the repository organized and up-to-date, **resource-corner** aims to be a go-to repository for anyone looking to enhance their knowledge and skills. Enjoy exploring and learning!

