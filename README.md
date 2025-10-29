# BrainyQuest

BrainyQuest is a small, static educational web project with a collection of kid-friendly games and puzzles. It’s built with plain HTML, CSS and JavaScript so it’s easy to run locally or host on any static site host (GitHub Pages, Netlify, etc.).

## Features

- Home, login, contact and about pages
- Games and puzzles organized under `games/`:
  - `Alpha/` — alphabet-related game
  - `puzzles/` — shape, color, jigsaw, memory and math puzzle pages
  - `quiz/` — quiz page with `quiz.js`
- Simple timer functionality in `timer.js`
- Main scripts: `script.js`, per-game JS files in game folders

## Project structure

home/
- index.html        # main landing page
- about.html
- contact.html
- game.html
- login.html
- script.js         # main site JS
- styles.css        # global styles
- timer.js
- games/
  - Alpha/
    - alpha.html
    - img/
  - puzzles/
    - color.html
    - jigsaw.html
    - math.html
    - memory.html
    - puzzles.html
    - shape.html
    - img/
  - quiz/
    - quiz.html
    - quiz.js
- img/

(This `README.md` lives in the `home/` folder alongside the site files.)

## How to run locally

Option A — Open in browser:

1. Double-click `index.html` (or open it with your browser). This works for most pages that don’t require a server.

Option B — Run a local static server (recommended for consistent behavior):

PowerShell example (from the `home` folder):

```powershell
# change to the project directory, then run a tiny HTTP server
cd 'K:\Project Programs\BrainyQuest\home'
python -m http.server 8000
# Open http://localhost:8000 in your browser
```

If you don't have Python, you can use any static server (Node `http-server`, Live Server extension, etc.).

## Development notes

- Files are plain HTML/CSS/JS; no build step required.
- Keep images under `img/` or the per-game `img/` folder.
- For new games, add a folder under `games/`, add an HTML file and any JS/CSS assets, and link from `index.html` or `game.html`.

## Contributing

1. Fork the repository.
2. Create a branch: `feature/your-feature`.
3. Make changes and keep them small and focused.
4. Open a pull request with a description of the change.

Suggested commit message: `feat: add <game-name> with basic UI and behavior`

## License

This project can be published under MIT License (or change as you prefer). Add a `LICENSE` file in the repo root if you want an explicit license.

## Contact

If you need help or want to collaborate, include your preferred contact information here (email or GitHub handle).

---

Enjoy building and sharing BrainyQuest!
