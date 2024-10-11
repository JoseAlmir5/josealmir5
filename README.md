## Seja Bem-Vindo ao meu perfil! Venha me conhecer um pouco.

- 💻 Desenvolvedor Front-end
- 📚 Cursando Analise e desenvolvimento de sistemas
- 🌱 Estudando e me aprofundando em JavaScript

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=josealmir5&show_icons=true&theme=calm)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=josealmir5&layout=compact&theme=calm)


<div>
<img height="45" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original.svg" />
<img height="45" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original.svg" />
<img height="45" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/javascript/javascript-original.svg" />
</div>        

![Snake animation]([https://github.com/JoseAlmir5/josealmir5/edit/main/README.md](https://github.com/JoseAlmir5))

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
         github_user_name: rafaballerini
        svg_out_path: dist/github-contribution-grid-snake.svg

  - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
