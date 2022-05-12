


<div align="center">
  <a href="https://github.com/Guilherme-Oliveira-Cunha"></a>
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=Guilherme-Oliveira-   Cunha&show_icons=true&theme=dracula&include_all_commits">
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Guilherme-Oliveira-  Cunha&layout=compact&langs_count=7&theme=dra">
</div>
      
<div style="display: inline_block"><br>
   <h3><b> Tecnologias que estou aprendendo a usar !! </b> <br><br>
   <img align="center" alt="CSS" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/adonisjs/adonisjs-original.svg">
   <img align="center" alt="HTML" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/adonisjs/adonisjs-original.svg">
   <img align="center" alt="PYTHON" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/adonisjs/adonisjs-original.svg">
   <img align="center" alt="MYSQL" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/adonisjs/adonisjs-original.svg">
   <img align="center" alt="DOCKER" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/adonisjs/adonisjs-original.svg">
   <img align="center" alt="POST" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/adonisjs/adonisjs-original.svg">
</div>

<div>
    <a href = "mailto:guilhermejf17@hotmail.com"><img src="https://img.shields.io/badge/-Gmail-%23333?style=for-the-badge&logo=gmail&logoCo>
    <a href="https://www.linkedin.com/in/guilherme-oliveira-python/" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo>
![Snake animation](https://github.com/Guilherme-Oliveira-Cunha/Guilherme-Oliveira-Cunha/blob/output/github-contribution-grid-snake.svg)
</div>
  
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
github_user_name: DevBatista1
svg_out_path: dist/github-contribution-grid-snake.svg
- uses: crazy-max/ghaction-github-pages@v2.1.3
with:
target_branch: output
build_dir: dist
env:
GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
