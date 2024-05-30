
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

### Notes
- [How to Setup Google Sign In Using Firebase](#Notes1)
- [How to Setup Github Sign In Using Firebase](#Notes2)
- [🌼Firebase Deploye](#Notes3)
- [Firebase Hosting Setup Complete Issue 😥](#Notes4)
- [🌼Deploy to Netlify](#Notes5)
  

### Code
- Programming Snippets

### Miscellaneous
- Diagrams and Infographics



# Notes1

## How to Setup Google Sign Up Using Firebase

### 1. Create Project
- Create a new Firebase project in the Firebase Console.

### 2. Register App with Web
- Register your app with Firebase.

### 3. Add Firebase SDK
- Run the following command to install Firebase SDK:
  ```bash
  npm install firebase
  ```
### 4. Add Firebase Config File
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

### 5. Set Up Firebase Authentication in Docs
- Go to Firebase Console > Docs > Build > Authentication > Web > Get Started

### 6. Create Login Page Component
- Go to Firebase Console > Docs > Build > Authentication > Web > Get Started

- Create a Login Page component:

> Path: root-folder/src/pages/LoginPage.js

`
LoginPage.jsx
`

```react
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

### 7. Create Login Page Component
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

### 8. Enable Google Sign-In Provider
- Go to Firebase Console > Build > Authentication > Sign-in method
- Enable Google (and any other providers like Facebook, GitHub, etc...)

### Troubleshooting

If you encounter the error: Firebase: Error (auth/configuration-not-found), try restarting your server.

<br><br>

# Notes2

# How to Setup Firebase Sign Up Using GitHub

### 1. Enable GitHub Provider in Firebase
- Go to Firebase Console > Build > Authentication > Sign-in method
- Enable the GitHub provider.

### 2. Configure GitHub Provider
- Add the Client ID and Client Secret from the GitHub developer console to the provider configuration in Firebase.

### 3. Create a GitHub App
- Go to your GitHub profile > Settings > Developer settings > New GitHub App
- Set the Callback URL to the one provided in the Firebase Console when enabling the GitHub sign-in provider.
- Complete the requirements to create the GitHub app. You will get the `Client ID`.
- To get the `Client Secret`, click on `Generate New Client Secret`.

### 4. Set Up Firebase Authentication in Docs
- Go to Firebase Console > Docs > Build > Authentication > Web > GitHub

### 5. Update Login Page Component for GitHub Authentication
- Add GitHub authentication to the Login Page component:

```
  import { GithubAuthProvider, getAuth, signInWithPopup } from "firebase/auth";
  import app from "../firebase/firebase.init";
  import { useState } from "react";

  const Login = () => {
    const [user, setUser] = useState(null);
    const auth = getAuth(app);
    const githubProvider = new GithubAuthProvider();

    // GitHub Sign-In function
    const handleGithubSignIn = () => {
      signInWithPopup(auth, githubProvider)
        .then(result => {
          const loggedInUser = result.user;
          console.log(loggedInUser); 
          // Log the user object to see all properties
          setUser(loggedInUser);
        })
        .catch(error => {
          console.log('Error', error.message);
        });
    };

    return (
      <div>
        <div className="text-center mt-24">
          <h2 className="text-4xl tracking-tight mb-10">
            Sign in into your account
          </h2>
        </div>
        <div className="flex flex-col justify-center my-2 mx-4 md:mx-0">
          <div className="w-full md:w-full px-3 mb-6">
            <button
              onClick={handleGithubSignIn}
              className="appearance-none block w-full bg-purple-700 text-gray-100 font-bold border border-gray-200 rounded-lg py-3 px-3 leading-tight hover:bg-blue-500 focus:outline-none focus:bg-white focus:border-gray-500"
            >
              Sign in with GitHub
            </button>
          </div>

          <div>
            {user && (
              <div>
                <h3>User: {user.displayName}</h3>
                <h4>Email: {user.email}</h4>
                {user.photoURL ? (
                  <img src={user.photoURL} alt="User profile" />
                ) : (
                  <p>No photo available</p>
                )}
              </div>
            )}
          </div>
        </div>
      </div>
    );
  };

  export default Login;

```
<br><br>

# Notes3

## 🌼Firebase Deploy

```
npm run build
```

```
firebase init
```


> Are you ready to proceed -> `y`

> Hosting: Configure files for Firebase Hosting and (optionally) set up GitHub Action deploys

> Use an existing project

> What do you want to use as your public directory? -> `dist`

> Configure as a single-page app (rewrite all urls to /index.html)? -> `y`

> Set up automatic builds and deploys with GitHub? `n`

```
firebase deploy
```

<br><br>

# Notes4

## ❗Firebase Hosting Setup Complete Issue 😥

You might have accidentally typed y and pressed enter for:

> What do you want to use as your public directory? `y`

If the live link page shows like this:

❗Welcome Firebase Hosting Setup Complete You're seeing this because you've successfully setup Firebase Hosting. Now it's time to go build something extraordinary!

**Solution**

**Step 1:** Replace index.html


Replace the contents of index.html in your root folder with:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <link rel="icon" type="image/svg+xml" href="/vite.svg" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>My-react-app</title>
  </head>
  <body>
    <div id="root"></div>
    <script type="module" src="/src/main.jsx"></script>
  </body>
</html>
```

**Step 2:** Delete Specific Folders and Files Delete the `dist` folder, `.firebase`, `.firebaserc`, and `firebase.json`.


**Step 3:** Run Commands in Terminal

Open PowerShell (or Git Bash if PowerShell gives errors) and run:


```
npm install firebase

```
***skip if already installed***
```
npm install -g firebase-tools
```

```
firebase login
```
```
firebase init
```

Follow these prompts:

> Are you ready to proceed?: `y`

> Select Hosting: `Hosting: Configure files for Firebase Hosting`

> Use an existing project: **Select your project**

> Public directory: Type `dist`

> Single-page app: `y`

> Automatic builds and deploys with GitHub: `n`

> Overwrite dist/index.html: `y` (if prompted)

```
npm run build
```

```
firebase deploy
```

**Step 4:** Verify Deployment

After deployment, open Chrome, check your live link, open the console tab, right-click the refresh button, and select "Empty Cache and Hard Reload" 3-4 times.

<br><br>

# Notes5

## 🌼Deploy to Netlify

**Step 1:** Create `_redirects` File

In your public folder, create a file named _redirects with the following content:

```
/* /index.html 200
```

**Step 2:** Build the Project

```
npm run build
```

**Step 3:** Deploy to Netlify

>Sign in to Netlify.

> Go to "Sites" and scroll down.

> Drag and drop your dist folder to deploy.


**Step 4:** Configure Firebase Authentication (If Applicable)

If you use Firebase Authentication, ensure it works with your Netlify deployment:

> Go to the Firebase Console.

> Click on the "Authentication" menu, then the "Settings" tab.

> Scroll down to "Authorized domains".

> Click "Add domain" and enter your Netlify URL.


<br><br>

### Contact

For any inquiries or suggestions, connect with me on [LinkedIn](https://www.linkedin.com/in/rockyhaque).

---

By keeping the repository organized and up-to-date, **resource-corner** aims to be a go-to repository for anyone looking to enhance their knowledge and skills. Enjoy exploring and learning!

