# TLNE / Your timelines

A standalone, browser-based Gantt planner with a terminal-inspired theme.

## Run locally

Open `index.html` in Chrome, Edge, Firefox, or Safari. There is no build step, dependency installation, or server requirement.

You can also serve the folder locally (optional):

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Features

- Expandable workstreams and reorderable subtasks
- Editable task names, descriptions, dates, durations, completion, and colors
- Draggable and resizable Gantt bars
- Graphical task dependencies with movable connector routing
- Zoom from days to years and fit-to-project view
- JSON import/export, including project name, task order, and dependencies
- Browser-local autosave

## Data

The application stores the current project in your browser's local storage. **Browser local storage is not synchronized across devices or repositories.** Use **Export JSON** to back up project data and **Import JSON** to restore it.

This repository contains the application only, not your browser's saved project data.

## Deploy with GitHub Pages

1. Create a GitHub repository and push the contents of this folder.
2. In your repository, go to **Settings → Pages**.
3. Select **Deploy from a branch**, choose `main` and `/ (root)`, then save.

GitHub Pages can serve `index.html` directly. No build configuration is needed.

## Git quick start

```bash
git init
git add .
git commit -m "Initial TLNE Gantt planner"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
git push -u origin main
```

Replace the example GitHub URL with your own repository URL.

## Architecture

`index.html` contains the HTML, CSS, JavaScript, and embedded TLNE logo in a single file. This keeps the app portable. The code can be split into separate files later as the project grows.
