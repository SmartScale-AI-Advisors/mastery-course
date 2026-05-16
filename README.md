# On the Pursuit of Mastery

A field manual for men in their twenties. Ten weeks. Drawn from Greene, the Stoics, Chamine, Jay, Epstein, and Newport.

## Live site

Once GitHub Pages is enabled on this repo, the manual will be live at:

[**https://smartscale-ai-advisors.github.io/mastery-course/**](https://smartscale-ai-advisors.github.io/mastery-course/)

## How it works

This is a single HTML file. No build step, no dependencies to install, no framework to learn. React and Babel are loaded from a CDN; JSX is compiled in the browser. The reader's progress (completed tasks, notes) is saved to their own browser via `localStorage`.

To work on it locally: open `index.html` in any browser. Done.

To deploy: push to GitHub and enable Pages.

## Repository setup

1. Create a new repo named `mastery-course` under the `SmartScale-AI-Advisors` org on GitHub  
2. Push this folder's contents to the `main` branch  
3. In the repo's Settings → Pages, set Source to "Deploy from a branch" and select `main` / `(root)`  
4. Wait 1–2 minutes for the first deploy  
5. The site will be live at [https://smartscale-ai-advisors.github.io/mastery-course/](https://smartscale-ai-advisors.github.io/mastery-course/)

## File structure

```
mastery-course/
├── index.html    # the entire app
└── README.md     # this file
```

That is intentional. The manual is read-mostly. The simplest architecture is the right one.

## Editing the content

The week-by-week content lives in a JavaScript `program` array inside `index.html`. Each week is a plain object with `title`, `principle`, `greene`, `stoic`, `tasks`, and `reflection` fields. Edit the strings, push to `main`, refresh the live site.

## Notes on browser storage

Reader progress is stored locally per-device. If a reader switches phones, their checkmarks do not follow. This is intentional — the manual asks no account, no sign-in, no tracking. The reader's notes are theirs.  
