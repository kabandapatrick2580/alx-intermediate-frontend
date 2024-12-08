# CSS Grid and Flexbox: Creating Complex, Responsive Layouts using Tailwind

## Overview
**Level:** Novice  
**Weight:** 1  
**Project Start:** December 1, 2024, 11:00 PM  
**Project End:** December 8, 2024, 11:00 PM  

This project focuses on hands-on exploration of Tailwind CSS to build responsive and aesthetically pleasing web layouts. Tasks are designed to introduce advanced Tailwind concepts, enabling learners to master utility-first CSS for modern web development. By progressing through tasks, learners will gain proficiency in responsive design principles, CSS Grid, and Flexbox, while enhancing their ability to create visually appealing and professional-grade web components.

## Learning Objectives
- **Master Tailwind CSS Configuration:** Learn installation and configuration for seamless integration.
- **Build Responsive Layouts:** Implement complex, responsive designs using Tailwind's utility classes.
- **Combine CSS Grid and Flexbox:** Develop advanced page structures by leveraging both techniques.
- **Design Aesthetically Pleasing Components:** Use Tailwind utilities to create visually appealing designs with gradients, spacing, and colors.
- **Optimize for Professional Development:** Adhere to best practices for structuring, coding, and managing CSS frameworks.

## Requirements
- Node.js installed on the local machine ([Download Node.js](https://nodejs.org)).
- Basic knowledge of HTML, CSS, and JavaScript.
- Familiarity with a code editor (e.g., VSCode) and browser developer tools.
- GitHub account for repository management.
- Tailwind CSS installed via npm or CDN.
- Modern browser to render and test designs.
- Internet connection for accessing Tailwind’s documentation and CDN links.

## Tasks

### 0. Setting Up and Installing Tailwind CSS with Configuration
**Objective:** Set up and install Tailwind CSS.  

**Instructions:**
1. Install Tailwind CSS.
2. Create a `tailwind.config.js` file with the following code:
   ```js
   /** @type {import('tailwindcss').Config} */
   module.exports = {
     content: ["./src/**/*.{html,js}"],
     theme: {
       extend: {},
     },
     plugins: [],
   };
   ```
3. Create a `src` directory and an `input.css` file inside it with:
   ```css
   @tailwind base;
   @tailwind components;
   @tailwind utilities;
   ```
4. Run the Tailwind CLI tool to build your CSS output:
   ```bash
   npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
   ```

**Repo:**  
- GitHub repository: `alx-intermediate-frontend`
- Directory: `0x02-tailwind-css`
- Files: `src/input.css`, `src/output.css`, `tailwind.config.js`

---

### 1. Creating a Responsive CSS Grid Layout with Tailwind CSS
**Objective:** Leverage Tailwind to create a basic CSS grid layout.

**Instructions:**
1. Create `1-index.html` with the following structure:
   ```html
   <main class="grid grid-cols-3 gap-4">
     <div class="bg-blue-200 p-4">Column 1</div>
     <div class="bg-blue-300 p-4">Column 2</div>
     <div class="bg-blue-400 p-4">Column 3</div>
   </main>
   ```
2. Make the layout responsive by adjusting the grid on smaller screens in `input.css`:
   ```css
   @media (max-width: 768px) {
     main {
       grid-template-columns: 1fr;
     }
   }
   ```

**Repo:**  
- GitHub repository: `alx-intermediate-frontend`
- Directory: `0x02-tailwind-css`
- File: `1-index.html`

---

### 2. Building a Complex Page Layout with Nested CSS Grids Using Tailwind CSS
**Objective:** Implement a complex layout using nested grids.

**Instructions:**
1. Create `2-index.html` with:
   ```html
   <main class="grid grid-cols-2 gap-4">
     <div class="grid grid-cols-2 p-4 gap-2 bg-blue-200">
       <div class="bg-blue-400 p-2">Nested 1</div>
       <div class="bg-blue-500 p-2">Nested 2</div>
     </div>
     <div class="grid grid-cols-2 p-4 gap-2 bg-red-200">
       <div class="bg-red-400 p-2">Nested 3</div>
       <div class="bg-red-500 p-2">Nested 4</div>
     </div>
   </main>
   ```

**Repo:**  
- GitHub repository: `alx-intermediate-frontend`
- Directory: `0x02-tailwind-css`
- File: `2-index.html`

---

### 3. Flexbox Basics - Build a Simple Navigation Bar
**Objective:** Create a horizontal navigation bar using Flexbox.

**Instructions:**
1. Create `3-nav_index.html` with a `nav` tag:
   ```html
   <nav class="flex space-x-5 justify-center bg-gray-300 text-white p-4">
     <a href="#" class="px-2 text-xl hover:bg-gray-500 p-2 rounded-lg">Home</a>
     <a href="#" class="px-2 text-xl hover:bg-gray-500 p-2 rounded-lg">About</a>
     <a href="#" class="px-2 text-xl hover:bg-gray-500 p-2 rounded-lg">Services</a>
     <a href="#" class="px-2 text-xl hover:bg-gray-500 p-2 rounded-lg">Contact</a>
   </nav>
   ```

**Repo:**  
- GitHub repository: `alx-intermediate-frontend`
- Directory: `0x02-tailwind-css`
- File: `3-nav_index.html`

---

### 4. Create a Responsive Flexbox Layout with Tailwind
**Objective:** Build a responsive layout using Flexbox.

**Instructions:**
1. Create `4-flexbox_index.html` with:
   ```html
   <main class="flex">
     <aside class="w-1/3 bg-gray-300 p-4">Sidebar</aside>
     <section class="w-2/3 bg-gray-500 p-4">Content Section</section>
   </main>
   ```

**Repo:**  
- GitHub repository: `alx-intermediate-frontend`
- Directory: `0x02-tailwind-css`
- File: `4-flexbox_index.html`

---

### 5. Combine CSS Grid and Flexbox for a Multi-Section Layout
**Objective:** Create a responsive layout using both CSS Grid and Flexbox.

**Instructions:**
1. Create `5-gridflex_index.html` with:
   ```html
   <main class="grid grid-cols-1 lg:grid-cols-3 gap-4 mt-4 min-h-screen">
     <section class="lg:col-span-2 flex">
       <div class="w-1/2 bg-red-200 p-4">Flexbox Item 1</div>
       <div class="w-1/2 bg-red-400 p-4">Flexbox Item 2</div>
     </section>
     <aside class="bg-green-200 p-4">Sidebar</aside>
   </main>
   ```

**Repo:**  
- GitHub repository: `alx-intermediate-frontend`
- Directory: `0x02-tailwind-css`
- File: `5-gridflex_index.html`

---

### 6. Build a Responsive Image Gallery Using CSS Grid
**Objective:** Expand the previous layout by adding a responsive image gallery.

**Instructions:**
1. Use the layout from Task 5 and add a 3-column image gallery below the content.
2. Adjust the gallery to display one image per row on smaller screens.

**Repo:**  
- GitHub repository: `alx-intermediate-frontend`
- Directory: `0x02-tailwind-css`
- File: `6-imageGallery.html`

---

### 7. Manual Review
Request manual QA review upon completion. An auto review will be launched at the deadline.

**Repo:**  
- GitHub repository: `alx-intermediate-frontend`
- Directory: `0x02-tailwind-css`

