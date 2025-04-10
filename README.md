<h1 align="center">Hi 👋, I'm [Your Name]</h1>




  
  

  <p align="left" style="margin-bottom: 20px;"><img src="https://komarev.com/ghpvc/?username=FarhanAlam-Official&label=Profile%20views&color=0e75b6&style=flat" alt="FarhanAlam-Official" /></p>






  
  
  
  

  <h3 align="left" style="margin-bottom: 10px;">Connect with me:</h3>










  <p align="left" style="margin-bottom: 20px;">

  </p>



















<hr style="width: 80%; margin: 30px auto;">
<h3 align="left" style="margin-bottom: 10px;">GitHub Stats:</h3>









<p>
<img align="center" src="https://github-readme-stats.vercel.app/api?username=FarhanAlam-Official&show_icons=true&locale=en&theme=default&show_icons=true&count_private=true" alt="FarhanAlam-Official" />
</p>









<p>
<img align="center" src="https://github-readme-stats.vercel.app/api/top-langs?username=FarhanAlam-Official&show_icons=true&locale=en&layout=compact&theme=default" alt="FarhanAlam-Official" />
</p>









<p>
<img align="center" src="https://github-readme-streak-stats.herokuapp.com/?user=FarhanAlam-Official&theme=default" alt="FarhanAlam-Official" />
</p>

















<hr style="width: 80%; margin: 30px auto;">
<h3 align="left" style="margin-bottom: 10px;">Pac-Man Contribution Graph:</h3>









<div align="center">
  <!-- Pac-Man contribution graph animation -->
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/FarhanAlam-Official/FarhanAlam-Official/output/pacman-contribution-graph-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/FarhanAlam-Official/FarhanAlam-Official/output/pacman-contribution-graph.svg">
    <img alt="pacman contribution graph" src="https://raw.githubusercontent.com/FarhanAlam-Official/FarhanAlam-Official/output/pacman-contribution-graph.svg">
  </picture>

  <!-- Note: The animation above will only work after you set up the GitHub Action workflow on your profile repository. -->
  <!-- For preview purposes, here's an example of what it will look like: -->
  <img src="https://raw.githubusercontent.com/abozanona/abozanona/output/pacman-contribution-graph-dark.svg" alt="Example Pac-Man Contribution Graph" style="display: block; margin-top: 20px; width: 100%;" />

  <p><em>generated with <a href="https://abozanona.github.io/pacman-contribution-graph/">abozanona/pacman-contribution-graph</a></em></p>
  <p><strong>Note:</strong> The animation will only appear after you set up the GitHub Action workflow on your profile repository.</p>

  <!-- Setup instructions -->
  <details>
    <summary><b>🔍 Click here for instructions to set up this Pac-Man animation on your profile</b></summary>
    <br/>
    <p>To get this working on your profile:</p>
    <ol>
      <li>Create a new repository with the same name as your GitHub username</li>
      <li>Create a <code>.github/workflows</code> directory in your repository</li>
      <li>Create a file named <code>pacman.yml</code> with the following content:</li>
    </ol>

    <pre>
name: Generate Pac-Man Game

on:
  schedule:
    - cron: "0 0 * * *" # Runs daily at midnight UTC
  workflow_dispatch: # Allows manual triggering
  push:
    branches:
      - main

jobs:
  generate:
    permissions:
      contents: write
    runs-on: ubuntu-latest
    timeout-minutes: 5
    steps:
      - name: Generate Pac-Man Contribution Graph
        uses: abozanona/pacman-contribution-graph@main
        with:
          github_user_name: ${{ github.repository_owner }}
      - name: Push to Output Branch
        uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
    </pre>

    <p>Then add this to your README.md:</p>

    <pre>
&lt;picture&gt;
  &lt;source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/FarhanAlam-Official/FarhanAlam-Official/output/pacman-contribution-graph-dark.svg"&gt;
  &lt;source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/FarhanAlam-Official/FarhanAlam-Official/output/pacman-contribution-graph.svg"&gt;
  &lt;img alt="pacman contribution graph" src="https://raw.githubusercontent.com/FarhanAlam-Official/FarhanAlam-Official/output/pacman-contribution-graph.svg"&gt;
&lt;/picture&gt;

_generated with [abozanona/pacman-contribution-graph](https://abozanona.github.io/pacman-contribution-graph/)_
    </pre>

    <p>The code above will automatically use your GitHub username (<code>FarhanAlam-Official</code>) when you set up the workflow.</p>

    <p>Alternatively, you can use the JavaScript approach:</p>

    <pre>
&lt;script type="module"&gt;
import { PacmanRenderer } from 'https://cdn.jsdelivr.net/npm/pacman-contribution-graph/dist/pacman-contribution-graph.min.js';
const pr = new PacmanRenderer({
    platform: 'github',
    username: 'FarhanAlam-Official',
    canvas: document.getElementById('canvas'),
    outputFormat: 'canvas',
    gameTheme: 'github'
});
pr.start();
&lt;/script&gt;
    </pre>

    <p>Make sure to add a canvas element: <code>&lt;canvas id="canvas"&gt;&lt;/canvas&gt;</code> to your page. The code above will use your GitHub username (<code>FarhanAlam-Official</code>).</p>
  </details>
</div>









