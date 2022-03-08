# Olá, sou Ruan! :D
<div>
  <a href="https://github.com/RSG27/github-readme-stats">
    <img  height="180em" align="center" src="https://github-readme-stats.vercel.app/api?username=RSG27&show_icons=true&theme=shades-of-purple" />
    <img height="180em" align="center" src="https://github-readme-stats.vercel.app/api/top-langs/?username=RSG27&layout=compact&theme=shades-of-purple" />
</div>

<div style: "display: inline-block;"><br>
<img align="center" alt="Ruan-HTML" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" />
<img align="center" alt="Ruan-CSS" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" />
<img align="center" alt="Ruan-CSS" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-plain.svg" />
<img align="center" alt="Ruan-CSS" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" />
</div>


# Sobre mim

🙏 Espiritualidade acima de tudo

💻 Estudando HTML5, CSS3 e Javascript (Front-end)
<br>

# Redes Sociais

[![Linkedin Badge](https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/ruan-silva-gaspar-a13a89226/)](https://www.linkedin.com/in/ruan-silva-gaspar-a13a89226/)

# Editor de Código - VSCode

<img height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" alt="Ruan_VSCode" />
  
<br>
  
name: Generate Datas

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:

jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: devemdobro
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
