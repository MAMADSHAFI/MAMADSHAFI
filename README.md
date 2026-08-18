<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:161b22&height=200&section=header&text=MAMAD%20SHAFI&fontSize=70&fontColor=58a6ff&animation=fadeIn&fontAlignY=38&desc=Security%20%7C%20Python%20%7C%20Automation&descAlignY=58&descSize=18" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&pause=1000&color=58A6FF&center=true&vCenter=true&width=600&lines=root%40mamadshafi%3A~%24+whoami;Penetration+Tester+in+Training;Python+%26+Automation+Enthusiast;Always+Learning%2C+Always+Building" alt="Typing SVG" />

<br/>

<img src="https://komarev.com/ghpvc/?username=MAMADSHAFI&label=VISITORS&color=0d1117&style=flat-square" alt="profile views"/>

</div>

---

## `> cat about_me.py`
```python
class AboutMe:
def __init__(self):
self.name     = "Mamad Shafi"
self.role     = "Security Researcher & Python Developer"
self.location = "In Your Heart"
self.focus    = ["Penetration Testing", "Automation", "AI"]
self.learning = ["OWASP Top 10", "NIST Framework", "Advanced Python"]

def say_hi(self):
print("Thanks for dropping by. Let's build something secure.")


me = AboutMe()
me.say_hi()

---

## `> ls ./tech_stack`

<div align="center">

### Languages & Core
<img src="https://skillicons.dev/icons?i=python,bash,js,html,css,cpp&theme=dark" />

### Tools & Platforms
<img src="https://skillicons.dev/icons?i=linux,kali,git,github,docker,vscode,mysql,postman&theme=dark" />

</div>

---

## `> ./stats --show-all`

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=MAMADSHAFI&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&icon_color=58a6ff&text_color=c9d1d9&include_all_commits=true&count_private=true"/>
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=MAMADSHAFI&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=c9d1d9&langs_count=8"/>

<br/><br/>

<img src="https://github-readme-streak-stats.herokuapp.com/?user=MAMADSHAFI&theme=github-dark-blue&hide_border=true&background=0d1117&ring=58a6ff&fire=58a6ff&currStreakLabel=58a6ff" alt="streak"/>

</div>

---

## `> ./contribution_snake`

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/MAMADSHAFI/MAMADSHAFI/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/MAMADSHAFI/MAMADSHAFI/output/github-snake.svg" />
  <img alt="github contribution snake animation" src="https://raw.githubusercontent.com/MAMADSHAFI/MAMADSHAFI/output/github-snake.svg" />
</picture>

<br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=MAMADSHAFI&bg_color=0d1117&color=58a6ff&line=58a6ff&point=c9d1d9&area=true&hide_border=true" width="100%"/>

</div>

---

## `> ssh contact@mamadshafi`

<div align="center">

| Channel | Address |
|:---|:---|
| **Telegram** | [@Mestershafi](https://t.me/Mestershafi) |
| **Instagram** | [mohammad0shafi](https://instagram.com/mohammad0shafi) |
| **Email** | [mohamadpainterghasemi@gmail.com](mailto:mohamadpainterghasemi@gmail.com) |
| **Location** | `In Your Heart` |

<br/>

<a href="https://t.me/Mestershafi"><img src="https://img.shields.io/badge/Telegram-0d1117?style=for-the-badge&logo=telegram&logoColor=58a6ff"/></a>
<a href="https://instagram.com/mohammad0shafi"><img src="https://img.shields.io/badge/Instagram-0d1117?style=for-the-badge&logo=instagram&logoColor=58a6ff"/></a>
<a href="mailto:mohamadpainterghasemi@gmail.com"><img src="https://img.shields.io/badge/Gmail-0d1117?style=for-the-badge&logo=gmail&logoColor=58a6ff"/></a>

</div>

---

<div align="center">


[ EOF ] ── exit code 0 ── connection closed

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:161b22,100:0d1117&height=120&section=footer" width="100%"/>

</div>
`

---

## `.github/workflows/snake.yml`

این فایل انیمیشن مار رو می‌سازه. مسیر و اسم فایل باید **دقیقاً** همین باشه:

```yaml
name: Generate Snake Animation

on:
  schedule:
    - cron: "0 0 * * *"
  workflow_dispatch:
  push:
    branches:
      - main

jobs:
  generate:
    runs-on: ubuntu-latest
    permissions:
      contents: write

    steps:
      - name: Generate snake SVGs
        uses: Platane/snk@v3
        id: snake-gif
        with:
          github_user_name: MAMADSHAFI
          outputs: |
            dist/github-snake.svg
            dist/github-snake-dark.svg?palette=github-dark

      - name: Push to output branch
        uses: crazy-max/ghaction-github-pages@v4
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
