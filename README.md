### Hello There!

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=sttormx&layout=demo&theme=dracula)](https://github.com/anuraghazra/github-readme-stats)


[![GitHub followers](https://img.shields.io/github/followers/Sttormx?label=Follow&style=social)](https://github.com/Sttormx/?tab=follow)
[![Instagram Badge](https://img.shields.io/badge/-9jpedro-blue?style=social&logo=Instagram&link=https://www.instagram.com/9jpedro/)](https://www.instagram.com/9jpedro/) 

![Snake animation](https://github.com/sttormx/sttormx/blob/output/github-contribution-grid-snake.svg)
# This is a basic workflow to help you get started with Actions

name: CI

# Controls when the workflow will run
on:
  # Triggers the workflow on push or pull request events but only for the main branch
  push:
    branches: [ main ]
  pull_request:
    branches: [ main ]

  # Allows you to run this workflow manually from the Actions tab
  workflow_dispatch:

# A workflow run is made up of one or more jobs that can run sequentially or in parallel
jobs:
  # This workflow contains a single job called "build"
  build:
    # The type of runner that the job will run on
    runs-on: ubuntu-latest

    # Steps represent a sequence of tasks that will be executed as part of the job
    steps:
      # Checks-out your repository under $GITHUB_WORKSPACE, so your job can access it
      - uses: actions/checkout@v2

      # Runs a single command using the runners shell
      - name: Run a one-line script
        run: echo Hello, world!

      # Runs a set of commands using the runners shell
      - name: Run a multi-line script
        run: |
          echo Add other actions to build,
          echo test, and deploy your project.
