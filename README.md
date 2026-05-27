# Personal Website

A simple, fast personal site — no build tools, no dependencies, just HTML/CSS.

## File structure

```
├── index.html          ← homepage (bio + experience)
├── blog.html           ← blog post listing
├── style.css           ← shared styles
└── blog/
    └── my-first-post.html   ← example/template post
```

## Deploying to GitHub Pages

1. Create a new repo on GitHub (e.g. `yourusername.github.io` for a root domain, or any name for a project page)
2. Push all these files to the repo
3. Go to **Settings → Pages → Source** and select your `main` branch
4. Your site will be live at `https://yourusername.github.io` (or `.../repo-name`)

For a custom domain: add a `CNAME` file with your domain, then configure DNS with your registrar.

## Writing a new blog post

1. Duplicate `blog/my-first-post.html`
2. Rename it (e.g. `blog/notes-on-rust.html`)
3. Update the `<title>`, `<meta name="description">`, and the post content
4. Add a new entry to `blog.html` pointing to it
5. Optionally add a preview to `index.html` in the "recent writing" section

## Customizing

- **Name / links**: search for `Your Name`, `yourusername`, `yourprofile`, `you@email.com` and replace throughout
- **Colors**: all in `style.css` under `:root` — change `--accent` for the orange highlight color
- **Fonts**: loaded from Google Fonts — swap the import URL in `style.css` to change them
- **Adding a projects page**: duplicate `blog.html`, change the content to a project grid
