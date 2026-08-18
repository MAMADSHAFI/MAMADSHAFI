<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:00ff41&height=200&section=header&text=MAMADSHAFI&fontSize=60&fontColor=00ff41&fontAlignY=38&desc=Developer%20%7C%20Security%20%7C%20Embedded&descAlignY=60&descSize=18&descColor=39d353" width="100%"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=18&duration=3000&pause=800&color=00FF41&center=true&vCenter=true&multiline=true&width=600&height=120&lines=~/developer+%24+cat+profile.txt;01+%3E+AI+Developer;02+%3E+Cybersecurity+Enthusiast;03+%3E+Desktop+%26+Web+Developer;04+%3E+Embedded+Systems+Explorer)](https://git.io/typing-svg)

</div>

---

## `> about_me.py`
```python
class AboutMe:
def __init__(self):
self.name     = "Mohammad Shafi"
self.alias    = "MAMADSHAFI"
self.location = "In Your Heart 💚"
self.focus    = ["AI Development", "Cybersecurity", "Embedded Systems"]
self.goal     = "Build things that matter and leave traces in the code"

def say_hi(self):
print("Thanks for visiting — hope you find something useful here.")
print(f"Currently focused on: {', '.join(self.focus)}")
print("Let's build the future together. 🚀")

me = AboutMe()
me.say_hi()

---

## `> contact.sh`

<div align="center">

[![Telegram](https://img.shields.io/badge/Telegram-@Mestershafi-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/Mestershafi)
[![Instagram](https://img.shields.io/badge/Instagram-mohammad0shafi-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/mohammad0shafi)
[![Email](https://img.shields.io/badge/Email-Contact_Me-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:mohamadpainterghasemi@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-MAMADSHAFI-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/MAMADSHAFI)

</div>

---

## `> tech_stack.json`

<div align="center">

[![My Skills](https://skillicons.dev/icons?i=python,c,cpp,linux,bash,git,github,vscode,arduino,raspberrypi,html,css,js,mysql&theme=dark&perline=7)](https://skillicons.dev)

</div>

---

## `> github_stats.sh`

<div align="center">

<img height="180em" src="https://github-readme-stats.vercel.app/api?username=MAMADSHAFI&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=00ff41&icon_color=39d353&text_color=c9d1d9&include_all_commits=true&count_private=true"/>

<img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=MAMADSHAFI&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=00ff41&text_color=c9d1d9&langs_count=8"/>

</div>

<div align="center">

[![GitHub Streak](https://streak-stats.demolab.com?user=MAMADSHAFI&theme=github-dark-blue&hide_border=true&background=0D1117&ring=00FF41&fire=39D353&currStreakLabel=00FF41&sideLabels=C9D1D9&dates=6E7681)](https://git.io/streak-stats)

</div>

---

## `> contribution_snake.gif`

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/MAMADSHAFI/MAMADSHAFI/output/github-contribution-grid-snake-dark.svg"/>
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/MAMADSHAFI/MAMADSHAFI/output/github-contribution-grid-snake.svg"/>
  <img alt="snake animation" src="https://raw.githubusercontent.com/MAMADSHAFI/MAMADSHAFI/output/github-contribution-grid-snake-dark.svg"/>
</picture>

</div>

---

## `> activity_graph.sh`

<div align="center">

[![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=MAMADSHAFI&theme=github-compact&bg_color=0d1117&color=00ff41&line=39d353&point=00ff41&hide_border=true)](https://github.com/ashutosh00710/github-readme-activity-graph)

</div>

---

<div align="center">

console
$ git commit -m "First, solve the problem. Then, write the code."

![Profile Views](https://komarev.com/ghpvc/?username=MAMADSHAFI&color=00ff41&style=flat-square&label=PROFILE+VIEWS)

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00ff41,100:0d1117&height=120&section=footer" width="100%"/>


---

## `.github/workflows/snake.yml` — نسخه کامل‌شده

```yaml
name: Generate Snake Animation

on:
  schedule:
    - cron: "0 0 * * *"
  workflow_dispatch:
  push:
    branches: [main, master]

jobs:
  generate:
    runs-on: ubuntu-latest
    timeout-minutes: 10
    permissions:
      contents: write

    steps:
      - uses: Platane/snk@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark

      - uses: crazy-max/ghaction-github-pages@v3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
