## Student Registration System

A simple, responsive Student Management web app built with HTML, CSS, and JavaScript. It allows you to register students, list them in a table, and edit or delete entries. Data is persisted in the browser using `localStorage`.

### Features
- **Register students** with name, ID, email, and contact number
- **Client-side validation** for name and contact number
- **Edit/Delete** existing student entries
- **Persistent storage** via `localStorage`
- **Responsive UI** for desktop, tablet, and mobile

### Tech Stack
- **HTML5** for structure (`index.html`)
- **CSS3** for styling and responsiveness (`style.css`)
- **JavaScript (ES6)** for logic and storage (`script.js`)

### Getting Started
1. Download or clone this repository.
2. Open `index.html` in any modern web browser (Chrome, Edge, Firefox, Safari).
   - Optional: Use a local dev server (e.g., VS Code “Live Server”) for a better experience.

### Usage
1. Fill in the form fields:
   - Student Name
   - Student ID
   - Email ID
   - Contact No
2. Click "Register Student" to add the entry.
3. Use the **Edit** button to load a row back into the form, make changes, then submit to save.
4. Use the **Delete** button to remove a student.

### Validation Rules
- **Name**: Letters and spaces only (`^[A-Za-z ]+$`)
- **Contact No**: Exactly 10 digits (`^\d{10}$`)

### Data Persistence
- Entries are stored in `localStorage` under the key `students` as a JSON array.
- To reset the app data, open DevTools and run: `localStorage.removeItem('students')` (or clear all site data).

### Project Structure
```
Student management System/
  index.html   # App markup & table layout
  style.css    # Styles, colors, and responsive rules
  script.js    # Logic: CRUD, validation, and localStorage
```

### Notes
- The marquee in the header is for a simple moving message effect.
- The ID and Contact inputs use `type="number"`; leading zeros (if any) may be dropped by some browsers.

### Roadmap / Ideas
- Add search and sort for the student table
- Validate email format more strictly and handle duplicates
- Export/Import data (CSV/JSON)
- Pagination for large lists

### License
This project is available under the MIT License. You may use, copy, modify, and distribute it as permitted by the license terms.