# Resource-Corner

<img src="./assets/cover/top-cover.png" />


![GitHub repo size](https://img.shields.io/github/repo-size/rockyhaque/resource-corner)
![GitHub stars](https://img.shields.io/github/stars/rockyhaque/resource-corner?style=social)
![GitHub forks](https://img.shields.io/github/forks/rockyhaque/rockyhaque?style=social)
[![Follow me on LinkedIn](https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=linkedin&logoColor=white&link=https://www.linkedin.com/in/your-linkedin-handle/)](https://www.linkedin.com/in/your-linkedin-handle/)
[![Follow me on Instagram](https://img.shields.io/badge/-Instagram-E4405F?style=flat-square&logo=instagram&logoColor=white&link=https://www.instagram.com/rocky_haque.10/)](https://www.instagram.com/rocky_haque.10/)
[![Connect with me on Facebook](https://img.shields.io/badge/-Facebook-1877F2?style=flat-square&logo=facebook&logoColor=white&link=https://www.facebook.com/rockyhaquee/)](https://www.facebook.com/rockyhaquee/)


A comprehensive collection of links, notes, code snippets, and various other resources to support learning and development.

## Table of Contents

- [Introduction](#introduction)
- [Repository Overview](#repository-overview)
  - [Tools](#tools)
  - [Links](#links)
  - [Notes](#notes)
  - [Code](#code)
  - [Profile](#profile)
- [Contribution Guidelines](#contribution-guidelines)
- [Contact](#contact)

## Introduction

Welcome to **resource-corner**! This repository, created by [Rocky Haque](https://www.linkedin.com/in/rockyhaque), serves as a comprehensive collection of diverse resources, including:

- **Links**: Curated links to valuable articles, tutorials, and external resources.
- **Notes**: Detailed notes on various topics to help with study and review.
- **Code**: A variety of code snippets and examples across different programming languages and frameworks.
- **And More**: Additional resources like diagrams, cheat sheets, and tools to aid in learning and development.

Feel free to explore and contribute to the **resource-corner**. Whether you're a student, professional, or hobbyist, this repository aims to be a one-stop resource hub for everyone.

## Repository Overview

### Tools

1.  [https://freefrontend.com/tailwind-code-examples](https://freefrontend.com/tailwind-code-examples/)
2.  [https://pagedone.io](https://pagedone.io)
3.  [https://headlessui.com](https://headlessui.com)
4.  [https://componentland.com](https://componentland.com)
5.  [https://www.npmjs.com/package/react-toastify](https://www.npmjs.com/package/react-toastify)
6.  [https://whimsical.com/a ](https://whimsical.com/a )
7.  [https://caniuse.com](https://caniuse.com)
8.  [https://www.framer.com](https://www.framer.com)
9.  [https://undraw.co](https://undraw.co)

### Links

- [https://dev.to](https://dev.to)

### Notes

1.  [How to Setup Google Sign In Using Firebase](#Notes1)
2.  [How to Setup Github Sign In Using Firebase](#Notes2)
3.  [Firebase Deploye 🌼](#Notes3)
4.  [Firebase Hosting Setup Complete Issue 😥](#Notes4)
5.  [Deploy to Netlify 🌼](#Notes5)
6.  [Deploy with Vercel for server-side 🌼](#Notes6)
7.  [Theme Switcher Documentation with DaisyUI 🌩️ ](#Notes7)
8.  [Basic Server setup with node & express js 🖥️ ](#Notes8)
9.  [Complete Server setup with JWT, MongoDB, Node & Express js ](#Notes9)
10. [Basic Contibution at Github](#Note10)
11. [Upload image with `imgbb` api](#Note-11)
12. [Custom Loading Spinner using react spiner](#Note-12)
13. [Empty Content with react spinners](#Note-13)
14. [Quick Animation with AOS](#Note-14)


### Code

1.  [Shared Section Title with description](#Code-1)
2.  [Section Heading with gradient underline](#Code-2)

### Profile

1. [https://i.ibb.co/9gdS9vP/usman-yousaf-y-IOVi-GQmj-J4-unsplash.jpg](https://i.ibb.co/9gdS9vP/usman-yousaf-y-IOVi-GQmj-J4-unsplash.jpg)
2. [https://i.ibb.co/QcjbGs5/tofan-teodor-Kjht-Jp7-Rh3-E-unsplash.jpg](https://i.ibb.co/QcjbGs5/tofan-teodor-Kjht-Jp7-Rh3-E-unsplash.jpg)
3. [https://i.ibb.co/Zx8HTV2/harry-pappas-xyaui-SBWRFs-unsplash.jpg](https://i.ibb.co/Zx8HTV2/harry-pappas-xyaui-SBWRFs-unsplash.jpg)
4. [https://i.ibb.co/tMK85PF/rodney-gainous-jr-p-VF71muh-Rs-unsplash.jpg](https://i.ibb.co/tMK85PF/rodney-gainous-jr-p-VF71muh-Rs-unsplash.jpg)
5. [https://i.ibb.co/Z1q8wdz/jordan-whitfield-Wj-Uy3-NY95y-U-unsplash.jpg](https://i.ibb.co/Z1q8wdz/jordan-whitfield-Wj-Uy3-NY95y-U-unsplash.jpg)



<br><br>

## Code-1

### Shared Section Title with description

```jsx
const SectionTitle = ({heading, description}) => {
    return (
        <div className="mx-auto text-center md:w-4/12 my-8 ">
            <h3 className="text-2xl md:text-4xl font-extrabold py-4 font-nunitoSans text-gray-800" data-aos="fade-right">{heading}</h3>
            <p className="font-roboto text-gray-600" data-aos="fade-left">{description}</p>
        </div>
    );
};

export default SectionTitle;
```

## Code-2

### Section Heading with gradient underline

```jsx
const SectionHeading = ({ heading }) => {
    return (
      <div className="relative mx-auto text-center md:w-6/12 my-12">
        {/* Curved decorative element behind the heading */}
        <div className="absolute inset-x-0 -top-8 transform rotate-3 opacity-20 bg-gradient-to-r from-indigo-400 via-purple-400 to-pink-400 h-14 w-full rounded-full blur-2xl"></div>
        
        {/* Main Heading */}
        <h3 className="relative z-10 text-xl md:text-3xl font-extrabold font-nunitoSans py-4 bg-gradient-to-r from-indigo-900 via-cyan-900 to-pink-500 text-transparent bg-clip-text drop-shadow-lg">
          {heading}
        </h3>
  
        {/* Subtle glowing line below the heading */}
        <div className="relative mx-auto mt-1 w-20 h-1 bg-gradient-to-r from-indigo-600 via-purple-600 to-pink-500 rounded-full before:absolute before:-inset-1 before:bg-glow before:blur-md before:opacity-60"></div>
  
        {/* Bottom curved decoration */}
        <div className="absolute inset-x-0 bottom-0 transform rotate-[-2deg] opacity-10 bg-gradient-to-r from-indigo-400 via-purple-400 to-pink-400 h-10 w-full rounded-full blur-xl"></div>
      </div>
    );
  };
  
  export default SectionHeading;
  
```

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

`firebase.init.js`

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

`LoginPage.jsx`

```javascript
import { getAuth } from "firebase/auth";

import app from "../firebase/firebase.init";

const Login = () => {
  const auth = getAuth(app);
  return <></>;
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
      .then((result) => {
        const user = result.user;
        console.log(user);
      })
      .catch((error) => {
        console.log("Error", error.message);
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

<br> <br>

<hr>

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
      .then((result) => {
        const loggedInUser = result.user;
        console.log(loggedInUser);
        // Log the user object to see all properties
        setUser(loggedInUser);
      })
      .catch((error) => {
        console.log("Error", error.message);
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

<br> <br>

<hr>

# Notes3

## 🌼Firebase Deploy


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
npm run build
```

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

```
firebase init
```

**_skip if already installed_**

```
npm install -g firebase-tools
```

```
firebase login
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

<br> <br>

<hr>

# Notes5

## 🌼Deploy to Netlify

**Step 1:** Create `_redirects` File

In your public folder, create a file named \_redirects with the following content:

```
/* /index.html 200
```

**Step 2:** Build the Project

```
npm run build
```

**Step 3:** Deploy to Netlify

> Sign in to Netlify.

> Go to "Sites" and scroll down.

> Drag and drop your dist folder to deploy.

**Step 4:** Configure Firebase Authentication (If Applicable)

If you use Firebase Authentication, ensure it works with your Netlify deployment:

> Go to the Firebase Console.

> Click on the "Authentication" menu, then the "Settings" tab.

> Scroll down to "Authorized domains".

> Click "Add domain" and enter your Netlify URL.

<br> <br>

<hr>

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

<hr>

# Notes7

# Theme Switcher Documentation

This documentation provides a step-by-step guide to implementing a theme switcher using Tailwind CSS and DaisyUI. Follow the instructions below to configure your project.

## 1. Configure Tailwind CSS

In your tailwind.config.js file, add the DaisyUI themes configuration:

```
daisyui: {

themes: [ "light", "dark", "cupcake", "bumblebee", "emerald", "corporate", "synthwave",
"retro", "cyberpunk", "valentine", "halloween", "garden", "forest", "aqua", "lofi", "pastel",
"fantasy", "wireframe", "black", "luxury", "dracula", "cmyk", "autumn", "business", "acid",
"lemonade", "night", "coffee", "winter", "dim", "nord", "sunset" ]

}
```

## 2. Create State in Navbar Component

In your Navbar.jsx file, create a state to manage the current theme:

```
const [theme, setTheme] = useState("light");
```

## 3. Persist Theme in Local Storage

Use `useEffect` to set the theme in localStorage and apply it when the page mounts:

```
useEffect(() => {
localStorage.setItem("theme", theme);
const localTheme = localStorage.getItem("theme");
document.querySelector("html").setAttribute("data-theme", localTheme);
}, [theme]);

```

## 4. Add Theme Controller Components

Include the DaisyUI theme controller component in your Navbar. Refer to the

[DaisyUI Theme Controller Components for more details.](https://daisyui.com/components/theme-controller)

Example component:

```
    <label className="cursor-pointer grid place-items-center ml-6">
            <input
              onChange={handleThemeToggle}
              type="checkbox"
              className="toggle theme-controller bg-base-content row-start-1 col-start-1 col-span-2"
            />
            <svg
              className="col-start-1 row-start-1 stroke-base-100 fill-base-100"
              xmlns="http://www.w3.org/2000/svg"
              width="14"
              height="14"
              viewBox="0 0 24 24"
              fill="none"
              stroke="currentColor"
              strokeWidth="2"
              strokeLinecap="round"
              strokeLinejoin="round"
            >
              <circle cx="12" cy="12" r="5" />
              <path d="M12 1v2M12 21v2M4.2 4.2l1.4 1.4M18.4 18.4l1.4 1.4M1 12h2M21 12h2M4.2 19.8l1.4-1.4M18.4 5.6l1.4-1.4" />
            </svg>
            <svg
              className="col-start-2 row-start-1 stroke-base-100 fill-base-100"
              xmlns="http://www.w3.org/2000/svg"
              width="14"
              height="14"
              viewBox="0 0 24 24"
              fill="none"
              stroke="currentColor"
              strokeWidth="2"
              strokeLinecap="round"
              strokeLinejoin="round"
            >
              <path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79z"></path>
            </svg>
    </label>
```

> **_Note:_** Remove the value property from the input field to make it dynamic and add onChange={handleThemeToggle}.

## 5. Create Theme Toggle Function

Add a function to handle the theme toggle:

```
const handleThemeToggle = (e) => {
    if(e.target.checked){
        setTheme("dracula");
    } else {
        setTheme("light");
    }
};

```

Now enjoy your theme switcher

<br> <br>

<hr>

# Notes8

# Basic Server setup with node & express js 🖥️

### 🔰Step - 1:

```
mkdir <Folder Name>
```

```
cd <Folder Name>
```

```
npm init -y
```

```
npm install express cors dotenv
```

<br>
  
### 🔰Step - 2:
- Create index.js file inside the server folder
- Add  "start": "node index.js", inside the  scripts in package.json file

<br>

### 🔰Step - 3:

```javascript
const express = require("express");
const app = express();
const cors = require("cors");

// config
require("dotenv").config();
const port = process.env.PORT || 5000;

// middleware
const corsOptions = {
  origin: ["http://localhost:5173", "http://localhost:5174"],
  credentials: true,
  optionSuccessStatus: 200,
};
app.use(cors(corsOptions));
app.use(express.json());

app.get("/", (req, res) => {
  res.send("Server is running...");
});

app.listen(port, () => {
  console.log(`Server is running on port ${port}`);
});
```

<br> <br>

<hr>

# Notes9

# Complete Server setup with JWT, MongoDB, Node & Express JS

### 🔰Step - 1:

```
mkdir <Folder Name>
```

```
cd <Folder Name>
```

```
npm init -y
```

```
npm install express cors dotenv cookie-parser jsonwebtoken mongodb
```

<br>
  
### 🔰Step - 2:
- Create index.js file inside the server folder
- Add  "start": "node index.js", inside the  scripts in package.json file

<br>

### 🔰Step - 3:

```javascript
const express = require("express");
const app = express();
const cors = require("cors");
const jwt = require("jsonwebtoken");
const cookieParser = require("cookie-parser");
const { MongoClient, ServerApiVersion, ObjectId } = require("mongodb");

// config
require("dotenv").config();
const port = process.env.PORT || 5000;

// middleware
const corsOptions = {
  origin: ["http://localhost:5173", "http://localhost:5174"],
  credentials: true,
  optionSuccessStatus: 200,
};
app.use(cors(corsOptions));
app.use(express.json());
app.use(cookieParser());

// verify jwt middleware
const verifyToken = (req, res, next) => {
  const token = req.cookies?.token;
  if (!token) {
    return res.status(401).send({ message: "Unauthorized Access!" });
  }
  if (token) {
    jwt.verify(token, process.env.ACCESS_TOKEN_SECRET, (error, decoded) => {
      if (error) {
        return res.status(401).send({ message: "Unauthorized Access!" });
      }
      req.user = decoded;
      next();
    });
  }
};

//--------------------- database connection-----------------------
//Todo: Change the cluster name
const uri = `mongodb+srv://${process.env.DB_USER}:${process.env.DB_PASS}@revive.2tkcldw.mongodb.net/?appName=Revive`;

// Create a MongoClient with a MongoClientOptions object to set the Stable API version
const client = new MongoClient(uri, {
  serverApi: {
    version: ServerApiVersion.v1,
    strict: true,
    deprecationErrors: true,
  },
});

async function run() {
  try {
    // Connect the client to the server	(optional starting in v4.7)
    await client.connect();

    //Todo: database and collection

    // JWT Generate
    app.post("/jwt", async (req, res) => {
      const user = req.body;
      const token = jwt.sign(user, process.env.ACCESS_TOKEN_SECRET, {
        expiresIn: "7d",
      });
      res
        .cookie("token", token, {
          httpOnly: true,
          secure: process.env.NODE_ENV === "production",
          sameSite: process.env.NODE_ENV === "production" ? "none" : "strict",
        })
        .send({ success: true });
    });

    // clear token with logout
    app.get("/logout", (req, res) => {
      res
        .clearCookie("token", {
          httpOnly: true,
          secure: process.env.NODE_ENV === "production",
          sameSite: process.env.NODE_ENV === "production" ? "none" : "strict",
          maxAge: 0,
        })
        .send({ success: true });
    });

    //Todo: Create your API here

    // Send a ping to confirm a successful connection
    await client.db("admin").command({ ping: 1 });
    console.log(
      "Pinged your deployment. You successfully connected to MongoDB!"
    );
  } finally {
    // Ensures that the client will close when you finish/error
    // await client.close();
  }
}
run().catch(console.dir);

app.get("/", (req, res) => {
  res.send("Your server is running...");
});

app.listen(port, () => {
  console.log(`Server is running on port ${port}`);
});
```

<br> <br>

<hr>

# Note10

# Basic Contibution at Github

## As a Contributor:

<h4>To contribute to this project, follow these steps:</h4>

1. Fork the Repository:
   - Fork the repository to your own GitHub account.
2. Clone the Repository:

   - Clone the forked repository to your local machine

   <br>

   ```
   git clone https://github.com/<your-username>/<repository-name>.git
   ```

3. Create a New Branch:

   - Before making any changes, create a new branch:

     - To see all branches:

     <br>

     ```
     git branch
     ```

     - To switch to the main branch:

     <br>

     ```
     git checkout main
     ```

     - To create a new branch:

     <br>

     ```
     git branch <new-branch-name>
     ```

     - Alternatively, create and switch to a new branch in one command:

     <br>

     ```
     git checkout -b <new-branch-name>
     ```

4. Update Your Work:

   Make your changes to the code.

   - If you make any changes to the existing code, commit those changes with a message:

    <br>

   ```
   git commit -am "Description of changes"
   ```

   - If you create new files, stage and commit them:

    <br>

   ```
   git add .
   git commit -am "Message for new file code"

   ```


5. Push Changes to Your Forked Repository:

    - Push your changes to your branch on your forked repository:

     <br>

     ```
     git push origin <new-branch-name>
     ```


6. Create a Pull Request:
    - Go to the original repository on GitHub.
    - Click on the "Compare & pull request" button.
    - Provide a meaningful description of the changes you have made.
    - Click on "Create Pull Request" to submit your changes for review.



## As the Repository Owner:

1. Review the Pull Request:
    - Review the changes submitted by the contributor.
    - Ensure the changes align with the project's goals and standards.

2. Merge the Pull Request:
    - Once satisfied with the changes, confirm the merge to incorporate the contributor's changes into the main branch.


## After the Merge (For Contributors):

<h4>If your changes have been merged by the owner, update your local repository to stay in sync with the main repository:</h4>

```
git pull origin main
```


# Note-11

## Upload image with `imgbb` api


1. Get the API key from imgbb developer API and add on `.env` file

```
VITE_IMGBB_API_KEY=****
```

2. Install Axios & proptypes(To handle prop validation)

```
npm i axios proptypes
```


3. > src > api > index.js

```js

import axios from "axios";

export const imageUpload = async (image) => {

  const formData = new FormData();
  formData.append("image", image);

  const { data } = await axios.post(
    `https://api.imgbb.com/1/upload?key=${import.meta.env.VITE_IMGBB_API_KEY}`,
    formData
  );

  return data.data.display_url;
};
```


# Note-12

### Custom Loading Spinner using react spiner

Install [React Spinners](https://www.davidhu.io/react-spinners) with Prop Types

    ```
    npm i react-spinners prop-types
    ```

    ```jsx
    import PropTypes from 'prop-types'
    import { HashLoader } from 'react-spinners'

    const LoadingSpinner = ({ smallHeight }) => {
      return (
        <div
          className={` ${smallHeight ? 'h-[250px]' : 'h-[70vh]'}
          flex 
          flex-col 
          justify-center 
          items-center `}
        >
          <HashLoader size={100} color='#421d81' />
        </div>
      )
    }

    LoadingSpinner.propTypes = {
      smallHeight: PropTypes.bool,
    }

    export default LoadingSpinner
    ```

# Note-13

### Empty Content with react spinners

1. Install [React Spinners](https://www.davidhu.io/react-spinners)

    ```
    npm i react-spinners
    ```

2. You can modify with `ClimbingBoxLoader`

    ```jsx

    import { ClimbingBoxLoader } from 'react-spinners';

    const EmptyContent = ({title, subTitle}) => {
        return (
            <div className="flex items-center justify-center mb-8">
              <div className="text-center">
                <div className="flex items-center justify-center">
                  <ClimbingBoxLoader size={12} color="#421d81" />
                </div>
                <h2 className="text-lg md:text-xl font-semibold text-gray-800">
                  {title}
                </h2>
                <p className="text-gray-500 mt-2">{subTitle}</p>
              </div>
            </div>
        );
    };

    export default EmptyContent;
    ```


# Note-14

### Quick Animation with [AOS](https://michalsnik.github.io/aos)

1. Install AOS

    ```
    npm i aos
    ```

2. To get access for every component use in `Root Layout`

    ```js

    import AOS from "aos";
    import "aos/dist/aos.css";

    const Root = () => {

      useEffect(() => {
        AOS.init({ duration: 2000 });
      }, []);

      return (
        <h3 className="text-2xl" data-aos="fade-right">Animation Content</h3>
      )
    }
      
    ```

    > NOTE: Make change here `data-aos="fade-right"`



### Contact

For any inquiries or suggestions, connect with me on [LinkedIn](https://www.linkedin.com/in/rockyhaque).

---

By keeping the repository organized and up-to-date, **resource-corner** aims to be a go-to repository for anyone looking to enhance their knowledge and skills. Enjoy exploring and learning!
