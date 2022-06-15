# Gatsby Starter Resume CMS

[![Netlify Status](https://api.netlify.com/api/v1/badges/a17204d8-649d-4817-903b-378bb79d7299/deploy-status)](https://app.netlify.com/sites/gatsby-starter-resume/deploys)

![resume-template](./preview.png "Gatsby resume template")


Gatsby Starter Resume CMS is a free starter template with  Netlify CMS as headless CMS. It is easy to customize the design with thanks to tailwind theming capabilities. It uses git as a backend and can be deployed to any static hosting service like Netlify, firebase hosting or Github pages.

[Demo](https://gatsby-starter-resume.netlify.app)

## Features

- One-page resume/CV
- PWA
- node.js
- Multiple Netlify CMS widgets
- Netlify CMS as Headless CMS
- Tailwind for styling with theming
- Optimized build process
- Basic SEO, site metadata
- Prettier
- Social media links
- Puppeter
- Generate PDF File

## Quick Start

### Create a Gatsby site

Use the Gatsby CLI to create a new site, specifying the resume starter.

```shell
# create a new Gatsby site using the blog starter
gatsby new my-resume https://github.com/george-barbu-cc
```

### Start developing

Navigate into your new site’s directory and start it up.

```shell
cd my-resume/
gatsby develop
```

## Updating Content

The resume content is generated from `data/profile.json` file. You can manually edit this file or setup Netlify CMS for online editing.

### Netlify CMS as Headless CMS

To use Netlify CMS  you’ll need to deploy to Netlify through GitHub, Gitlab or Bitbucket, set up continuous deployment, and do a few configuration. For Github:

Open `static/admin/config.yml`. Replace `george-barbu-cc/resume` with your GitHub username and project name. This step is important for managing and deploying the Netlify CMS interface.

```yaml
backend:
  name: github
  repo: george-barbu-cc/resume #TODO replace this with your own repo
```

Publish your repo to Github, then, open [Netlify](app.netlify.com) and add a “New site from Git”. Choose your newly created repo and click on “Deploy site” with the default deployment settings.

Finally need to set up an OAuth application on GitHub. Start development build with `gatsby develop` and visit `http://localhost:8000/admin` and authorize Netlify to make commits for you.

If it doesn't work, the instructions for setting up OAuth can be found here: [Netlify’s Using an Authorization Provider](https://www.netlify.com/docs/authentication-providers/#using-an-authentication-provider).
