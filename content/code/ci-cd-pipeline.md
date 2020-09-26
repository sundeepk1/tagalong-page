---
title: "CI/CD pipeline used by this site"
date: 2019-12-09T13:45:27+01:00

categories: ["DevOps", "Howto"]
tags: ["cicd","circleci","github","hugo"]
---
[![CI/CD chart](/img/ci-cd-chart.png)](/img/ci-cd-chart.png)

This website is built from Markdown files using [Hugo static website generator](https://gohugo.io/) and hosted by [GitHub Pages](https://pages.github.com/), a web hosting service of [GitHub](https://github.com/about) platform.

The CI (continuous integration) part of the pipeline is implemented with Hugo's [built-in webserver mode](https://gohugo.io/commands/hugo_server/). It will watch the files for any changes and automatically rebuild the site on-the-fly, even refreshing the web browser view for the user (this can be disabled).

<!--more-->

The CD (continuous deployment) portion is relying on [Circle CI](https://circleci.com/) online platform which runs a 3-step workflow:

### 1. Build

- Create a Dockerized instance of Hugo tool
- Pull the latest version of the website sources from the `master` branch in the project's GitHub repository
- Generate HTML/JS/CSS content with Hugo and preserve it in temporary storage
- Validate the generated artifacts using `htmlproofer` tool.

### 2. Approve

- Await approval from the maintainer for deployment

### 3. Deploy

- Create a Docker container for GitHub Pages' export tool
- Load the output of the "Build" stage
- Commit these generated files to a reserved `gh-pages` branch in the GitHub repository

Once the contents are loaded into GitHub, they will replace the previous version of the website thus completing the deployment to production environment.
