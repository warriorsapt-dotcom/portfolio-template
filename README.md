# Warrior Portfolio

A developer portfolio built with HTML, CSS and vanilla JavaScript. A dark interface with neon green accents introduces the developer, highlights projects and links to public GitHub repositories.

![Portfolio preview](Screenshot%20From%202025-10-09%2003-38-39.png)

## What it demonstrates

- Responsive layouts using CSS Grid, Flexbox and media queries.
- A separate projects page that loads up to 20 public repositories from the GitHub API, ordered by recent updates.
- Loading, empty and error states for repository requests.
- Keyboard focus styles, contact links and small visual effects.
- Static hosting without a package manager or build step.

## Run locally

Clone the repository and open `index.html` in your browser:

```sh
git clone https://github.com/warriorsapt-dotcom/portfolio-template.git
cd portfolio-template
```

For a local HTTP preview, run this from the repository directory with Python 3 installed:

```sh
python -m http.server 8000
```

Open http://localhost:8000. The projects page requires internet access to reach GitHub.

## Customize

| File | What to change |
| --- | --- |
| `index.html` | Introduction, skills, featured projects, contact details and social links |
| `index.html` → `:root` | Background, accent and text colors |
| `projects.html` → `const user` | GitHub username used to load repositories |

Replace the sample project links and placeholder footer links before using the template as your own portfolio.

## Contact form behavior

The form currently validates input and **simulates a successful submission** with a timer. It does not deliver messages. Use the email link for contact, or replace `handleForm` with a real submission integration before offering the form to visitors.

## Deploy

Upload the repository's static files to a static web host. Keep `index.html` and `projects.html` in the same directory; no build command is needed. For GitHub Pages, configure deployment from the `main` branch and repository root in the repository's Pages settings.

## Repository layout

```text
index.html                              Landing page, styles and interactions
projects.html                           Public GitHub repository browser
Screenshot From 2025-10-09 03-38-39.png  Portfolio preview
LICENSE                                 MIT license
```

## License

[MIT](LICENSE).
