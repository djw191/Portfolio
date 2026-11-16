# Derek Woodard — Portfolio

Source for my portfolio site: **https://djw191.github.io/Portfolio/**

I'm a software developer at Epic and a contract gameplay programmer on [IVOR](https://store.steampowered.com/app/3033980/IVOR/), a Unity first-person shooter. The site collects my professional work, game projects, and resume.

## Highlights

- **[IVOR](https://djw191.github.io/Portfolio/tags/#ivor)**: enemy AI, ragdoll and destruction physics, rebinding menus, performance, and lighting for a Unity FPS
- **[Epic](https://djw191.github.io/Portfolio/blog/Epic/)**: hospital inventory software in MUMPS and React
- **[Mythos](https://djw191.github.io/Portfolio/blog/Mythos/)**: networked card game with a C# socket server, Best in Show at the 2022 MAGD Expo, later [rewritten in Haskell](https://djw191.github.io/Portfolio/blog/UWM-Special-Topics-Haskell/) with TLS
- **[Resume (PDF)](https://djw191.github.io/Portfolio/assets/Resume.pdf)**

## Built with

- [Jekyll](https://jekyllrb.com/) on GitHub Pages
- [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes) theme (`dirt` skin)
- LaTeX for the resume (`assets/resume.tex`)

## Running locally

Requires Ruby 3.3 with Bundler.

```sh
bundle install
bundle exec jekyll serve --livereload
```

Then open http://127.0.0.1:4000.

## Building the resume

Requires a LaTeX distribution (MiKTeX or TeX Live).

```sh
cd assets
pdflatex -jobname=Resume resume.tex
```

## Layout

| Path | Contents |
|---|---|
| `_posts/` | Project write-ups |
| `_pages/` | About page, archives, 404 |
| `_includes/head/custom.html` | Favicons |
| `assets/images/` | Post and feature images |
| `assets/resume.tex` | Resume source (`Resume.pdf` is the built copy) |
