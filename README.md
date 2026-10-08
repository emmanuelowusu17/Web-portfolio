# Emmanuel Owusu – Web Portfolio

My personal portfolio website, built as part of a Web Development Fundamentals course at MSU Denver. It introduces who I am, the skills I'm learning, and the projects I'm working on as a Computer Science student.

## Built With

- **HTML5** – page structure
- **CSS3** – custom styling (`style.css`)
- **Bootstrap 5.3** – responsive grid, cards, buttons, and navbar
- **jQuery** – loads the shared navigation bar into each page
- **Git & GitHub** – version control

## Pages

| Page | Description |
|------|-------------|
| **Home** (`index.html`) | Intro section with my photo and short bio, a skills section, and featured projects |
| **Projects** (`projects.html`) | Details about each project I'm working on |
| **About** (`about.html`) | My background, my CS journey, what I'm currently learning, and my career goals |

## Project Structure

```
Web-portfolio/
├── index.html       # Home page
├── projects.html    # Projects page
├── about.html       # About page
├── nav.html         # Shared navigation bar, loaded into every page
├── style.css        # Custom styles
├── images/          # Profile photo, skill logos, project images, background
└── README.md
```

## How It Works

- **Shared navigation:** Every page has an empty `<div id="nav-placeholder">`. A short jQuery script loads `nav.html` into it, so the navbar only needs to be edited in one place.
- **Responsive layout:** Bootstrap's grid changes the layout by screen size. For example, the skill cards show 2 per row on phones, 3 on tablets, and all 5 in one row on large screens.
- **Accessibility:** Images have descriptive alt text, the navigation has ARIA labels, and the pages were checked with the [WAVE](https://wave.webaim.org/) accessibility tool.

## Running It Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/emmanuelowusu17/Web-portfolio.git
   ```
2. Open the folder in VS Code.
3. Start it with a local server, such as the **Live Server** extension (right-click `index.html` → *Open with Live Server*).

> **Note:** Opening `index.html` by double-clicking it won't show the navigation bar. Browsers block loading `nav.html` from a local file, so a local server is needed.

## Roadmap

This portfolio will grow as I learn more:

- [ ] Contact links and a resume
- [ ] Deploy with GitHub Pages
- [ ] **JavaScript:** dark/light mode toggle, active page highlighting, contact form
- [ ] **Python:** add Python and AI projects
- [ ] Turn the planned projects (Cybersecurity Awareness Hub, Beginner Developer Toolkit) into finished projects

## Author

**Emmanuel Junior Owusu**
Computer Science Student at MSU Denver
GitHub: [@emmanuelowusu17](https://github.com/emmanuelowusu17)
