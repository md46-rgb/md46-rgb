md46-rgb/
├── README.md
├── assets/
│   └── banner.svg
└── .github/
    └── workflows/
        └── snake.yml<div align="center">

<img width="100%" src="./assets/banner.svg">

# Hi 👋 I'm md46-rgb

<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=28&pause=1000&color=00F7FF&center=true&vCenter=true&width=800&lines=AI+Developer;Python+Engineer;Machine+Learning+Explorer;Building+cool+things+⚡"/>

<p>
Building projects • Learning continuously • Exploring AI
</p>

<img src="https://komarev.com/ghpvc/?username=md46-rgb&label=Profile+Views&color=0e75b6&style=for-the-badge"/>

</div>

---

## 🚀 About Me

- 🔭 Working on AI projects
- 🌱 Learning LLM engineering
- 💻 Exploring full-stack development
- ⚡ Open source enthusiast

---

## 🛠 Tech Stack

<p align="left">

<img src="https://skillicons.dev/icons?i=python,tensorflow,pytorch,opencv,fastapi,mongodb,docker,git,github,vscode"/>

</p>

---

## 📊 GitHub Stats

<div align="center">

<img width="49%" src="https://github-readme-stats.vercel.app/api?username=md46-rgb&show_icons=true&theme=tokyonight"/>

<img width="49%" src="https://github-readme-streak-stats.herokuapp.com/?user=md46-rgb&theme=tokyonight"/>

<img width="49%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=md46-rgb&layout=compact&theme=tokyonight"/>

</div>

---

## 🏆 Trophies

<div align="center">

<img src="https://github-profile-trophy.vercel.app/?username=md46-rgb&theme=algolia&no-frame=true"/>

</div>

---

## 🐍 Contribution Snake

<div align="center">

<img src="https://github.com/md46-rgb/md46-rgb/blob/output/github-contribution-grid-snake.svg"/>

</div>

---

## 📌 Featured Projects

- AI Project #1
- AI Project #2
- Full Stack Project
- Open Source Contribution

---

<div align="center">

⭐ Thanks for visiting

</div>
<svg fill="none" viewBox="0 0 1000 220" xmlns="http://www.w3.org/2000/svg">
<rect width="1000" height="220" fill="#0d1117"/>
<circle cx="150" cy="60" r="100" fill="#00F7FF" opacity=".15"/>
<circle cx="850" cy="170" r="140" fill="#8A2BE2" opacity=".15"/>
<text x="50%" y="48%" dominant-baseline="middle" text-anchor="middle"
font-size="42" fill="#00F7FF" font-family="monospace">
md46-rgb
</text>
<text x="50%" y="68%" dominant-baseline="middle" text-anchor="middle"
font-size="18" fill="white" font-family="monospace">
AI • Python • Machine Learning
</text>
</svg>
name: Generate Snake

on:
  schedule:
    - cron: "0 */12 * * *"

  workflow_dispatch:

jobs:
  generate:
    runs-on: ubuntu-latest

    steps:
      - uses: Platane/snk@v3
        with:
          github_user_name: md46-rgb
          outputs: |
            dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v4
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
