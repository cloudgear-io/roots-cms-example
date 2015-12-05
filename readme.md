# Roots + netlify CMS

This is a simple example of how to integrate netlify CMS with a roots based site.

It's based on Brian Rinaldi's great [Static Site Samples](https://github.com/remotesynth/Static-Site-Samples) and meant as a simple example of how to hook netlify CMS up with a roots based site.

## Setting up

Make sure to install the [netlify-git-api](https://github.com/netlify/netlify-git-api) before you start.

Then:

```bash
git clone https://github.com/netlify-templates/hexo-cms-example.git
cd roots-cms-example
netlify-git-api users add
netlify-git-api serve
```

Open a separate terminal window and run:

```bash
npm install
roots watch
```

## Using

Visit [localhost:4000](http://localhost:4000/) to browser the site.

Visit [localhost:4000/admin](http://localhost:4000/admin) to use the CMS.

To run against the GitHub API in production, edit the production backend settings for `admin/config.yml` with the correct repository and branch.

Then run:

```bash
CMS_ENV=production roots watch
```
