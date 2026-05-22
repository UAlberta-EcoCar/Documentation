# EcoCar Documentation

This repository contains documentation for the EcoCar clube.
It is a [Jekyll] site built using the [Just the Docs] theme, 
and is hosted using GitHub pages here [https://ualberta-ecocar.github.io/Documentation/](https://ualberta-ecocar.github.io/Documentation/)

## Contributing to the docs

Pages are stored in the `/docs` folder.
The documentation is written in Markdown, a simple markup language
to write formatted text. See the [basic syntax](https://www.markdownguide.org/basic-syntax/) to get started.
Some text editors like VSCode have the ability to preview Markdown.

For more advanced features, take a look at the [Just the Docs] documentation.

To preview your changes locally, 
first install [Jekyll] and [Bundler] on your computer:

1.  Run 
    ```sh
    bundle install
    ```
1. Then run 
    ```sh
    bundle exec jekyll serve
    ``` 
    to build your site and preview it at `localhost:4000`.

    The built site is stored in the directory `_site`.

## Licensing and Attribution

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
