# Deploy this as your GitHub profile README

These files are built for **[em-Abdullah](https://github.com/em-Abdullah)** — Tenno theme (slate + cyan + emerald).

Your profile repo **already exists**: [`em-Abdullah/em-Abdullah`](https://github.com/em-Abdullah/em-Abdullah).  
This package **replaces** that README with the animated Tenno layout, while keeping your links, about, and tech stack.

## 1. Push into the profile repo

From this project (or copy the SVG + README + `.github` files into `em-Abdullah/em-Abdullah`):

```bash
git remote add profile https://github.com/em-Abdullah/em-Abdullah.git   # once
git push profile main:main
```

Or manually: replace `README.md`, all `abdullah-*.svg` files, and `.github/workflows/snake.yml` in that repo.

## 2. Enable the contribution snake

1. Open the repo → **Actions** → enable workflows if prompted  
2. Run **Generate Snake** once (workflow dispatch)  
3. After it finishes, the `output` branch will hold the snake SVGs and the README snake section will light up  

## 3. Local preview

```bash
python3 preview/serve.py
```

Then open the URL printed in the terminal (default `http://127.0.0.1:43127`).

## Customization

| File | What it is |
|------|------------|
| `abdullah-banner.svg` | Dark banner + floating animated photo avatar |
| `abdullah-banner-light.svg` | Light-mode banner |
| `abdullah-lanyard.svg` | Swinging ID badge with your photo |
| `abdullah-stats.svg` | Stats card |
| `abdullah-langs.svg` | Languages card |
| `abdullah-trophies.svg` | Trophy row |
| `README.md` | Profile layout |

Theme colors live in those SVGs: cyan `#22d3ee`, emerald `#34d399`, slate panels `#0c1219`.

Featured Work on the right of the badge is intentionally empty (“soon”) until you have public projects to list.
