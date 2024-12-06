# Semantic HTML Project

## About the Project
This project focuses on building a solid foundation in **Semantic HTML** while emphasizing accessibility, SEO optimization, and the implementation of **ARIA roles** for enhanced usability. Through incremental tasks, learners will structure and enhance a web page to make it visually organized, optimized for screen readers, and search engines. By the end of the project, learners will understand the importance of semantic elements and accessibility features in modern web development.

## Learning Objectives
- **Master Semantic HTML**: Learn to structure web pages using semantic elements such as `<header>`, `<main>`, `<article>`, `<section>`, and `<footer>` for better content organization and accessibility.
- **Optimize for SEO**: Understand how to improve the visibility of your webpage through appropriate usage of meta tags and proper document structure.
- **Enhance Accessibility**: Implement ARIA roles and attributes to make web forms and content more accessible to users with disabilities.
- **Understand Form Design Best Practices**: Learn to create accessible and user-friendly forms using modern HTML techniques.
- **Adopt Incremental Development**: Practice progressive enhancement by building upon the foundation of each previous task.

## Requirements
- A working understanding of HTML5.
- Familiarity with semantic HTML elements and their purpose.
- Basic knowledge of SEO and its importance in web development.
- Awareness of web accessibility standards, including ARIA roles and attributes.

---

## Tasks

### 0. Creating a Structured HTML Document Using Semantic Elements
**Objective**: Practice structuring a simple HTML document using semantic elements.

Create your first HTML file `0-index.html` with:
- Inside the `<html>` tag, create the `<head>` and `<body>` tags (empty) in this order.
- Inside the `<body>` tag:
  - Add a `<header>` that contains a `<nav>` with at least three links.
  - Create a `<main>` section that contains an `<article>`. Inside the `<article>`:
    - Add an `<h1>` tag for the title.
    - Add a `<section>` for the content.
  - Add a `<footer>` with some copyright information: `© Copyright`.

**Note**: Remember the structure of an HTML file starts with a `<!DOCTYPE html>` declaration.

**Repo**:  
- GitHub repository: `alx-intermediate-frontend`  
- Directory: `0x00-semantic_html`  
- File: `0-index.html`

---

### 1. Enhancing HTML Document with Meta Tags and Title for SEO and Accessibility
**Objective**: Enhance the structure of the HTML document by adding meta tags for improved SEO, accessibility, and responsiveness, while properly defining the document’s character set and title.

- Copy the content of `0-index.html` into `1-index.html`.  
- Inside the `<head>` tag:
  - Add a `<meta>` tag with the `charset` attribute set to `utf-8`.
  - Add four more meta tags with the following:
    1. `name="description" content="A blog post about semantic HTML and accessibility practices"`
    2. `name="keywords" content="HTML, Semantic, Accessibility, Blog, SEO"`
    3. `name="author" content="<your-name>"`
    4. `name="viewport" content="width=device-width, initial-scale=1.0"`
  - Add a `<title>` tag with the text: `Semantic HTML Blog Post`.

**Repo**:  
- GitHub repository: `alx-intermediate-frontend`  
- Directory: `0x00-semantic_html`  
- File: `1-index.html`

---

### 2. Creating a Blog Post Layout Using Semantic HTML Elements
**Objective**: Apply semantic elements to create a blog post layout.

- Copy the content of `1-index.html` into `2-index.html`.
- Inside the `<header>` tag:
  - Add an `<h1>` tag with the content `My Blog`.
  - Add a `<nav>` tag. Inside it, create a `<ul>` tag with three `<li>` tags referencing the following links:
    - `Home`
    - `About`
    - `Contact`
- Inside the `<main>` tag:
  - Inside the `<article>` tag:
    - Add a `<header>` tag with an `<h2>` tag: `Understanding Semantic HTML`.
    - Add a `<p>` tag: `Published on <time datetime="2024-09-10">September 10</time>`.
    - Inside the `<section>` tag:
      - Add an `<h3>` tag: `Introduction`.
      - Add a `<p>` tag: `Semantic HTML helps improve the accessibility and SEO of your website. In this post, we’ll explore its benefits and how to implement it.`

**Repo**:  
- GitHub repository: `alx-intermediate-frontend`  
- Directory: `0x00-semantic_html`  
- File: `2-index.html`

---

### 3. Enhancing Form Accessibility with ARIA Roles and Attributes
**Objective**: Implement ARIA roles to improve accessibility in a form.

- Copy the content of `2-index.html` into `3-index.html`.
- Inside the `<main>` element, add a new `<section>` tag.
- Inside the `<section>` tag:
  - Add a `<form>` tag with the following attributes:
    - `action="#"`
    - `method="POST"`
    - `aria-labelledby="form-title"`
    - `role="form"`
  - Inside the `<form>`:
    - Add a `<div>` with:
      - A `<label>` tag with `for="name"`.
      - An `<input>` tag with:
        - `type="text"`
        - `id="name"`
        - `name="name"`
        - `aria-required="true"`
    - Add another `<div>` with:
      - A `<label>` tag with `for="email"`.
      - An `<input>` tag with:
        - `type="email"`
        - `id="email"`
        - `name="email"`
        - `aria-required="true"`
    - Add another `<div>` with:
      - A `<button>` tag with:
        - `type="submit"`
        - `aria-label="Submit the form"`
    - Add a `<div>` tag with:
      - `aria-live="polite"`
      - `role="alert"`

**Repo**:  
- GitHub repository: `alx-intermediate-frontend`  
- Directory: `0x00-semantic_html`  
- File: `3-index.html`

---

### 4. Manual Review
**Repo**:  
- GitHub repository: `alx-intermediate-frontend`  
- Directory: `0x00-semantic_html`
