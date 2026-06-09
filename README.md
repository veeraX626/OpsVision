# OpsVision

OpsVision is a modern, fully responsive static landing page for a **Server Monitoring Dashboard** platform.
It is designed with a professional SaaS style using a light-elegant glassmorphism theme and interactive dashboard visuals.

## Tech Stack

- HTML5
- CSS3
- JavaScript (Vanilla)
- Nginx (for containerized static hosting)

## Project Structure

```text
.
├── assets/
├── css/
│   └── style.css
├── js/
│   └── script.js
├── index.html
├── Dockerfile
└── .dockerignore
```

## Features

- Responsive design for mobile, tablet, and desktop
- Modern glassmorphism UI
- Smooth scroll and reveal animations
- Animated live metrics counters
- Interactive FAQ accordion
- Realistic monitoring dashboard widgets
- SEO-friendly semantic HTML layout

## Run Locally

You can serve the static site using Python:

```bash
cd /Users/veerabhanushali/Desktop/Jenkins
python3 -m http.server 8085
```

Then open:

- `http://127.0.0.1:8085`
- `http://localhost:8085`

## Run with Docker (Nginx)

Build the image:

```bash
docker build -t opsvision:latest .
```

Run the container:

```bash
docker run --name opsvision -p 8085:80 --rm opsvision:latest
```

Open in browser:

- `http://127.0.0.1:8085`

## Notes

- The project is fully static and has no backend dependencies.
- The Docker image serves files from Nginx default web root: `/usr/share/nginx/html`.
- `.dockerignore` excludes repo/editor noise for cleaner builds.

## Customization

- Update layout/content in `index.html`
- Update theme and styles in `css/style.css`
- Update interactions in `js/script.js`
