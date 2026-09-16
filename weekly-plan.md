# Application Development 2 (Mobile)

## Weekly Plan

> Your roadmap for the term: what each week aims at, what we cover, and the one feature you ship
> toward **"Wanderlist"** - a travel & places planner we build increment by increment. Read each
> week before its first class. Full instructions for each week live in that week's own document.

---

## Week 1: Foundations & First Run

You have an app idea and a phone in your pocket. This week closes the gap between them: the toolbox
installed, a real app running on the standard emulator, a screen that says something you wrote, and
that code safely on GitHub. No prior mobile experience assumed.

**Goals:**

- Know how the course works: the two-app plan, how grading follows the weekly features, and why React Native + Expo.
- Understand where each tool runs - Node.js and the bundler on your computer, the app on the device.
- Run an app on the course's standard target, the **Pixel 10 emulator** (your own phone is optional).
- Write your first component.
- Put the project under Git and push it to GitHub.

**Topics:**

- The big picture: a finished app demoed, where Wanderlist is going, and why this course is database-free.
- The toolbox, installed together with a checkpoint after each step: Node.js, VS Code, Git, Android Studio, the Pixel 10 device.
- A JavaScript/ES6 refresher while editing real code; your first JSX and your first component.
- Git: `init`, `add`, `commit`, push to your own GitHub repository. From now on every week ends with a push.

**Hand-in:** a short written reflection - the toolchain in your own words, where you got stuck, and
what you would like to build. Read and answered, never scored. Code submissions start in Week 2.

---

## Week 2: Components & Styling

Real apps show the same card dozens of times. This week you build one **once** and reuse it -
components and props - and Wanderlist gets its first real screen.

**Goals:**

- Build and reuse your own components, passing data in through props.
- Compose a screen from `View`, `Text`, `Image` and `ScrollView`.
- Lay out and style with `StyleSheet` and Flexbox.

**Topics:**

- Why React groups markup and logic into components, and how JSX becomes real native views.
- Your first `PlaceCard`, fed through props; the Home screen built around it.
- `StyleSheet` and Flexbox: direction, justify, align.
- Consolidation: a one-prop `Badge` lab and a short self-test.

**This week's feature:** a static Home screen with a header and a styled, reusable `PlaceCard`,
pushed to your repository.

---

## Week 3: State & Forms (intro TypeScript)

Your app cannot yet remember anything the user types. This week it learns to react - and the
project switches to TypeScript.

**Goals:**

- Use `useState` and event handlers to make the UI respond.
- Build a controlled, validated `TextInput` form with visible errors.
- Read and write basic TypeScript: type the form and the `Place` it produces.

**Topics:**

- State and re-rendering; handling taps and text changes.
- The "Add a place" form: controlled inputs, validation, conditional error messages.
- The `Place` type, and why the list is typed from here on.

**This week's feature:** a validated "Add a place" form that adds to a typed in-memory list.

---

## Week 4: Lists, Group Build & Final Project Proposal

How does an app show ten thousand posts without crashing? The efficient list. Then the week turns:
you build a small app **from an empty folder**, in a group, using Weeks 1-4 at once - and you plan
the app you will build on your own.

**This week is structured differently from every other one. The list work is not handed in. It is
still on the midterm.**

**Goals:**

- Render collections from arrays with stable keys.
- Display the places with `FlatList` and a reusable row component.
- Handle the empty state so a screen with no data still reads as finished.
- Apply Weeks 1-4 together, from an empty project rather than an existing one.
- Separate the symptom you saw from the cause you found, and write both down.
- Plan your **Final Project** and get the proposal approved.

**Topics:**

- Arrays to UI, and why keys matter.
- `FlatList`, your `PlaceCard` as the row, and a friendly empty state. Supervised build time closes the session.
- Group build: "Grocery Run" from a fresh project, in groups of 3-4 with assigned roles. You are not expected to finish.
- The reflection wall: what you built, what does not work, and your struggles as symptom / what we tried / how it ended - posted anonymously and read together.
- Final Project kickoff: the proposal - problem, target user, 3-5 screens, capabilities, data source.

**This week's assignment:** the **group reflection document**, uploaded by every member, with your
own **Final Project proposal** alongside it. The group app is never submitted.

---

## Week 5: Midterm + Navigation

The week opens with the **midterm** on Weeks 1-4, and it is this week's assignment. The rest of the
week is navigation: real apps are made of many screens, and Wanderlist gets its sections and a
screen for each place.

**Goals:**

- Demonstrate Weeks 1-4 on the midterm (20%).
- Understand file-based routing: the `app/` folder *is* the route table.
- Build tab navigation - Places, Explore, Settings - with Expo Router.
- Open a detail screen on a dynamic route and pass it data through route params.

**Topics:**

- Midterm: a short written section, then an individual build from an empty project.
- `_layout.tsx` as the frame, not a screen; the three tabs.
- Two screens that look deliberate: the Explore placeholder and a real Settings screen.
- A dynamic route, `app/place/[id].tsx`, opened from a list row - and the fact that everything off a route arrives as a string.

