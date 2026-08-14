# Adnan Khan — Portfolio

Personal portfolio site. Operations Research and Stochastic Optimization.

Single-file build: `index.html` contains all HTML, CSS and JavaScript. No frameworks, no build step, no dependencies. It loads two Google Fonts and nothing else.

## What is in it

- **The Lab** — three optimization models running live in the browser:
  - **Vehicle Routing** — Clarke-Wright savings with 2-opt refinement, benchmarked against a nearest-neighbour sequential baseline. Mirrors the comparison in the thesis.
  - **Markov Decision Process** — value iteration on the Bellman optimality equation, using the exact parameters from the CentraleSupélec machine replacement project: ten degradation states, y(s) = 5 + s − 0.15s², profit 150 k€/ton. Adjust γ, replacement cost and transition probability and the threshold policy moves correctly.
  - **Risk-Averse Capacity Planning** — expected cost against CVaR over sampled demand scenarios, showing that risk aversion buys more capacity. A reduced form of the two-stage stochastic power generation model.
- Projects, thesis, experience, education, toolkit, awards, languages
- Downloadable CV

## Deploy to GitHub Pages

1. Create a repository named exactly `Adnan-Khan-OR.github.io` (replace with your GitHub username).
2. Upload `index.html`, `README.md` and the `assets/` folder. Drag and drop into the browser works.
3. Go to **Settings → Pages**. Under *Source* pick **Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
4. Wait two or three minutes. The site is live at `https://Adnan-Khan-OR.github.io`.

For a project-page URL instead, name the repo anything (for example `portfolio`) and the address becomes `https://Adnan-Khan-OR.github.io/portfolio`.

## Editing

Everything is in `index.html`.

- Text content sits in plain HTML between the `<section>` tags.
- Colours are CSS variables at the top of `<style>`: `--ac` is the teal accent, `--ac2` amber, `--bg` background.
- The three demos are at the bottom of `<script>`, each clearly commented.

## Files

```
index.html                 whole site
README.md                  this file
assets/adnan.jpg           portrait
assets/Adnan-Khan-CV.pdf   downloadable CV
assets/SO-P1-_*.png        result figures from the power generation notebook
```

## Still to add

- Repository links on each project card, once the code is public
- Thesis results: instance size, improvement over baseline, solve time
- A permanent email address in place of the student one
