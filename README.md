# 🏗️ SSA PROJECTS PVT. LTD.

### Construction • Infrastructure • Engineering • Development

<p align="center">
  <img src="logo.jpeg" alt="SSA Projects Pvt. Ltd." width="110">
</p>

<p align="center">
  <strong>Engineering Excellence. Built to Perform.</strong>
</p>

<p align="center">
  A modern, responsive and performance-focused corporate website
  for <strong>SSA Projects Pvt. Ltd.</strong>
</p>

<p align="center">

  <a href="https://miles-morales-rgb.github.io/ssa-projects/">
    <img src="https://img.shields.io/badge/Live%20Website-Visit%20Site-d4af37?style=for-the-badge" alt="Live Website">
  </a>

  <img src="https://img.shields.io/badge/HTML5-Static%20Website-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">

  <img src="https://img.shields.io/badge/CSS3-Responsive-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3">

  <img src="https://img.shields.io/badge/JavaScript-Vanilla-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript">

  <img src="https://img.shields.io/badge/GitHub%20Pages-Deployed-222222?style=for-the-badge&logo=github" alt="GitHub Pages">

</p>

---

## 🌐 Live Website

> **SSA Projects Pvt. Ltd. — Official Website**

### [Visit Website →](https://miles-morales-rgb.github.io/ssa-projects/)

---

## ✨ Overview

**SSA Projects Pvt. Ltd.** is a modern static corporate website designed to showcase the company's expertise, projects, team and business capabilities.

The website focuses on:

- 🏗️ Construction
- 🏢 Infrastructure
- ⚙️ Engineering
- 🏨 Luxury Hospitality
- 📐 Project Management
- 🌐 Development Projects
- 📊 Corporate Portfolio

The frontend is completely static and optimized for fast loading, responsive layouts and easy content management.

---

# 🚀 Features

### 🎨 Modern UI

- Premium dark corporate design
- Responsive layout
- Smooth animations
- Interactive project cards
- Modern navigation
- Mobile-friendly interface
- Glass-style UI elements
- Corporate gold accent design

### 📁 Dynamic Projects

Project information is loaded from:

```text
projects.json
```

Projects can contain:

```json
{
  "title": "Project Name",
  "category": "Hospitality",
  "location": "India",
  "shortDescription": "Short project description.",
  "description": "Detailed project description.",
  "imageUrl": "images/projects/project.jpg",
  "featured": true,
  "displayOrder": 1
}
```

The website automatically reads the JSON data and generates the project cards.

---

# 👥 Team Management

Team information is loaded dynamically from:

```text
team.json
```

Example:

```json
{
  "name": "Team Member",
  "role": "Project Director",
  "imageUrl": "images/team/member.jpg",
  "quote": "Building excellence through execution.",
  "displayOrder": 1
}
```

Team members are automatically sorted using:

```text
displayOrder
```

---

# ⚡ Performance

Performance is an important part of the website architecture.

### Initial Rendering

The website first loads:

```text
HTML
 ↓
CSS
 ↓
Main UI
```

Project and team data are then requested asynchronously:

```text
             ┌── projects.json
Website ─────┤
             └── team.json
```

Both JSON files are fetched in parallel.

### Image Optimization

Project and team images use:

```html
loading="lazy"
decoding="async"
```

This prevents unnecessary images from blocking the initial page load.

### Hero Video

The large hero video is intentionally delayed so that the main website content can render first.

---

# 🔍 SEO

The website includes several SEO features:

- SEO-friendly `<title>`
- Meta description
- Canonical URL
- Search engine indexing directives
- Google Search Console verification
- Open Graph metadata
- Twitter/X metadata
- Organization structured data
- Website structured data
- Semantic HTML
- Image ALT attributes
- `robots.txt`
- `sitemap.xml`

### Sitemap

```text
https://miles-morales-rgb.github.io/ssa-projects/sitemap.xml
```

### Robots

