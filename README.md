# Privacy Pages Repository

This repository is designed to host privacy policies and terms of service for multiple applications.

## Structure

```
privacy-pages/
├─ index.html                         # Entry point: lists links to all app policies
├─ apps/
│  ├─ moji/
│  │  ├─ index.html                   # Moji App entry (optional)
│  │  ├─ privacy/
│  │  │  └─ index.html                # Moji Privacy Policy page
│  │  ├─ terms/
│  │  │  └─ index.html                # Moji Terms of Use
│  │  └─ assets/
│  │     └─ style.css                 # Moji App-specific styles
│  ├─ app2/
│  │  ├─ privacy/index.html           # App2 Privacy Policy page
│  │  └─ assets/style.css             # App2 App-specific styles
│  └─ ...                              # Add more apps here
├─ templates/
│  ├─ app-privacy.template.html       # Template for new app privacy policies
│  └─ app-terms.template.html         # Template for new app terms of service
├─ .nojekyll                          # Prevents Jekyll from processing the site
└─ README.md
```

## How to add a new application

1.  Create a new directory under `apps/` with your app's name (e.g., `apps/new-app/`).
2.  Inside your new app directory, create `privacy/` and optionally `terms/` and `assets/` directories.
3.  Copy `templates/app-privacy.template.html` to `apps/new-app/privacy/index.html` and modify its content.
4.  Optionally, copy `templates/app-terms.template.html` to `apps/new-app/terms/index.html` and modify its content.
5.  Optionally, create `apps/new-app/assets/style.css` for app-specific styling.
6.  Update the main `index.html` to include links to your new app's policies.

## Live Demo

You can view the live demo of this project hosted on GitHub Pages here: [https://mett-barr.github.io/privacy-pages/](https://mett-barr.github.io/privacy-pages/)
