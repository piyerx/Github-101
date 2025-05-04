 # GitHub Pages Guide

Learn how to host your website or project documentation directly from a GitHub repository using GitHub Pages.

---

## 📚 Table of Contents

* [1. What is GitHub Pages?](#1-what-is-github-pages)
* [2. Types of GitHub Pages](#2-types-of-github-pages)
* [3. Setting Up GitHub Pages](#3-setting-up-github-pages)
* [4. Custom Domain (Optional)](#4-custom-domain-optional)
* [5. Tips and Notes](#5-tips-and-notes)

---

## 1. What is GitHub Pages?

GitHub Pages is a free static site hosting service that takes files from a GitHub repository and serves them as a website.

Great for:

* Portfolios
* Project documentation
* Blog/static websites (Jekyll, Hugo, etc.)

## 2. Types of GitHub Pages

* **User/Organization Site:**

  * Must be named `username.github.io`
  * One per GitHub account
  * Hosted from the root of the `main` branch

* **Project Site:**

  * Can be any repo name
  * Hosted from the `docs/` folder or `gh-pages` branch
  * URL: `https://username.github.io/repository-name/`

## 3. Setting Up GitHub Pages

### For a Project Site:

1. Go to your repository on GitHub.
2. Click on **Settings** > **Pages** (on the sidebar).
3. Under **Source**, choose:

   * Branch: `main`
   * Folder: `/root` or `/docs` (if your HTML is inside a docs folder)
4. Click **Save**.
5. GitHub will provide a URL to access your site.

### Example

```html
index.html
style.css
```

Once enabled, site will be hosted at:
`https://username.github.io/repository-name/`

## 4. Custom Domain (Optional)

1. Purchase and configure your custom domain with DNS.
2. In **Pages settings**, enter your custom domain.
3. Create a `CNAME` file with your domain name inside the repository (optional if GitHub adds it automatically).
4. GitHub handles HTTPS automatically.

## 5. Tips and Notes

* Changes pushed to the repo take a few seconds to reflect.
* Make sure your `index.html` is at the correct location.
* You can use GitHub Actions to automate build and deploy workflows.
* You can add `.nojekyll` file if you're not using Jekyll to avoid unwanted processing.

---

## Final Thoughts

GitHub Pages is a powerful and free way to showcase your work or build lightweight web apps. Experiment with it and use it to give your projects a home online.

*~Created by [Piyush](https://github.com/piyerx)*