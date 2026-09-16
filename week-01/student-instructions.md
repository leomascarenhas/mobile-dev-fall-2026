# Week 1 - Student Instructions

> **Due: Monday, September 21, 2026 at 23:59** - hand in on Lea.

**This week:** install the tools, run your first app on the Pixel 10 emulator, and push it to GitHub.

**Our standard setup:** Android Studio's Pixel 10 emulator. If it runs there, it counts. Your own
phone (Expo Go) is optional.

## Install, in this order

1. **Node.js**, the LTS version - nodejs.org
2. **VS Code** - code.visualstudio.com
3. **Git** - git-scm.com, then a free account on github.com
4. **Android Studio** - developer.android.com/studio. Accept the standard setup; it downloads about
   15 GB.
5. **The Pixel 10 emulator** - in Android Studio: More Actions, Virtual Device Manager, Phone,
   Pixel 10, the newest Recommended system image, Finish, then press play.

Check the first three in a **new** terminal:

```
node --version
npm --version
git --version
```

"command not found"? Close the terminal and open a new one.

## Steps

1. Create the app and start it. Keep this terminal open, then press `a` with the Pixel 10 running:

   ```
   npx create-expo-app@latest wanderlist
   cd wanderlist
   npx expo start
   ```

2. In VS Code, open `src/app/index.tsx` and replace everything in it: a centred `Text` saying
   "Welcome to Wanderlist", with the app name in a `const` shown with `{ }`. Save and watch the
   emulator update.
3. In a second terminal, inside `wanderlist`, take your first snapshot. Use your GitHub email:

   ```
   git config --global user.name "Your Name"
   git config --global user.email "you@example.com"
   git init
   git add .
   git commit -m "Week 1: welcome screen"
   ```

4. On github.com, create an **empty** repository named `wanderlist` (no README), then push:

   ```
   git remote add origin https://github.com/YOUR-USERNAME/wanderlist.git
   git branch -M main
   git push -u origin main
   ```

   Asked for a password? Sign in through the browser window, or use a personal access token - your
   account password does not work.

## Done when

- [ ] The app runs on the Pixel 10 and says "Welcome to Wanderlist"
- [ ] Your repository on github.com shows your files

## What to submit

One file on Lea (`.md`, `.txt` or `.pdf`), half a page:

1. What does Node.js do, and where does each tool run - your computer or the device?
2. Where are you? Does the app run? Is it on GitHub - paste the link. Where are you stuck?
3. Your JavaScript experience, and the app you would like to build by the end of the course.

This reflection is formative: read and answered, not scored. "I am stuck at the emulator step" is a
good answer.
