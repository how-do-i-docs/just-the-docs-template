<p align="center">
  <a href="https://howdoidocs.tech">
    <img src="https://github.com/how-do-i-docs/design/raw/main/assets/howdoidocs-logo-bg.svg" height="96">
    <h1 align="center">How Do I Docs? — Docs Site Template</h1>
  </a>
</p>

<h3 align="center">
  A quick-and-easy template for spinning up a bare minimum documentation site, powered by <a href="https://just-the-docs.github.io/just-the-docs/">Just the Docs</a>!
</h3>

<p align="center">
    <a href="https://github.com/how-do-i-docs/site"><strong>Site Source</strong></a>  ·
    <a href="https://github.com/how-do-i-docs/design"><strong>Design</strong></a>  ·
  <a href="https://docs.howdoidocs.tech"><strong>Documentation</strong></a> ·
  <a href="https://github.com/how-do-i-docs/doc-templates"><strong>Templates</strong></a>
</p>
<br/>

## Overview

This is a *bare-minimum* template to create a [Jekyll] site that:

- uses the [Just the Docs] theme;
- can be built and published on [GitHub Pages];
- can be built and previewed locally, and published on other platforms.

More specifically, the created site:

- uses a gem-based approach, i.e. uses a `Gemfile` and loads the `just-the-docs` gem;
- uses the [GitHub Pages / Actions workflow] to build and publish the site on GitHub Pages.

To get started with creating a site, simply:

1. click "[use this template]" to create a GitHub repository
2. go to Settings > Pages > Build and deployment > Source, and select GitHub Actions

If you want to maintain your docs in the `docs` directory of an existing project repo, see [Hosting your docs from an existing project repo](#hosting-your-docs-from-an-existing-project-repo).

After completing the creation of your new site on GitHub, update it as needed:

## Replace the content of the template pages

Update the following files to your own content:

- `index.md` (your new home page)
- `README.md` (information for those who access your site repo on GitHub)

## Publishing your site on GitHub Pages

1.  If your created site is `YOUR-USERNAME/YOUR-SITE-NAME`, update `_config.yml` to:

    ```yaml
    title: YOUR TITLE
    description: YOUR DESCRIPTION
    theme: just-the-docs

    url: https://YOUR-USERNAME.github.io/YOUR-SITE-NAME

    aux_links: # remove if you don't want this link to appear on your pages
      Template Repository: https://github.com/YOUR-USERNAME/YOUR-SITE-NAME
    ```

2.  Push your updated `_config.yml` to your site on GitHub.

3.  In your newly created repo on GitHub:
    - go to the `Settings` tab -> `Pages` -> `Build and deployment`, then select `Source`: `GitHub Actions`.
    - if there were any failed Actions, go to the `Actions` tab and click on `Re-run jobs`.

## Building and previewing your site locally

Assuming [Jekyll] and [Bundler] are installed on your computer:

1.  Change your working directory to the root directory of your site.

2.  Run `bundle install`.

3.  Run `bundle exec jekyll serve` to build your site and preview it at `localhost:4000`.

    The built site is stored in the directory `_site`.

## Publishing your built site on a different platform

Just upload all the files in the directory `_site`.

## Customization

You're free to customize sites that you create with this template, however you like!

[Browse our documentation][Just the Docs] to learn more about how to use this theme.


## Additional Resources

- [Site Repository](https://github.com/how-do-i-docs/site)
- [Design Repository](https://github.com/how-do-i-docs/design)
- [Templates Repository](https://github.com/how-do-i-docs/doc-templates)
- [Documentation Site](https://docs.howdoidocs.tech)

## Credits

- Logo based on writing emoji from [OpenMoji](https://openmoji.org)
- Interface font used is Rasmus Andersson's [Inter](https://rsms.me/inter/)
- Substantial content pulled from [The Good Docs Project](https://thegooddocsproject.dev)
- Documentation site template is from [Just the Docs](https://github.com/just-the-docs/just-the-docs)

## Terms of use

This repository is licensed under the [MIT License]. You are generally free to reuse or extend upon this code as you see fit; just include the original copy of the license (which is preserved when you "make a template"). While it's not necessary, we'd love to hear from you if you do use this template, and how we can improve it for future use!

The deployment GitHub Actions workflow is heavily based on GitHub's mixed-party [starter workflows]. A copy of their MIT License is available in [actions/starter-workflows].

----

[^1]: [It can take up to 10 minutes for changes to your site to publish after you push the changes to GitHub](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll#creating-your-site).

[Jekyll]: https://jekyllrb.com
[Just the Docs]: https://just-the-docs.github.io/just-the-docs/
[GitHub Pages]: https://docs.github.com/en/pages
[GitHub Pages / Actions workflow]: https://github.blog/changelog/2022-07-27-github-pages-custom-github-actions-workflows-beta/
[Bundler]: https://bundler.io
[use this template]: https://github.com/just-the-docs/just-the-docs-template/generate
[`jekyll-default-layout`]: https://github.com/benbalter/jekyll-default-layout
[`jekyll-seo-tag`]: https://jekyll.github.io/jekyll-seo-tag
[MIT License]: https://en.wikipedia.org/wiki/MIT_License
[starter workflows]: https://github.com/actions/starter-workflows/blob/main/pages/jekyll.yml
[actions/starter-workflows]: https://github.com/actions/starter-workflows/blob/main/LICENSE
