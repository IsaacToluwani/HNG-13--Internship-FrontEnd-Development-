# Stage 1: Multi-Page Profile Project — Contact & About Pages

This project builds upon the **Stage 0 Profile Card** task, extending it into a **multi-page application** with two new pages:
- A **Contact Us** page featuring form validation and accessibility best practices.
- An **About Me** page with reflective, semantic content.

Each page maintains semantic HTML structure, full accessibility, responsiveness, and the required `data-testid` attributes for testing.

---

## 📁 Project Structure

```
project-root/
│
├── index.html            # Profile Card (Stage 0)
├── contact.html          # Contact Us Page (Stage 1)
├── about.html            # About Me Page (Stage 1)
│
├── css/
│   └── styles.css        # Global styles for all pages
│
├── js/
│   └── main.js           # JavaScript for form validation
│
└── README.txt            # Project documentation
```

---

## 🧠 Project Overview

### 1. Contact Us Page

**Purpose:**  
Collect user messages with client-side validation and accessible form design.

**Required Fields & Test IDs:**
- Full name — `data-testid="test-contact-name"`
- Email — `data-testid="test-contact-email"`
- Subject — `data-testid="test-contact-subject"`
- Message — `data-testid="test-contact-message"`
- Submit button — `data-testid="test-contact-submit"`
- Error messages — `data-testid="test-contact-error-<field>"`
- Success message — `data-testid="test-contact-success"`

**Validation Rules:**
- All fields are required.  
- Email must be in a valid format (e.g., `name@example.com`).  
- Message must be at least **10 characters**.  
- On success, show a confirmation message dynamically.

**Accessibility Requirements:**
- Each input field must have a `<label>` linked with `for` and `id`.  
- Error messages are tied to inputs via `aria-describedby`.  
- Form is fully keyboard-accessible and responsive across devices.

---

### 2. About Me Page

**Purpose:**  
Share personal reflections, goals, and growth insights from this program.

**Required Sections & Test IDs:**
- Bio — `data-testid="test-about-bio"`
- Goals in this program — `data-testid="test-about-goals"`
- Areas of low confidence — `data-testid="test-about-confidence"`
- Note to future self — `data-testid="test-about-future-note"`
- Extra thoughts — `data-testid="test-about-extra"`

**Semantic Structure:**
```html
<main data-testid="test-about-page">
  <section data-testid="test-about-bio">...</section>
  <section data-testid="test-about-goals">...</section>
  <section data-testid="test-about-confidence">...</section>
  <section data-testid="test-about-future-note">...</section>
  <section data-testid="test-about-extra">...</section>
</main>
```

Each section includes headings (`<h2>`, `<h3>`) and paragraphs for clarity and structure.

---

## 🎨 Responsiveness & Layout

- **Mobile:** Stack sections vertically, full-width inputs and content.
- **Tablet/Desktop:** Two-column layout for better visual balance.
- Use **Flexbox** or **CSS Grid** for layout.
- Maintain consistent color palette and typography from Stage 0.

Reference:  
[CSS-Tricks – Media Queries for Standard Devices](https://css-tricks.com/snippets/css/media-queries-for-standard-devices/)

---

## ♿ Accessibility Highlights

- Semantic elements (`<main>`, `<section>`, `<header>`, `<label>`, etc.)
- Accessible form structure with ARIA attributes.
- Keyboard navigable links and buttons.
- Visible focus states on interactive elements.
- All images have descriptive `alt` text.

---

## 🧩 Tech Stack

- **HTML5** — Semantic and accessible structure  
- **CSS3** — Responsive design with Flexbox and Grid  
- **JavaScript (Vanilla JS)** — Form validation and interactive behavior  

---

## 🧪 Testing & Data Test IDs

Automated tests target specific elements using `data-testid` attributes.  
Ensure all elements include **exactly matching** IDs as listed in this document.

Example:
```html
<input id="email" name="email" data-testid="test-contact-email" required>
<span id="emailError" data-testid="test-contact-error-email"></span>
```

---

## 🚀 Deployment

Hosted on **Netlify** / **GitHub Pages** for easy public access.

### Live Demo:
👉 [Your Live Site URL Here]

### GitHub Repository:
👉 [Your GitHub Repo Link Here]

---

## ⚙️ How to Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/momo/stage1-multipage-profile.git
   ```
2. Navigate to the project folder:
   ```bash
   cd stage1-multipage-profile
   ```
3. Open `index.html` in your browser.

---

## 🕓 Submission Details

- **Submission Form:** [https://forms.gle/J65RPCVspzJJDGNP7](https://forms.gle/J65RPCVspzJJDGNP7)  
- **Deadline:** **22nd October 2025, 11:59 PM WAT (GMT +1)**  
- **Deliverables:**
  - Live URL
  - GitHub repo link with README and instructions

---

## 📚 References

- [MDN: HTML – A Good Basis for Accessibility](https://developer.mozilla.org/en-US/docs/Learn/Accessibility/HTML)  
- [MDN: Client-side Form Validation](https://developer.mozilla.org/en-US/docs/Learn/Forms/Form_validation)  
- [W3C WAI: Accessible Forms Tutorial](https://www.w3.org/WAI/tutorials/forms/)  
- [CSS-Tricks: Responsive Media Queries](https://css-tricks.com/snippets/css/media-queries-for-standard-devices/)

---

### 🧑‍💻 Author
**Name:** Momo  
**Email:** [Your Contact Email]  
**GitHub:** [https://github.com/momo](https://github.com/momo)
