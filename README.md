# Smart College Assistant

A digital platform for college students: dashboard, notices, faculty, subjects, academic dates, search and a college chatbot. Built for B.Tech Computer Science, Semester 5 (AKTU curriculum).

## Features
- Student account: create account, sign in, forgot password, sign out
- Dashboard with attendance, CGPA, semester subjects, upcoming dates and latest notices
- Notices and announcements
- Faculty information (role, office, hours, email)
- Subject information (code, teacher, unit outline)
- Important academic dates with countdowns
- Search across notices, faculty, subjects, dates and FAQs
- College assistant chatbot (ChatGPT-style chat window)
- Light and dark mode, responsive on mobile

## Tech stack
HTML, CSS and JavaScript in a single file (`index.html`). No build step.

## Run locally
Open `index.html` in any browser.

## Publish on GitHub Pages
1. Create a new repository and upload `index.html` and `README.md`.
2. Go to Settings > Pages.
3. Under Source choose "Deploy from a branch", branch `main`, folder `/ (root)`, then Save.
4. After a minute the site is live at `https://<your-username>.github.io/<repository-name>/`.

## Customise the data
Edit the arrays at the top of the `<script>` in `index.html`: `FAC` (faculty), `SUB` (subjects), `NOT` (notices), `CAL` (dates), `FAQ` (chatbot answers) and `STUDENT`.

## Notes and limits
- Sign-in data is stored in the browser (localStorage) with hashed passwords. It is a demo and not secure. For real accounts use Firebase Authentication.
- On GitHub Pages the chatbot answers from the built-in college FAQ and data. Open-ended AI answers need a backend (for example a Firebase Cloud Function) that calls an AI API, because API keys must never be placed in a public page.
- Faculty names, notices and dates are sample data. Subject unit outlines are summaries; check the official AKTU syllabus for exact content.
