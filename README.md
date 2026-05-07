# Zustand Practice App

A simple React application built to practice state management using Zustand.

## Features

* Add courses
* Remove courses
* Toggle course completion status
* Persistent storage using Zustand middleware
* Global state management without Redux

---

# Tech Stack

* React
* Zustand
* JavaScript
* CSS

---

# Zustand Concepts Practiced

* `create()` store creation
* Global state management
* Zustand middleware
* `persist` middleware
* `devtools` middleware
* State selectors
* Updating arrays in state

---

# Project Structure

```txt
src/
 ├── app/
 │    └── courseStore.js
 │
 ├── components/
 │    ├── CourseForm.jsx
 │    └── CourseList.jsx
 │
 ├── App.js
 └── App.css
```

---

# Installation

Clone the repository:

```bash
git clone https://github.com/Nikita-Saxena391/Zustand-practice.git
```

Move into the project folder:

```bash
cd Zustand-practice
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm start
```

---

# Zustand Store Example

```js
import { create } from 'zustand'

const useStore = create((set) => ({
  courses: [],
  addCourse: (course) =>
    set((state) => ({
      courses: [course, ...state.courses],
    })),
}))
```

---

# Learning Outcomes

Through this project, I learned:

* How Zustand simplifies state management
* Difference between Zustand and Redux Toolkit
* Using middleware in Zustand
* Managing global state efficiently in React
* Persisting state using localStorage

---


