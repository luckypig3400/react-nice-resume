# My Resume using template: React Nice Resume :page_with_curl:

## [LIVE DEMO](https://nordicgiant2.github.io/react-nice-resume-page/index.html)

![img](https://github.com/nordicgiant2/react-nice-resume/blob/master/public/images/img.jpg?raw=true)

---

## Description
This project forks from [https://github.com/nordicgiant2/react-nice-resume](https://github.com/nordicgiant2/react-nice-resume), I fork this nice react resume template to build my own resume page, thanks to the [Author](https://github.com/nordicgiant2).

---

## Run or build the Project
### 1. Clone the project

### 2. Run the project
```shell
npm i
npm start
```

### 3. Build
```shell
npm run build
```

---

## Deploy on Github Page

* [Tuturial Article](https://create-react-app.dev/docs/deployment/#github-pages)

### Step1: Add ```homepage``` to ```package.json```

The step below is important!

If you skip it, your app will not deploy correctly.

Open your package.json and add a homepage field for your project:
```json
  "homepage": "https://myusername.github.io/my-app",
```
or for a GitHub user page:
```json
  "homepage": "https://myusername.github.io",
```
**I just use the easier method, for deploying on any Location/Path:**
```json
  "homepage": ".",
```
> Reference: https://create-react-app.dev/docs/deployment/#serving-the-same-build-from-different-paths

### Step2: Install gh-pages and add deploy to scripts in ```package.json```

1. Install necessary package for deploying on Github
```shell
npm install --save gh-pages
```

2. Add deploy script in ```package.json```
```
  "scripts": {
+   "predeploy": "npm run build",
+   "deploy": "gh-pages -d build",
    "start": "react-scripts start",
    "build": "react-scripts build",
```

### Step3: Run the deploy script & finish 😄
```shell
npm run deploy
```