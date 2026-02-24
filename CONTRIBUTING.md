# Contributing to Signature Theme

First off, thank you for considering contributing to Signature Theme! It's people like you that make the open-source community such a great place to learn, inspire, and create.

## Project Philosophy
Signature Theme is a **zero-dependency vanilla CSS framework**. 
* We do **not** use preprocessors like Sass or LESS.
* We do **not** use utility libraries like Tailwind or Bootstrap.
* We rely exclusively on modern CSS3 features (Custom Properties, :has(), @layer, etc.) and semantic HTML5.

## How to Contribute

### 1. Fork and Clone
Fork the repository to your GitHub account and clone it locally:
\\\ash
git clone https://github.com/YOUR_USERNAME/Signature-Theme.git
cd Signature-Theme
\\\

### 2. Branching Strategy
Create a new branch for your feature or bugfix. We use the following naming conventions:
* \eature/your-feature-name\
* \ugfix/issue-description\
* \docs/update-readme\

\\\ash
git checkout -b feature/awesome-new-card
\\\

### 3. Local Development
Because this project has zero dependencies, you don't need npm or build tools. However, to avoid CORS issues with the CDN-loaded fonts, serve the directory via a local HTTP server:
\\\ash
# Python
python -m http.server 8000

# Node.js
npx serve -l 8000
\\\
Visit \http://localhost:8000\ to preview your changes.

### 4. Code Style Requirements
* **CSS:** Use 4 spaces for indentation. Group new rules within the appropriate \@layer\ (reset, base, components, or utilities).
* **HTML:** Maintain semantic structure. Ensure all interactive elements remain accessible.
* **Bi-Directional Support:** Do not use hardcoded \margin-left\ or \padding-right\. Always use logical properties like \margin-inline-start\ and \padding-inline-end\ to maintain automatic RTL/LTR compatibility.

### 5. Commit Convention
We follow [Conventional Commits](https://www.conventionalcommits.org/):
* \eat: add new accordion component\
* \ix: resolve logical property alignment in RTL mode\
* \docs: update API reference for buttons\

### 6. Pull Requests
* Push your branch to your fork.
* Open a Pull Request against our \main\ branch.
* Ensure you fill out the provided Pull Request template completely.