```text
https://miles-morales-rgb.github.io/ssa-projects/robots.txt
```

---

# 📂 Project Structure

```text
ssa-projects/
│
├── index.html
│
├── projects.json
├── team.json
│
├── logo.jpeg
├── video.mp4
├── hero-poster.jpg
│
├── images/
│   │
│   ├── projects/
│   │   ├── project-01.jpg
│   │   ├── project-02.jpg
│   │   └── ...
│   │
│   └── team/
│       ├── member-01.jpg
│       ├── member-02.jpg
│       └── ...
│
├── robots.txt
├── sitemap.xml
│
├── server.js
│
└── README.md
```

---

# 🖼️ Image Management

### Project Images

Store project images inside:

```text
images/projects/
```

Example:

```text
images/projects/jw-marriott.jpg
```

Then reference the image in `projects.json`:

```json
"imageUrl": "images/projects/jw-marriott.jpg"
```

### Team Images

Store team images inside:

```text
images/team/
```

Example:

```text
images/team/director.jpg
```

Then reference:

```json
"imageUrl": "images/team/director.jpg"
```

---

# 🛠️ Local Development

You can run the website locally before publishing it.

### Requirements

- Node.js
- Modern web browser

### Start Server

Open a terminal inside the project folder:

```bash
node server.js
```

The website will be available at:

```text
http://localhost:8000
```

---

# ☁️ Deployment

The website is designed for **GitHub Pages**.

### Step 1 — Upload

Upload the website files to your GitHub repository.

### Step 2 — Enable GitHub Pages

Go to:

```text
Repository
→ Settings
→ Pages
```

Select your deployment branch and folder.

### Step 3 — Publish

GitHub Pages will automatically deploy the website.

Live website:

```text
https://miles-morales-rgb.github.io/ssa-projects/
```

---

# 🔄 Updating Content

The website content can be updated without modifying the main HTML layout.

## Add a Project

Open:

```text
projects.json
```

Add:

```json
{
  "title": "New Project",
  "category": "Commercial",
  "location": "India",
  "shortDescription": "Project overview.",
  "description": "Detailed project information.",
  "imageUrl": "images/projects/new-project.jpg",
  "featured": true,
  "displayOrder": 5
}
```

Commit the changes.

The website will automatically load the updated project data.

---

## Add a Team Member

Open:

```text
team.json
```

Add:

```json
{
  "name": "John Doe",
  "role": "Project Director",
  "imageUrl": "images/team/john-doe.jpg",
  "quote": "Building excellence through execution.",
  "displayOrder": 5
}
```

Commit the changes and GitHub Pages will publish the update.

---

# 🔐 Security

This website is a **public static frontend**.

Never store sensitive credentials in the repository.

### ❌ Never commit:

```text
Passwords
GitHub Personal Access Tokens
API Keys
Private Keys
Authentication Tokens
Database Credentials
Private Credentials
```

Anything published through GitHub Pages should be treated as publicly accessible.

---

# 📱 Responsive Design

The website is designed for:

| Device | Support |
|---|---|
| 🖥️ Desktop | ✅ |
| 💻 Laptop | ✅ |
| 📱 Mobile | ✅ |
| 📲 Tablet | ✅ |

---

# 📬 Contact

For business inquiries:

```text
info@ssaprojects.com
```

The website provides a contact interface that can create an email inquiry through the visitor's email client.

---

# 🏢 Company

## SSA Projects Pvt. Ltd.

**Construction • Infrastructure • Engineering • Development**

---

# 📜 License

This website and its associated content are proprietary to:

**SSA Projects Pvt. Ltd.**

The website design, branding, images, project information, source code and other proprietary content may not be reproduced, redistributed or used without appropriate authorization.

---

<p align="center">

### Built for SSA Projects Pvt. Ltd.

<strong>Engineering Excellence. Built to Perform.</strong>

<br><br>

<a href="https://miles-morales-rgb.github.io/ssa-projects/">
  Visit Official Website →
</a>

</p>
