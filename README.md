# Emmanuel Owusu – Web Portfolio

My personal portfolio website, built as part of a Web Development Fundamentals course at MSU Denver. It introduces who I am, the skills I'm learning, and the projects I'm working on as a Computer Science student.

**Live site:** https://emmanuelowusu17.github.io/Web-portfolio/

## Built With

- **HTML5** – page structure
- **CSS3** – custom styling (`style.css`)
- **Bootstrap 5.3** – responsive grid, cards, buttons, and navbar
- **Bootstrap Icons** – email, GitHub, and LinkedIn icons
- **jQuery** – loads the shared navigation bar into each page
- **Git & GitHub** – version control

## Pages

| Page | Description |
|------|-------------|
| **Home** (`index.html`) | Intro section with my photo, short bio, contact links, a skills section, and featured projects |
| **Projects** (`projects.html`) | Details about each project I'm working on |
| **About** (`about.html`) | My background, my CS journey, what I'm currently learning, and my career goals |
| **Contact** (`contact.html`) | Ways to reach me: email, GitHub, and LinkedIn |

## Projects

### Cybersecurity Awareness Hub

**Live site:** https://emmanuelowusu17.github.io/Web-portfolio/cybersecurity/

A cybersecurity awareness website that teaches students and everyday internet users how to protect their personal information and online accounts. It covers three habits: spotting phishing, creating strong passwords, and turning on multifactor authentication (MFA).

#### Purpose

Most people don't get hacked by advanced attacks. They get tricked by a fake email, or they reuse a weak password. This site turns official government security guidance into short, plain-English pages with examples and clear steps, so that anyone can understand it and act on it. You don't need a technical background.

#### The Problem It Solves

- **Phishing works because people don't know the warning signs.** In 2025, people reported losing **$215,843,126** to phishing and spoofing scams to the FBI ([IC3 2025 Internet Crime Report](https://www.ic3.gov/AnnualReport/Reports/2025_IC3Report.pdf), p. 8).
- **Weak and reused passwords** let one stolen password unlock many accounts.
- **Many people have never turned on MFA**, even though it can stop a criminal who already has their password.
- **Official guidance is hard to read.** Sources like NIST's Digital Identity Guidelines are written for IT professionals, not everyday users.

#### Who It's For

Students and everyday internet users who want to protect their personal information and online accounts from cybercriminals.

#### Benefits

After using the site, a visitor should be able to:

- **Recognize phishing** emails, texts, and suspicious links, and know what to do if they already clicked one
- **Create strong passwords** using passphrases and a password manager
- **Turn on MFA** and choose the strongest method an account offers
- **Report scams** to the right place (FTC, FBI IC3, APWG, or SPAM 7726)
- **Take action right away** with a printable safety checklist

Taken together, these habits help prevent identity theft, financial loss, and account takeover.

#### Planning

The project started as a plan for a cybersecurity course assignment:

1. **Identified the need:** phishing and weak passwords are among the most common ways criminals get into accounts.
2. **Chose the audience:** students and everyday internet users.
3. **Set the goal:** users should be able to recognize phishing, create strong passwords, and use MFA.
4. **Chose the format:** a website, because it's easy to share with a link, works on phones and computers, and lets people learn at their own pace.
5. **Researched and verified** every fact using four reliable sources (listed below).
6. **Outlined the pages** before writing any code: Home → Phishing → Passwords → MFA → Resources.
7. **Built it one page at a time**, committing each page to GitHub as it was finished.

#### Why a Website?

- **Shareable:** anyone can open it from a single link, with nothing to download.
- **Self-paced:** visitors can jump to the topic they need.
- **Responsive:** it works on a phone, where most phishing texts are read.
- **Interactive:** it includes a clickable "What If...?" section, a checklist, and a practice phishing email.

#### Pages

| Page | What it teaches |
|------|-----------------|
| **Home** | Why online safety matters, a real FBI statistic, and 3 things to do today |
| **Phishing** | Scammers' common stories, a **practice phishing email with 5 marked red flags**, the Recognize → Resist → Delete steps, and what to do if you clicked |
| **Passwords** | The 3 rules (long, random, unique), weak vs. strong examples, passphrases, password managers, and password myths vs. facts |
| **MFA** | What MFA is, how it stops criminals, MFA methods ranked from strongest to weakest, and how to turn it on |
| **Resources** | A printable safety checklist, where to report scams, and all sources |

#### How It Was Built

