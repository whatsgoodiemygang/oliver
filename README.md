<div align="center">

# 📚 Oliver
### Abingdon School Library System

*A single-page web app for pupils and staff — browse books, get AI reading recommendations, track challenges, and write reviews.*

[![Live App](https://img.shields.io/badge/Live%20App-DE048E?style=for-the-badge&logo=github&logoColor=white)](https://whatsgoodiemygang.github.io/oliver/)
[![GitHub Pages](https://img.shields.io/badge/Hosted%20on-GitHub%20Pages-222?style=for-the-badge&logo=github)](https://whatsgoodiemygang.github.io/oliver/)
[![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)](https://firebase.google.com)

</div>

---

## ✨ Features

| Feature | Description |
|---|---|
| 📖 **Book Catalogue** | Browse, search, and filter the full library with fuzzy search powered by Fuse.js |
| 🤖 **AI Research Chat** | Ask questions and get tailored reading suggestions powered by Claude AI |
| 🎭 **Mood Recommendations** | Tell the app how you're feeling — it'll find the perfect book |
| 🏆 **Reading Challenge** | Track progress against school-set reading challenges with visual milestones |
| ✍️ **Book Reviews** | Write and read community reviews with star ratings |
| 🔧 **Staff Admin Panel** | Librarians can manage the catalogue, reviews, and challenges |
| 🌙 **Dark Mode** | Full dark/light mode with system preference support |
| 🔐 **Google Auth** | Sign in with your `@abingdon.org.uk` account or school email |

---

## 🚀 How to Use

<details>
<summary><b>Signing In</b></summary>

Open the app and click **Sign In**. Use your `@abingdon.org.uk` Google account for one-click login, or enter your school email and password manually.

</details>

<details>
<summary><b>Browsing the Catalogue</b></summary>

Head to the **Catalogue** tab. Use the search bar to find books by title, author, or keyword. Filter by genre using the chips at the top. Click any book card to see full details, availability, and reviews.

</details>

<details>
<summary><b>AI Research Chat</b></summary>

Go to the **Research** tab and type your question or topic. The AI will suggest relevant books from the catalogue and provide reading guidance — great for homework, projects, or finding something new.

</details>

<details>
<summary><b>Mood Recommendations</b></summary>

Visit the **Discover** tab and select how you're feeling. The app will surface a curated selection of books that match your vibe — adventurous, calm, curious, or anything in between.

</details>

<details>
<summary><b>Reading Challenge</b></summary>

The **Challenge** tab shows your current reading challenge. Log finished books, track your progress bar, and earn milestones as you go. Challenges are set by library staff.

</details>

<details>
<summary><b>Writing a Review</b></summary>

Open any book's detail page from the catalogue and scroll to the **Reviews** section. Give it a star rating, write your thoughts, and submit. Your review appears instantly for other pupils.

</details>

<details>
<summary><b>Staff Admin Panel</b></summary>

Staff accounts automatically see the **Admin** tab after signing in. From here you can:
- Add, edit, or remove books from the catalogue
- Moderate and delete pupil reviews
- Set and update the reading challenge
- View pupil progress

</details>

---

## 🛠️ Setup & Deployment

> The app requires no server — it's a single HTML file hosted on GitHub Pages.

**1. Fork or clone the repo**
```
git clone https://github.com/whatsgoodiemygang/Oliver.git
```

**2. Configure Firebase**

Create a project at [console.firebase.google.com](https://console.firebase.google.com), enable Authentication (Google + Email/Password) and Firestore, then paste your config into the app's Firebase config block.

**3. Enable GitHub Pages**

Go to **Settings → Pages**, set the branch to `main`, and save. GitHub publishes your site automatically.

**4. Add your domain to Firebase**

In Firebase Console go to **Authentication → Settings → Authorised domains** and add your GitHub Pages domain (e.g. `whatsgoodiemygang.github.io`).

**5. Done** ✅

Visit your GitHub Pages URL and sign in. No server required.

---

## 🗂️ Repo Structure

```
/
├── index.html                    ← the full app (all CSS + JS inline)
├── firebase-app-compat.js        ← Firebase core SDK
├── firebase-auth-compat.js       ← Firebase Authentication
├── firebase-firestore-compat.js  ← Cloud Firestore
├── firebase-analytics-compat.js  ← Firebase Analytics
└── fuse_min.js                   ← Fuzzy search library
```

---

## 🧱 Tech Stack

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)
![Fuse.js](https://img.shields.io/badge/Fuse.js-000000?style=flat-square)
![Claude AI](https://img.shields.io/badge/Claude%20AI-DE048E?style=flat-square)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-222?style=flat-square&logo=github)

A deliberately simple stack — no build tools, no bundler, no framework. Just one HTML file that works anywhere.

---

## 📖 Wiki

For a full breakdown of how this app was built — from the original concept through to solving the Smoothwall content filter issue — see the [**project wiki**](../../wiki).

---

<div align="center">
  <sub>Built with ♥ for Abingdon School · <a href="https://whatsgoodiemygang.github.io/oliver/">whatsgoodiemygang.github.io/oliver</a></sub>
</div>
