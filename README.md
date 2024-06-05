## Hi there 👋


<a href="https://github.com/MarceloNobrega29">
  <table>
    <tr>
      <td><img height="180" src="https://github-readme-stats.vercel.app/api?username=MarceloNobrega29&show_icons=true&theme=darcula" /></td>
      <td><img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=MarceloNobrega29&layout=compact&theme=darcula" /></td>
    </tr>
  </table>
</a>



<div style="display: inline_block"><br>
  <img align="center" alt="MN-Python" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg">
  <img align="center" alt="MN-Java" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/java/java-original.svg" />       
  <img align="center" alt="MN-HTML" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg">
  <img align="center" alt="MN-CSS" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg">
</div>
 
  ## 
  Sou um estudante de programação iniciante com uma paixão imensa por tecnologia. Desde sempre, a área de TI me fascina e motiva a aprender e crescer profissionalmente. Estou constantemente em busca de novos conhecimentos e habilidades para me tornar um desenvolvedor competente e inovador. Acredito que, com dedicação e perseverança, posso alcançar grandes feitos no mundo da tecnologia.

  
<div>  
  <a href="https://www.instagram.com/ferreir4.nb/" target="_blank"><img src="https://img.shields.io/badge/-Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></a>
  <a href = "mailto:nobregamf29@hotmail.com"><img src="https://img.shields.io/badge/-Gmail-%23333?style=for-the-badge&logo=gmail&logoColor=white" target="_blank"></a>
  <a href="https://www.linkedin.com/in/marcelo-n%C3%B3brega-8046752ba/" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a> 
  
</div>

## Minhas IDEs

<div>
  <img src="https://img.shields.io/badge/Eclipse-2C2255?style=for-the-badge&logo=eclipse&logoColor=white">
  <img src="https://img.shields.io/badge/Visual_Studio_Code-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white"
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
          github_user_name: MarceloNobrega29
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
  
