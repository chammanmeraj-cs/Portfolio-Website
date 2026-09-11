# Personal Web Portfolio (Emerald Obsidian Theme)

## Project Title
Emerald Obsidian – Interactive Personal Portfolio

## Project Objective
To design and deploy a responsive, high-contrast, and accessible personal web portfolio that showcases front-end development skills, featured projects, and provides a direct communication line for potential opportunities.

## Project Overview
This project is a modern, single-page web portfolio built from scratch. It features an "Emerald Obsidian" visual identity, utilizing glassmorphism cards, structured section layouts, dynamic category filtering for showcase items, and standard user input validation for contact queries.

## Technologies Used
* **Frontend:** HTML5, CSS3 (Flexbox, CSS Grid, Custom Variables)
* **Scripting:** JavaScript (Vanilla ES6)
* **Icons & Fonts:** FontAwesome 6.4, Google Fonts
* **Version Control & Hosting:** Git, GitHub, GitHub Pages

## Main Features
* **Custom Emerald Obsidian Theme:** High-contrast aesthetic with custom CSS variables and glassmorphism styling.
* **Dynamic Category Filtering:** Interactive filtering using custom `data-*` attributes for seamless sorting between JS Apps and Tools.
* **Client-Side Form Validation:** Real-time JavaScript validation for input fields (Name, Email format, Message content).
* **Fully Responsive Design:** Dynamic grid layouts adapted for mobile, tablet, and desktop viewports.

## Website Screenshots
![Portfolio Preview](Assets/Screenshot%202026-09-11%20163336.png)

## Repository & Deployment Links
* **GitHub Repository Link:** [https://github.com/chammanmeraj-cs/Portfolio-Website](https://github.com/chammanmeraj-cs/Portfolio-Website)
* **Live Website Link:** [https://chammanmeraj-cs.github.io/Portfolio-Website/](https://chammanmeraj-cs.github.io/Portfolio-Website/)

## Challenges Faced
1. **Filter Attribute Mismatch:** Project buttons failed to toggle showcase cards due to mismatched string values between HTML `data-filter` attributes and JavaScript queries.
2. **Local Session Conflict:** Social icon redirection (LinkedIn) opened incorrect browser user profiles due to active local session cookies across secondary browsers.
3. **Redundant Logic Errors:** Unlinked dark mode JavaScript functions caused runtime script execution errors after transitioning to a fixed visual theme.

## Solutions Implemented
1. **Attribute Normalization:** Synchronized all filtering categories (`js-app`, `tool`) and applied strict `.trim().toLowerCase()` string handling in JavaScript.
2. **URL & Environment Isolation:** Enforced full URL schemes with `target="_blank"` and `rel="noopener noreferrer"` attributes, validating behavior via incognito browser sessions.
3. **Script Refactoring:** Wrapped all DOM operations inside a single `DOMContentLoaded` listener and purged unmapped theme toggle events.

## Key Learnings
* Mastering DOM manipulation and layout state management with pure Vanilla JavaScript.
* Structuring clean CSS using dynamic variables for cohesive color palette maintenance.
* Utilizing Git workflows effectively for repository synchronization and version tracking.

## Future Improvements
* Integrating server-side contact form handling via Formspree or EmailJS.
* Adding smooth scroll-spy navigation for active section highlighting.
