# 📌 Bookmark Dashboard

A modern, minimal, and fully client-side **bookmark management web app** built using React (CDN) and TailwindCSS.

This app allows users to organize bookmarks into draggable columns, similar to a lightweight Trello-style interface — all without any backend.

---

## 🚀 Features

### 📂 Column-Based Organization

* Create multiple lists (columns)
* Each column holds bookmarks
* Auto-generated names (`Column 1`, `Column 2`, ...)

### ✏️ Editable Column Names

* Click on a column title to rename it inline

### 🗑️ Clean Delete UX

* Delete buttons (×) are hidden by default
* Appear only on hover for a clean interface

### 🔖 Bookmark Management

* Add bookmarks via modal popup
* Each bookmark includes:

  * Title
  * URL
  * Auto-fetched favicon

### 🔄 Drag & Drop (Full Support)

* Reorder bookmarks within a column
* Move bookmarks across columns
* Reorder entire columns horizontally

### 🎯 Visual Feedback

* Drop indicators for precise placement
* Hover-based UI interactions

### 💾 Persistent Storage

* Uses browser **localStorage**
* Data persists across reloads and sessions

---

## 🧠 Data Storage

All data is stored locally in the browser using:

```javascript
localStorage.setItem("columns", JSON.stringify(columns));
```

### Structure:

```json
[
  {
    "name": "Column 1",
    "links": [
      { "title": "Google", "url": "https://google.com" }
    ]
  }
]
```

---

## 🖥️ Tech Stack

* **React (CDN)** – UI logic
* **Tailwind CSS (CDN)** – Styling
* **Vanilla JavaScript** – Drag & Drop logic
* **localStorage** – Persistence layer

---

## 📦 How to Use

1. Open the HTML file in your browser
2. Create your first list
3. Add bookmarks using the "Add Bookmark" button
4. Drag to organize

---

## ⚠️ Limitations

* No backend → data is device/browser specific
* No sync across devices
* Clearing browser data will delete all bookmarks
* Drag & drop optimized for desktop (limited mobile support)

---

## 🔮 Future Improvements

* Multi-screen navigation system
* Export / Import bookmarks (JSON backup)
* Chrome Extension version
* Grid / icon view (like Chrome new tab)
* Mobile drag support
* Animations & transitions

---

## 💡 Inspiration

* Trello-style boards
* Modern bookmark managers
* Minimal dashboard interfaces

---

## 📁 File Reference

Your current implementation: 

---

## 🧑‍💻 Author

Built as a personal productivity tool and experimental UI project.

---

## ⭐ Notes

This project is intentionally **frontend-only** to keep it simple, fast, and portable.

It serves as a strong foundation for building:

* Bookmark tools
* Dashboards
* Productivity apps
* Chrome extensions

---
