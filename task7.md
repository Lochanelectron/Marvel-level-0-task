# Task 7 — Portfolio Webpage
 
## What the Task Was
 
Build a personal portfolio website that shows info about yourself — interests, projects, social media, etc. It had to be responsive and pushed to a GitHub repo. No framework restrictions.
 
---
 
## What I Built
 
A single-page portfolio using plain **HTML, CSS, and vanilla JavaScript** — no frameworks needed.
 
The site has these sections:
 
- **Hero** — Name, tagline, and a call-to-action button
- **About** — A short intro with a live "status" card showing current state (mood, passion found, etc.)
- **Education** — A timeline layout with placeholder slots to fill in degree and school details
- **Interests** — Cards covering things like building stuff and iterating through life experiences
- **Projects** — Pre-styled cards ready to be filled in with real projects later
- **Contact** — Email listed, all social media platforms crossed out (not on any of them)
 
---
 
## Design Choices
 
- **Dark theme** with yellow accents
- **Syne** (display font) + **Space Mono** (body font) — gives it a techy but personality-filled look
- Scroll animations using `IntersectionObserver`
- Fully **responsive** — hamburger menu on mobile, single-column layout on small screens
- Humor baked in — status shows `passion_found: false`, contact section says *"this man is living under a rock"*
 
---
 
## How to Deploy (GitHub Pages)
 
1. Create a GitHub account at github.com
2. Make a new **public** repo named `your-username.github.io`
3. Upload `index.html` via the GitHub UI
4. Go to **Settings → Pages**, set branch to `main`, save
5. Live URL will be: `https://your-username.github.io`
 
---
 
## What's Left to Fill In
 
| Section | What to add |
|---|---|
| Education | Degree name, university, years |
| Projects | Project name, description, link |
| Contact | Nothing — email is already there |
 
---
 
## Files
 
| File | Description |
|---|---|
| `index.html` | The entire website — HTML + CSS + JS in one file |
 
---
 
*Built for the Web Development module — Task 7.*
