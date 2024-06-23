
# Resource-Corner

A comprehensive collection of links, notes, code snippets, and various other resources to support learning and development.

## Table of Contents
- [Introduction](#introduction)
- [Repository Overview](#repository-overview)
  - [Links](#links)
  - [Notes](#notes)
  - [Code](#code)
  - [Profile](#profile)
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
- [🌼Deploy with Vercel for server side](#Notes6)
  

### Code
- Programming Snippets

### Profile
https://i.ibb.co/9gdS9vP/usman-yousaf-y-IOVi-GQmj-J4-unsplash.jpg
https://i.ibb.co/QcjbGs5/tofan-teodor-Kjht-Jp7-Rh3-E-unsplash.jpg
https://i.ibb.co/Zx8HTV2/harry-pappas-xyaui-SBWRFs-unsplash.jpg
https://i.ibb.co/tMK85PF/rodney-gainous-jr-p-VF71muh-Rs-unsplash.jpg
https://i.ibb.co/Z1q8wdz/jordan-whitfield-Wj-Uy3-NY95y-U-unsplash.jpg
https://i.ibb.co/FVr35Vj/karsten-winegeart-k-Wm6b-XPJl4s-unsplash.jpg
https://i.ibb.co/CHY13Kz/ryan-snaadt-H9-Gr-Uo-Tk-Wr-M-unsplash.jpg
https://i.ibb.co/bz8Dz6B/jackson-schaal-AR9mvykz-SOA-unsplash.jpg
https://i.ibb.co/7jL9vZp/viktor-forgacs-j-BTMr-R6-Q334-unsplash.jpg
https://i.ibb.co/wRPnPZ3/christian-buehner-DIt-Ylc26z-VI-unsplash.jpg
https://i.ibb.co/0jb93bB/petr-sevcovic-au-Cjz0gucr0-unsplash.jpg
https://i.ibb.co/0BTYnvb/clay-elliot-PF7m-P2x-Ce-Qw-unsplash.jpg
https://i.ibb.co/Gvrvnhd/harps-joseph-t-Avp-DE7f-Xg-Y-unsplash.jpg
https://i.ibb.co/PcR9Xjj/andre-sebastian-X6a-MAzo-VJzk-unsplash.jpg
https://i.ibb.co/z4RM7ff/kazi-mizan-Woc-Of-FRUTSM-unsplash.jpg
https://i.ibb.co/WfYKxkk/ryan-hoffman-v7-Jja2-Ch-N6s-unsplash.jpg
https://i.ibb.co/4fb24LJ/zoran-borojevic-f5xi-Gm-Fw-XIU-unsplash.jpg
https://i.ibb.co/z65P8Hk/nartan-buyukyildiz-hr-fe-H2-URs0-unsplash.jpg
https://i.ibb.co/L1TrWZt/albert-dera-ILip77-Sbm-OE-unsplash.jpg
https://i.ibb.co/fHczrnd/jeffrey-keenan-p-Uhxo-Sap-PFA-unsplash.jpg
https://i.ibb.co/hRYxxDr/james-balensiefen-sn-Filgm4-RU-unsplash.jpg
https://i.ibb.co/BgcZZQ7/shipman-northcutt-sg-ZX15-Da8-YE-unsplash.jpg
https://i.ibb.co/5GRtY8R/josh-scorpio-H3-Tuh0hw-YQk-unsplash.jpg
https://i.ibb.co/qxCK9Dx/andre-sebastian-C2-Nf5i-POnz0-unsplash.jpg
https://i.ibb.co/Mh3KVfF/clay-elliot-Hf-MCgq-OLTy-M-unsplash.jpg
https://i.ibb.co/2nNHYhW/jurica-koletic-7-YVZYZe-ITc8-unsplash.jpg
https://i.ibb.co/ZzprBnH/darshan-patel-QJEVpydul-Gs-unsplash.jpg
https://i.ibb.co/C7Zxy2N/alexander-hipp-i-EEBWg-Y-6l-A-unsplash.jpg


<br>

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

```javascript 
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

```javascript 
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

```javascript 
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

```javascript 
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

# Notes6

## 🌼Deploy with Vercel for server side

# Deploying Plant Palace Server to Vercel

## Setting Up Environment Variables
1. Navigate to **Settings > Environment Variables** in your Vercel dashboard.
2. Click **Add** to create a new environment variable.

## Deployment Steps
1. Open your terminal and navigate to your project directory.
2. Run the following command to start the deployment process:

    ```sh
    vercel
    ```

3. Follow the prompts:
    - Set up and deploy: `yes`
    - Scope: `rockyhaque's projects`
    - Link to existing project: `no`
    - Project name: `plant-palace-server`
    - Directory location: `./`

4. Once the project is linked, inspect the deployment at the provided URL.

    ```sh
    Inspect: https://vercel.com/rockyhaques-projects/plant-palace-server/65vgHSVVdRWy6jvj1mCUGx34TxSt
    ```

5. Your project is now live at:

    ```sh
    Production: https://plant-palace-server-hx5v1zdvi-rockyhaques-projects.vercel.app
    ```

6. To overwrite the deployment later, use the following command:

    ```sh
    vercel --prod
    ```

## Production Deployment
1. To deploy to production, run:

    ```sh
    vercel --prod
    ```

2. Inspect the production deployment at:

    ```sh
    Inspect: https://vercel.com/rockyhaques-projects/plant-palace-server/6veHFZGJ57C64zqi21FuBTRdDEy4
    ```

3. Your production project is now live at:

    ```sh
    Production: https://plant-palace-server-2s047nub9-rockyhaques-projects.vercel.app
    ```

## Vercel Configuration

Create a `vercel.json` file in your project directory with the following content:

```json
{
    "version": 2,
    "builds": [
        {
            "src": "./index.js",
            "use": "@vercel/node"
        }
    ],
    "routes": [
        {
            "src": "/(.*)",
            "dest": "/",
            "methods": ["GET", "POST", "PUT", "PATCH", "DELETE", "OPTIONS"]
        }
    ]
}

```

<br> <br>

### Contact

For any inquiries or suggestions, connect with me on [LinkedIn](https://www.linkedin.com/in/rockyhaque).

---

By keeping the repository organized and up-to-date, **resource-corner** aims to be a go-to repository for anyone looking to enhance their knowledge and skills. Enjoy exploring and learning!

