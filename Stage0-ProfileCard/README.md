Profile Card Component
=======================

A small, accessible, and responsive Profile Card built with semantic HTML, modern CSS, and vanilla JavaScript. 
Every visible element includes a data-testid attribute for automated testing.

-----------------------------------
PROJECT OVERVIEW
-----------------------------------
This project implements a Profile Card that displays a user’s information such as name, bio, avatar, current time (in milliseconds), hobbies, dislikes, and social links.

It follows semantic HTML, accessibility best practices, and responsive design.

-----------------------------------
FEATURES
-----------------------------------
- Semantic HTML structure (article, header, section, figure, nav, etc.)
- Accessible markup with alt text and keyboard-focusable links
- Responsive design using Flexbox and media queries
- Displays current time in milliseconds using Date.now()
- Social links open safely in new tabs (target="_blank" + rel="noopener noreferrer")
- Includes all required data-testid attributes for automated testing
- Clean, maintainable CSS layout adaptable for all devices

-----------------------------------
FOLDER STRUCTURE
-----------------------------------
project/
│
├── index.html
├── style.css
├── script.js
└── README.txt

-----------------------------------
DATA TEST IDS
-----------------------------------
Profile card root container — test-profile-card
User name — test-user-name
Short biography — test-user-bio
Current time (milliseconds) — test-user-time
Avatar image — test-user-avatar
Social links container — test-user-social-links
Individual social link (optional) — test-user-social-<network>
Hobbies list — test-user-hobbies
Dislikes list — test-user-dislikes

-----------------------------------
EXAMPLE HTML STRUCTURE
-----------------------------------
<article data-testid="test-profile-card">
  <header>
    <h2 data-testid="test-user-name">Jane Doe</h2>
  </header>

  <figure>
    <img src="avatar.jpg" alt="Portrait of Jane Doe" data-testid="test-user-avatar" />
  </figure>

  <p data-testid="test-user-bio">
    Frontend developer passionate about accessibility and design systems.
  </p>

  <p data-testid="test-user-time" id="user-time"></p>

  <nav data-testid="test-user-social-links">
    <ul>
      <li><a href="https://twitter.com" target="_blank" rel="noopener noreferrer" data-testid="test-user-social-twitter">Twitter</a></li>
      <li><a href="https://github.com" target="_blank" rel="noopener noreferrer" data-testid="test-user-social-github">GitHub</a></li>
    </ul>
  </nav>

  <section data-testid="test-user-hobbies">
    <h3>Hobbies</h3>
    <ul>
      <li>Photography</li>
      <li>Cycling</li>
      <li>Cooking</li>
    </ul>
  </section>

  <section data-testid="test-user-dislikes">
    <h3>Dislikes</h3>
    <ul>
      <li>Procrastination</li>
      <li>Cold Coffee</li>
    </ul>
  </section>
</article>

-----------------------------------
JAVASCRIPT FUNCTIONALITY
-----------------------------------
Displays the current time in milliseconds using:

document.getElementById("user-time").textContent = Date.now();

Optionally, update dynamically with setInterval().

-----------------------------------
RESPONSIVENESS
-----------------------------------
- Uses Flexbox and media queries.
- Mobile: stacked vertically.
- Desktop: avatar left, text right.

-----------------------------------
ACCESSIBILITY
-----------------------------------
- All images include alt text.
- Links are keyboard-focusable with visible focus states.
- Semantic regions aid screen readers.
- Color contrast follows accessibility standards.

-----------------------------------
HOW TO RUN LOCALLY
-----------------------------------
1. Clone the repo:
   git clone https://github.com/yourusername/profile-card-component.git

2. Open folder:
   cd profile-card-component

3. Open index.html in your browser.

-----------------------------------
DEPLOYMENT
-----------------------------------
Can be deployed via:
- Netlify
- GitHub Pages
- Vercel

Example: https://yourusername.github.io/profile-card-component/

-----------------------------------
TESTING NOTES
-----------------------------------
- All elements have required data-testids.
- Time value matches Date.now() (within acceptable delta).
- Keyboard focus and accessibility can be verified with browser dev tools.

-----------------------------------
REFERENCES
-----------------------------------
HTML Semantics — https://developer.mozilla.org/en-US/docs/Web/HTML/Element
Accessible Images & Alt Text — https://developer.mozilla.org/en-US/docs/Web/Accessibility/Images
