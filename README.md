Advanced Single-File Portfolio
This repository contains the source code for a modern, interactive, single-file personal portfolio website. It is built with vanilla HTML, CSS, and JavaScript and features numerous advanced animations and effects, all contained within a single index.html file for easy deployment.

A screenshot of the live portfolio website.

🚀 Live Demo
You can see a live version of this portfolio here: [Link to your live site] (https://xgolsawx.github.io/Portfolio_Sample1/)

✨ Key Features
This project is more than just a static page; it's a demonstration of modern web capabilities:

Single-File Architecture: All HTML, CSS, and JavaScript are in one index.html file. No build-step, no dependencies.

Interactive Particle Background: A performant, lightweight <canvas> particle animation that runs in the background.

3D Tilt Effects:

The main profile card has a 3D parallax tilt effect on mouse move.

Project cards feature a 3D tilt and a dynamic "shine" effect on hover.

Draggable Project Carousel: A touch-friendly, mouse-draggable horizontal carousel to showcase projects.

Project Modal & Code Viewer: Clicking a project opens a modal with details and a mock code snippet (with a 'Copy to Clipboard' button).

Animated Skills: SVG radial progress bars that animate into view when the user scrolls to the "Skills" section, triggered by an IntersectionObserver.

Typed Headline: An auto-typing effect for the hero section's subheading.

Theme Toggle: A functional (and system-preference-aware) light/dark mode toggle, built with CSS variables.

Custom Cursor: A smooth, custom-animated cursor dot and ring that reacts to interactive elements.

Responsive Design: Fully responsive layout for mobile, tablet, and desktop devices.

Accessibility: Includes ARIA attributes, keyboard navigation support, and smooth scrolling for anchors.

🛠️ How to Use
Since this is a single-file project, setup is incredibly simple.

Clone the repository:

Bash

git clone https://github.com/your-username/your-repo-name.git
Open the file: Navigate to the cloned directory and open the index.html file in your web browser. That's it!

🎨 Customization
All content can be edited directly in the index.html file.

Colors & Theme: Change the entire color palette by editing the CSS variables in the :root { ... } block at the top of the <style> section.

Personal Information:

Header/Logo: Update the HTML in the <header> block.

Profile Card: Update the HTML in the <aside class="profile-card"> block.

Typed Words: In the <script> section (near the bottom), find the typedWords() function and modify the words array:

JavaScript

const words = ["new word 1", "new word 2", "new word 3"];
Skills:

Update the .skill-card HTML elements with your skills.

Update the values array in the skillAnimate() function to match the percentages for your skills:

JavaScript

const values = [90, 86, 78]; // Update these percentages
Projects:

Add or edit the <article class="project-card"> elements in the "PROJECTS" section.

The modal window pulls its content from the data- attributes on each card (data-title, data-desc, data-img, data-tags).

Timeline:

Edit the .timeline-item elements in the "TIMELINE" section.

Contact Form:

The contact form is currently a mock and only simulates a send.

To make it functional, find the contactForm() function and integrate a service like EmailJS or your own backend API. The code includes a commented-out example for EmailJS.

💻 Tech Stack
HTML5

CSS3 (with CSS Variables, Flexbox, Grid, and backdrop-filter)

Vanilla JavaScript (ES6+) (No libraries or frameworks)

📜 License
This project is licensed under the MIT License. Feel free to use it as a template for your own portfolio.
