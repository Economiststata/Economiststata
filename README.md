## Hola a todos 👋

:computer: 
##  Economista Independiente 

###  Vías de contacto
Correo: ronald.rosa96@gmail.com

⚡ Recent Activity

<!--START_SECTION:activity-->

<!--END_SECTION:activity-->

update_readme.yml

name: Update README

on:

schedule:

- cron: '0 */12 * * *' #

workflow_dispatch:

jobs:

build:

name: Update this repo's README with recent activity

runs-on: ubuntu-latest

permissions:

contents: write

steps:

- uses: actions/checkout@v4

- uses: jamesgeorge007/github-activity-readme@master

env:

GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