- **HTML, CSS, and Bootstrap 5.3**, with no custom JavaScript.
- **Same repository as the portfolio:** the site lives in its own `cybersecurity/` folder with its own `nav.html` and `cyber.css`. Relative links connect the two sites. `cybersecurity/index.html` goes into the site, and `../index.html` goes back to the portfolio.
- **Bootstrap components** for clear communication:
  - cards for topics
  - an accordion for the "What If...?" questions
  - alerts for warnings
  - tables for examples and reporting
  - checkboxes for the safety checklist
- **A "digital grid" banner** drawn with pure CSS (`linear-gradient`) to give the site a cyber look without image files.
- **Accessibility:**
  - high-contrast colors
  - `aria-label`s on the red-flag markers
  - `<caption>` and `scope` on tables
  - `<fieldset>`/`<legend>` for checklist groups
  - decorative emoji hidden from screen readers
  - reduced motion for users who prefer it
- **Print-friendly:** an `@media print` rule hides the navbar and footer when the checklist is printed.
- **Safety by design:** the practice phishing email uses a made-up company ("StreamFlix"), and its "button" is plain text, so it can't be clicked. External links use `rel="noopener"`.

#### Sources

1. **CISA**, *Secure Our World*: https://www.cisa.gov/secure-our-world
2. **Federal Trade Commission (FTC)**, *How to Recognize and Avoid Phishing Scams*: https://consumer.ftc.gov/articles/how-recognize-and-avoid-phishing-scams
3. **NIST**, *Digital Identity Guidelines (SP 800-63-4)*: https://pages.nist.gov/800-63-4/
4. **FBI Internet Crime Complaint Center (IC3)**, *2025 Internet Crime Report*: https://www.ic3.gov/AnnualReport/Reports/2025_IC3Report.pdf

### Beginner Developer Toolkit

**Live site:** https://emmanuelowusu17.github.io/Web-portfolio/toolkit/

A step-by-step guide for people who are new to software engineering, or who have a passion for building things and want to learn how to make a website. It teaches HTML, CSS, and Bootstrap, plus version control with Git and GitHub, and ends with publishing a real website for free.

#### Purpose

Learning to code can feel overwhelming at the start. There are many tools, and most tutorials assume you already know which one to learn first. This toolkit puts the five core tools in order, explains each one in plain English, and shows real code that beginners can copy and change. The goal is for a complete beginner to go from an empty folder to a live website.

#### The Problem It Solves

- **Beginners don't know where to start.** HTML, CSS, Bootstrap, Git, and GitHub are often taught separately, so it's hard to see how they fit together.
- **Official documentation is written for developers.** Guides like MDN and the Bootstrap docs are excellent, but they can be a lot for someone on day one.
- **Version control is often skipped.** Many beginners never learn Git until a job or a class requires it, even though it protects their work from the start.
- **Publishing seems hard.** Many beginners don't know they can put a website online for free with GitHub Pages.

#### Who It's For

People who are new to software engineering, students, career changers, and anyone with a passion for building websites who doesn't know where to begin. No experience is needed.

#### Benefits

After using the toolkit, a visitor should be able to:

- **Set up the free tools** a web developer uses: VS Code, Live Server, Git, and a GitHub account
- **Write an HTML page** with headings, paragraphs, links, lists, and images
- **Style a page with CSS** using selectors, common properties, and the box model
- **Build a responsive layout** with Bootstrap's grid and components
- **Use Git and GitHub** to commit changes and push a project online
- **Publish a website** with GitHub Pages

#### Planning

1. **Identified the need:** beginners struggle to know which tools to learn and in what order.
2. **Chose the audience:** people new to software engineering or with a passion for building websites.
3. **Set the goal:** a visitor should be able to build a simple website and publish it with GitHub Pages.
4. **Chose the format:** a website, so the lessons can show real code and live Bootstrap examples that work on the page.
5. **Ordered the lessons** like a learning path: HTML → CSS → Bootstrap → Git & GitHub, with each step building on the last.
6. **Verified the content** against official documentation (listed below).
7. **Reused the structure** of the Cybersecurity Awareness Hub: a shared navbar, one CSS file, and the same page layout.

#### Pages

| Page | What it teaches |
|------|-----------------|
| **Home** | Who it's for, how the tools fit together (explained like building a house), the 4-step learning path, and the free tools to install |
| **HTML** | What HTML is, the parts of an element, the basic page structure, common tags, a "try it yourself" exercise, good habits, and common mistakes |
| **CSS** | What CSS is, how to link a stylesheet, the parts of a CSS rule, selectors, common properties, the box model, and a practice stylesheet |
| **Bootstrap** | How to add Bootstrap, the 12-column grid with a **live resizable example**, breakpoints, live buttons, alerts, and cards next to their code, and utility classes |
| **Git & GitHub** | Git vs. GitHub, key words, how code moves from your folder to GitHub, one-time setup, the commands for a first project, commit messages, and publishing with GitHub Pages |
| **Resources** | A printable beginner checklist, practice project ideas, and free sources for further learning |

