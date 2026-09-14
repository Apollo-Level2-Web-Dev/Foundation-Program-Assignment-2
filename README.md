# 🎬 Assignment: Movie Explorer

> **Objective:** Build a responsive **Movie Explorer Application** using React. Users should be able to browse movies, search for specific titles, and view detailed information in an interactive modal.

---

## 🛠️ Technology Stack

* **Core:** JavaScript, React
* **Styling:** CSS, Tailwind CSS *(Optional but recommended)*
* **Data:** Free Movie Database API *(e.g., OMDB, TMDB)*

---

## 📋 Features & Requirements

###  1. Home Page

The Home Page serves as the landing page and must include the following sections:

####  Navbar
* Application logo or brand name.
* Navigation links.
* A prominent button/link to navigate to the **Movie Listing Page**.

####  Hero Banner
A visually attractive section to hook the user. It must include:
* A movie-related background image or gradient.
* Application title/heading.
* A short, engaging description.
* A Call-To-Action (CTA) button navigating to the **Movie Listing Page**.

**📐 UI Wireframe Example:**
```text
╭──────────────────────────────────────────────────────╮
│  🎬 MovieExplorer                        [ Movies ]  │
├──────────────────────────────────────────────────────┤
│                                                      │
│                 DISCOVER MOVIES                    │
│                                                      │
│        Explore and discover your favorite            │
│        movies from around the world.                 │
│                                                      │
│                 [   Explore Now ]                   │
│                                                      │
╰──────────────────────────────────────────────────────╯
```

####  Footer
* Application name.
* Copyright information (e.g., `© 2026 MovieExplorer`).
* Optional social media or GitHub links.

---

###  2. Movie Listing Page

Create a dedicated page where users can browse and search for movies.

####  Search Functionality
* Include a prominent search bar at the top of the page.
* Users must be able to search by **movie title**.
* The movie grid should dynamically update based on the search query.

** UI Wireframe Example:**
```text
╭──────────────────────────────────────────────────────╮
│  🔍 Search for a movie...                            │
╰──────────────────────────────────────────────────────╯
```

#### 🌐 API Integration & State Management
Fetch movie data from your chosen **Free Movie Database API**. You must gracefully handle the following states:

| State | Expected Behavior / UI |
| :--- | :--- |
|  **Loading** | Show a spinner or "Loading movies..." text. |
|  **Error** | Show "Something went wrong. Please try again." |
|  **Empty** | Show "No movies found." when search yields 0 results. |

#### 🎬 Movie Cards
Display movies using reusable Card components. Each card must include:
* Movie poster image.
* Movie title.
* Release year/date.
* Rating (e.g., ⭐ 8.5).
* A `See Details` button.

** UI Wireframe Example:**
```text
╭─────────────────────╮
│                     │
│       Poster        │
│                     │
├─────────────────────┤
│  Movie Title        │
│  ⭐ 8.5  •  📅 2024 │
│                     │
│  [ See Details ]    │
╰─────────────────────╯
```
>  **Requirement:** Cards must be displayed using a **responsive CSS Grid or Flexbox layout**.

---

### 🎞️ 3. Movie Details Modal

When a user clicks the **See Details** button, open a modal overlay displaying in-depth information about the selected movie.

**Modal Contents:**
* Movie backdrop image or large poster.
* Movie title.
* Overview / Plot description.
* Rating and Release date.
* Any additional relevant info from the API (e.g., Genre, Director).

** UI Wireframe Example:**
```text
╭──────────────────────────────────────────────╮
│                                      [ ✕ ]   │
├──────────────────────────────────────────────┤
│                                              │
│               MOVIE BACKDROP               │
│                                              │
├──────────────────────────────────────────────┤
│  Movie Title                                 │
│  ⭐ Rating: 8.5   |   📅 Release: 2024       │
│                                              │
│  Overview:                                │
│  Movie description goes here...              │
│                                              │
│                              [ ❌ Close ]    │
╰──────────────────────────────────────────────╯
```

**Interaction Requirements:**
* Must be closable via the `✕` (Close) button.
* *Optional:* Closable by clicking outside the modal (on the backdrop).

---

## 📱 Responsive Design & UX

The application must be fully responsive and provide a seamless experience across all devices:
*  **Mobile:** Single column layout, stacked elements, touch-friendly buttons.
*  **Tablet:** 2-3 column grid for movie cards.
*  **Desktop:** 3-4+ column grid for movie cards, optimized spacing.

---

## 📌 Submission Guidelines

Students must submit the following via the designated submission portal:

1.  **GitHub Repository Link** *(Ensure it is public and includes a `README.md`)*.
2.  **Live Deployment Link** *(e.g., Vercel, Netlify, GitHub Pages)*.

> ⚠️ **Note:** Ensure your `.env` files are ignored in Git and your API keys are not exposed in the public repository.

---

## 📊 Grading Rubric

| Criteria | Description | Marks |
| :--- | :--- | :---: |
|  **Home Page** | Navbar, Hero Banner & Footer implementation | **10** |
|  **Listing & Search** | Movie Listing Page & Search functionality | **12** |
|  **API & States** | API Integration, Loading, Error & Empty states | **10** |
|  **Cards & Layout** | Reusable Movie Cards & Responsive Grid | **8** |
|  **Details Modal** | Modal UI, Data display & Close interactions | **12** |
|  **Responsiveness** | Mobile/Tablet/Desktop adaptability & Overall UI | **5** |
|  **Code Quality** | Component structure, clean code, and best practices | **3** |
| | | |
| ** TOTAL** | | **60** |
