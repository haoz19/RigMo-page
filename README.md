# RigMo Project Page

Source for the [RigMo](https://arxiv.org/abs/2601.06378) project page.

> **RigMo: Unifying Rig and Motion Learning for Generative Animation**
> Hao Zhang, Jiahao Luo, Bohui Wan, Yizhou Zhao, Zongrui Li, Michael Vasilkovsky,
> Chaoyang Wang, Jian Wang, Narendra Ahuja, Bing Zhou.

This is a static site (single `index.html` with inline CSS, plus image assets under
`pdf2png/`). No build step is required.

## Local preview

```bash
python -m http.server 8000
# then open http://localhost:8000
```

## Deploy (GitHub Pages)

1. Push this folder to a GitHub repo (e.g. `haoz19/RigMo-page`).
2. In the repo: **Settings → Pages → Build and deployment**.
3. Set **Source = Deploy from a branch**, **Branch = `main`**, **Folder = `/ (root)`**.
4. The site goes live at `https://haoz19.github.io/RigMo-page/`.

The `.nojekyll` file is required so GitHub Pages serves all asset folders verbatim.

## Structure

```
.
├── index.html              # the whole page
├── RigMo.png               # logo / favicon
├── .nojekyll               # disable Jekyll processing
└── pdf2png/                # figure images
    ├── teaser/teaser-1.png
    ├── overview/overview-1.png
    ├── DiT/DiT-1.png
    ├── fig3/fig3-1.png
    ├── fig4/fig4-1.png
    └── fig6/fig6-1.png
```
