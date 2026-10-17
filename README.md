# Emmanuel Owusu – Web Portfolio

My personal portfolio website, built as part of a Web Development Fundamentals course at MSU Denver. It introduces who I am, the skills I'm learning, and the projects I'm working on as a Computer Science student.

**Live site:** https://emmanuelowusu17.github.io/Web-portfolio/

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

### Beginner Developer Toolkit *(planned)*

A guide for beginners interested in web development, covering tools such as HTML, CSS, Bootstrap, Git, and GitHub.

## Project Structure

```
Web-portfolio/
├── index.html       # Home page
├── projects.html    # Projects page
├── about.html       # About page
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
- [x] Deploy with GitHub Pages
- [x] Build the Cybersecurity Awareness Hub
- [ ] Build the Beginner Developer Toolkit
- [ ] **JavaScript:** dark/light mode toggle, active page highlighting, contact form, and a phishing quiz and saved checklist for the Cybersecurity Awareness Hub
- [ ] **Python:** add Python and AI projects

## Author

**Emmanuel Junior Owusu**
Computer Science Student at MSU Denver
GitHub: [@emmanuelowusu17](https://github.com/emmanuelowusu17)
