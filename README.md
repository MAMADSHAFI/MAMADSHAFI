<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=28&pause=1000&color=00FF9C&center=true&vCenter=true&width=600&lines=Hi%2C+I'm+Mohammad+Shafi;AI+Developer+%7C+Cybersecurity;Welcome+to+my+terminal+%F0%9F%91%BE" alt="banner" />

</div>

---

## `> about_me.py`
```python
class AboutMe:
def __init__(self):
self.name = "Mohammad Shafi"
self.alias = "MAMADSHAFI"
self.focus = ["AI Development", "Cybersecurity", "Embedded Systems"]
self.goal = "Build things that matter and leave traces in the code"

def say_hi(self):
print("Thanks for visiting — hope you find something useful here.")
print(f"Currently focused on: {', '.join(self.focus)}")
print("Let's build the future together.")


me = AboutMe()
me.say_hi()

---

## `> contact.sh`

<div align="center">

[![Telegram](https://img.shields.io/badge/Telegram-%40Mestershafi-229ED9?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/Mestershafi)
[![Instagram](https://img.shields.io/badge/Instagram-mohammad0shafi-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/mohammad0shafi)
[![Email](https://img.shields.io/badge/Email-Contact-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:mohamadpainterghasemi@gmail.com)

</div>

---

## `> tech_stack.json`

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)

</div>

---

## `> github_stats.sh`

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=MAMADSHAFI&show_icons=true&theme=dark&hide_border=true&bg_color=0D1117&title_color=00FF9C&icon_color=00FF9C" alt="stats" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=MAMADSHAFI&layout=compact&theme=dark&hide_border=true&bg_color=0D1117&title_color=00FF9C" alt="top langs" />

</div>

---

## `> contribution_snake.gif`

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/MAMADSHAFI/MAMADSHAFI/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/MAMADSHAFI/MAMADSHAFI/output/github-snake.svg" />
  <img alt="snake animation" src="https://raw.githubusercontent.com/MAMADSHAFI/MAMADSHAFI/output/github-snake.svg" />
</picture>

</div>

---

<div align="center">

![Profile Views](https://komarev.com/ghpvc/?username=MAMADSHAFI&style=for-the-badge&color=00FF9C&label=PROFILE+VIEWS)

</div>
`

## ۲) فایل `.github/workflows/snake.yml` — این کد YAML رو اینجا بذار، نه توی README

مشکل بزرگ‌تر اینه که YAML قبلی هم غلط بود؛ `on:` نداشت و `outputs` بد نوشته شده بود. این نسخه‌ی درست رو جایگزین کن:

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
    timeout-minutes: 10
    permissions:
      contents: write
    steps:
      - name: Generate snake SVGs
        uses: Platane/snk@v3
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
