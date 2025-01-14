# 🚀 criptovaluta Deployment Guide

This guide will help you deploy your **criptovaluta** to **GitHub Pages** step-by-step. 🌟

---

## 🛠️ Prerequisites

Make sure you have the following before proceeding:

- ✅ **React App** ready to be deployed.
- ✅ **GitHub Repository** where your project is pushed.

---

## 📦 Step 1: Install `gh-pages`

In your React project directory, open the terminal and run the following command:

```bash
npm install gh-pages --save-dev
```

This will install the `gh-pages` package needed for deployment. ✅

---

## 🖊️ Step 2: Update `package.json`

### Add the `homepage` field:
Include the following line at the **beginning** of your `package.json` file:

```json
"homepage": "https://<your-github-username>.github.io/<your-repository-name>"
```

👉 Example for this project:  
```json
"homepage": "https://shanmukavenkat.github.io/criptovaluta"
```

### Add `predeploy` and `deploy` scripts:
Under the `"scripts"` section, add these lines:

```json
"predeploy": "npm run build",
"deploy": "gh-pages -d build",
```

Your `"scripts"` section should now look something like this:

```json
"scripts": {
  "start": "react-scripts start",
  "build": "react-scripts build",
  "test": "react-scripts test",
  "eject": "react-scripts eject",
  "predeploy": "npm run build",
  "deploy": "gh-pages -d build"
}
```

---

## 🚀 Step 3: Deploy to GitHub Pages

Now, you're all set to deploy your app! 🎉

1. Push all changes to your GitHub repository using the following commands:

   ```bash
   git add .
   git commit -m "Added gh-pages deployment"
   git push
   ```

2. Run the deploy command in your project terminal:

   ```bash
   npm run deploy
   ```

---

## 🎉 Success!

After running the `npm run deploy` command, your app will be published to **GitHub Pages**. 🚀

👉 You can now view your app at:

```
https://<your-github-username>.github.io/<your-repository-name>
```

For this project:  
**[Crypto-App](https://shanmukavenkat.github.io/criptovaluta)** 🌟

---

## ❤️ Enjoy!

That's it! You've successfully deployed your React app to GitHub Pages. Happy coding! ✨