**This week's assignment:** the **midterm** itself. There is no separate weekly hand-in: this week's
navigation goes in with Week 6's.

**This week's feature:** three tabs and a detail screen for each place, with the form, list and
empty state all still working behind Places.

---

## Week 6: APIs & Async (Final Build I)

Everything in your app so far is something you typed in yourself. This week it starts pulling real
data off the internet, and stays usable while it waits and when it fails. Your Final Project build
starts too.

**Goals:**

- Call a web API with `fetch` and `async/await`.
- Load on mount with `useEffect`, handling loading and error states.
- Type the data you fetch.
- Start building your Final Project from your approved proposal.

**Topics:**

- Promises and `async/await`; our two keyless APIs (REST Countries, Open-Meteo); typing the response.
- `useEffect` on mount; a loading state and a readable error message, not a frozen screen.
- Studio time on your own project.

**This week's deliverable:** one hand-in carrying **navigation** from Week 5 (tabs, a detail screen
on a dynamic route, params) and the **Explore tab live** (fetched, typed, loading and error states).

---

## Week 7: Persistence & Device (Final Build II)

Close the app and everything is gone. Real apps remember, and they use the device itself.

**Goals:**

- Save and reload data with **AsyncStorage** so places survive a restart.
- Understand why this app stores on-device rather than in a database, and where databases do belong.
- Use one device capability - the camera - to attach a photo to a place.
- Keep building your own Final Project in studio time.

**Topics:**

- AsyncStorage: a small storage helper, saving and loading the list, and the first-run case.
- Why database-free: the database you are learning next door lives on a server and needs a network; a phone often has neither (competency 00SR). We look at what SQLite on a device looks like so the line is clear - awareness only and not assessed. In the Final Project an on-device database is optional, never required and worth no extra marks; a server database stays out of scope.
- The camera: permission, capture, and attaching the photo to a place.
- Studio time on your own project.

**This week's deliverables:** Wanderlist persists across a restart and attaches a photo - the guided
app is done. You also hand in the **Week 7 reflection**: half a page to a page on what the guided
project left you with and where your Final Project stands.

---

## Week 8: Final Project Demos & Submission

You have built one full app with the training wheels on. This week is about finishing your own one
*well*, then presenting it.

**Goals:**

- Structure a project so it stays manageable: folders, screens, navigation.
- Move shared logic into typed hooks and reusable components.
- Present and submit your Final Project (25%).

**Topics:**

- Project layout; a screen orchestrates, it does not fetch and does not save.
- Custom hooks and component reuse; polish before demos.
- Live demos on an emulator or your own phone.
- Catch-up demos for anyone who has not presented yet.

**This week's deliverable:** the **Final Project**, presented live (25%) and its source zip handed
in.

---

## Week 9: Quality - Unit Tests

A demo that worked once tells one story; code that proves it still works tells a better one. This
week is all about unit tests: writing them, and shaping code so it can be tested at all.

**Goals:**

- Write unit tests with `describe`, `it` and `expect`, and see one go red before it goes green.
- Restructure code so it can be tested: pure functions out of screens, the device half split off.

**Topics:**

- What a unit test is, and why most existing code cannot be tested where it stands.
- Pure functions; the `react-native` import as the line between testable and not.
- Tests for the bugs the cohort already had - the first-run `null`, the unexpected response shape.
- A test-first practice lab and a quick check.

**No hand-in this week** - the tests you write here are the ones GitHub runs for you in Week 10.

---

## Week 10: CI/CD + Consolidation

Your tests only help if someone runs them. This week GitHub runs them for you on every push, and
the rest of the week is time to close your gaps before the exam.

**Goals:**

- Put a GitHub Actions workflow on your own repository and watch it go red, then green.
- Understand the D in CI/CD: what a real release is, and why Expo Go is not one.
- Close the gaps you still have before the Final Exam.

**Topics:**

- CI with GitHub Actions: checkout, `npm ci`, typecheck, test, and what a red tick means.
- The D in CI/CD - what a real release is, and why Expo Go is not one.
- Consolidation studio: a practice lab, a quick check, and catch-up time on anything still unfinished.

**No hand-in this week** - the time is yours to get ready for the Final Exam.

---

## Week 11: Review & Final Exam

The last week proves the skills are yours.

**Goals:**

- Consolidate the whole course.
- Demonstrate it on the **Final Exam** (25%).

**Topics:**

- A practice quiz with the answers walked through immediately - the review is built from what it
  exposes, plus whatever you bring that you cannot yet write from memory.
- The exam: the whole course, weighted toward async and APIs, persistence, device features, tests
  and CI/CD, and diagnosing code.
- Course wrap and where to go next.

**The week closes with the Final Exam** - the paper is about two hours of work.

**This week's deliverable:** the completed **Final Exam** (25%).

---