#### How It Was Built

- **HTML, CSS, and Bootstrap 5.3**, with no custom JavaScript, the same as the Cybersecurity Awareness Hub.
- **Its own folder:** the site lives in `toolkit/` with its own `nav.html` and `toolkit.css`. `../index.html` links back to the portfolio.
- **Code examples** use `<pre>` and `<code>` with a dark, editor-style design and a file-name label. Symbols like `<` and `>` are written as `&lt;` and `&gt;` so the browser shows the code instead of running it.
- **Live examples:** the Bootstrap page includes working grid columns, buttons, alerts, and a card, so visitors see the result next to the code.
- **A box model diagram** made from four nested `<div>`s styled with CSS, with no image files.
- **Accessibility:**
  - high-contrast colors, including a darker color for inline code
  - `<caption>` and `scope` on tables
  - `<fieldset>`/`<legend>` for checklist groups
  - `tabindex="0"` on code blocks, so keyboard users can scroll long lines
  - decorative emoji hidden from screen readers
  - reduced motion for users who prefer it
- **Print-friendly:** an `@media print` rule hides the navbar and footer when the checklist is printed.

#### Sources

1. **MDN Web Docs**, *Learn Web Development*: https://developer.mozilla.org/en-US/docs/Learn_web_development
2. **Bootstrap**, *Bootstrap 5.3 Documentation*: https://getbootstrap.com/docs/5.3/getting-started/introduction/
3. **Scott Chacon and Ben Straub**, *Pro Git* (2nd edition): https://git-scm.com/book/en/v2
4. **GitHub Docs**, *Get Started*: https://docs.github.com/en/get-started
5. **GitHub Docs**, *GitHub Pages Quickstart*: https://docs.github.com/en/pages/quickstart

## Project Structure

```
Web-portfolio/
├── index.html       # Home page
├── projects.html    # Projects page
├── about.html       # About page
├── contact.html     # Contact page
├── nav.html         # Shared navigation bar, loaded into every page
├── style.css        # Custom styles
├── images/          # Profile photo, skill logos, project images, background
├── cybersecurity/   # Cybersecurity Awareness Hub (its own mini-site)
│   ├── index.html       # Home: why it matters, topics, 3 things to do today
│   ├── phishing.html    # Spotting phishing, practice email, what-if answers
│   ├── passwords.html   # Strong password rules, examples, myths vs. facts
│   ├── mfa.html         # What MFA is, ranked methods, how to turn it on
│   ├── resources.html   # Checklist, where to report, sources
│   ├── nav.html         # Navigation bar for the cybersecurity pages
│   └── cyber.css        # Styles for the cybersecurity pages
├── toolkit/         # Beginner Developer Toolkit (its own mini-site)
│   ├── index.html            # Home: who it's for, how the tools fit, learning path, tools to install
│   ├── html-basics.html      # Step 1: HTML elements, page structure, common tags
│   ├── css-basics.html       # Step 2: CSS rules, selectors, properties, box model
│   ├── bootstrap-basics.html # Step 3: Bootstrap grid, live components, utility classes
│   ├── git-github.html       # Step 4: Git commands, GitHub, publishing with GitHub Pages
│   ├── resources.html        # Checklist, practice projects, sources
│   ├── nav.html              # Navigation bar for the toolkit pages
│   └── toolkit.css           # Styles for the toolkit pages
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

- [x] Contact links (email, GitHub, LinkedIn)
- [ ] Resume
- [x] Deploy with GitHub Pages
- [x] Build the Cybersecurity Awareness Hub
- [x] Build the Beginner Developer Toolkit
- [ ] **JavaScript:** dark/light mode toggle, active page highlighting, contact form, and a phishing quiz and saved checklist for the Cybersecurity Awareness Hub
- [ ] **Python:** add Python and AI projects

## Author

**Emmanuel Junior Owusu**
Computer Science Student at MSU Denver
GitHub: [@emmanuelowusu17](https://github.com/emmanuelowusu17)
LinkedIn: [Emmanuel Owusu](https://www.linkedin.com/in/emmanuel-owusu-128698404)
