![Header](./github-header-image.png)

name: Add Badges
on:
  push:
    branches:
      - master
jobs:
  run:
    runs-on: ubuntu-latest
    steps:
      - uses: wow-actions/add-badges@v1
        env:
          repo_url: ${{ github.event.repository.html_url }}
          repo_name: ${{ github.event.repository.name }}
          repo_owner: ${{ github.event.repository.owner.login }}
        with:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
          center: true
          badges: |
            [
              [
                {
                  "badge": "https://img.shields.io/github/license/${{ env.repo_owner }}/${{ env.repo_name }}?style=flat-square",
                  "alt": "MIT License",
                  "link": "${{ env.repo_url }}/blob/master/LICENSE"
                },
                {
                  "badge": "https://img.shields.io/badge/language-TypeScript-blue.svg?style=flat-square",
                  "alt": "Language",
                  "link": "https://www.typescriptlang.org"
                },
                {
                  "badge": "https://img.shields.io/badge/PRs-Welcome-brightgreen.svg?style=flat-square",
                  "alt": "PRs Welcome",
                  "link": "${{ env.repo_url }}/pulls"
                },
                {
                  "badge": "https://img.shields.io/static/v1?label=&labelColor=505050&message=marketplace&color=0076D6&style=flat-square&logo=google-chrome&logoColor=0076D6",
                  "alt": "website",
                  "link": "https://github.com/marketplace/actions/${{ env.repo_name }}"
                }
              ],
              [
                {
                  "badge": "https://img.shields.io/github/workflow/status/${{ env.repo_owner }}/${{ env.repo_name }}/Release/master?logo=github&style=flat-square",
                  "alt": "build",
                  "link": "${{ env.repo_url }}/actions/workflows/release.yml"
                },
                {
                  "badge": "https://img.shields.io/lgtm/grade/javascript/g/${{ env.repo_owner }}/${{ env.repo_name }}.svg?logo=lgtm&style=flat-square",
                  "alt": "Language grade: JavaScript",
                  "link": "https://lgtm.com/projects/g/${{ env.repo_owner }}/${{ env.repo_name }}/context:javascript"
                }
              ]
            ]
- 👀 I’m interested in Geology, Geophysics, Geotechnical Engineering, Data Science and Web development.

- 💻 Passionate in Data Science, Web application development and Open Source contributor

- 🌱 I’m currently learning Machine learning with Python, Frontend dev: HTML/CSS/JavaScript "React" and Backend dev with Python "streamlib & Flask".

- 💞️ I’m looking to collaborate on Datascience Web application proejcts.

- 📊 All of my projects are available [here](https://github.com/Noctax?tab=repositories)

- 💬 Don't hesitate to contact me


<!---
Noctax/Noctax is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
