# Task 6: Host a Static Website with GitHub Pages

**DevOps Internship, Elevate Labs**

## Live Website
🔗 https://ja983.github.io/Elevate-Labs-5/

## Objective
Deploy a simple HTML website for free using GitHub Pages.

## What I Built
A small static website made with HTML and CSS:
- `index.html`: the main page (the default file GitHub Pages loads)
- `style.css`: custom styling (colors, fonts, layout)

## Tools Used
- Git and GitHub
- GitHub Pages
- HTML and CSS

## Steps I Followed
1. Created `index.html` and `style.css` locally.
2. Initialized a Git repository and committed the files:
```bash
   git init
   git add .
   git commit -m "Add static website"
   git branch -M main
```
3. Created a new public repository on GitHub and pushed the code:
```bash
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
```
4. Went to **Settings → Pages**.
5. Set Source to **Deploy from a branch**, selected branch **main** and folder **/ (root)**, then clicked **Save**.
6. Waited 1-2 minutes, then opened the live link GitHub provided.
7. Customized the look with CSS and pushed the changes, which redeployed automatically.

## How to Update the Site
Edit the files, then run:
```bash
git add .
git commit -m "Update site"
git push
```
GitHub Pages rebuilds and redeploys automatically.

## Key Learnings
- GitHub Pages hosts **static** content only (HTML, CSS, JS), with no server-side code.
- `index.html` in the root is the default file served.
- Every push to `main` triggers a new deployment.
- Custom domains are supported through Settings → Pages.

## Interview Questions: Quick Answers
1. What is GitHub Pages?
   A free static site hosting service that serves HTML, CSS and JS directly from a GitHub repository.
   
2. Can you host dynamic apps?
   No. There is no server-side code (PHP, Node, Python backends, databases). Client-side JavaScript works, and you can call external APIs.
   
3. What are the limits?
   Roughly a 1 GB recommended repo/site size, about 100 GB/month soft bandwidth, and 10 builds per hour. Free accounts need public repos,
   and commercial use is discouraged.
   
4. How do you update the site?
   Edit files, then git add, commit and push to the main branch. GitHub rebuilds and redeploys automatically.
   
5. What happens when you delete the repo?
   The site goes offline and the URL returns 404.
   
6. What is the default file?
   index.html in the root of the published folder.
   
7. Can you use a custom domain?
   Yes. Set it under Settings → Pages → Custom domain, and add a CNAME (or A) record at your DNS provider. HTTPS is available too.
