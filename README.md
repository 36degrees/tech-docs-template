# Tech Docs Template

The Tech Docs Template is a [middleman template][mmt] that
you can use to build technical documentation using a GOV.UK style.

This repo is the template used to generate new sites. The generated site uses HTML, CSS, JS and images from the [tech docs gem](https://github.com/alphagov/tech-docs-gem).

👉 Find out more about the template and its features from the [Tech Docs Template documentation][tdt-docs].

## Before you start

To use the Tech Docs Template you need:

- [Ruby][install-ruby]
- [Middleman][install-middleman]

## Get started

To create a new project using the Tech Docs Template, run:

```sh
middleman init PROJECT_NAME -T alphagov/tech-docs-template
```

where `PROJECT_NAME` is the name of your new project.

This command creates a minimal functional website using the Tech Docs Template.

## Preview your website locally

To preview your new website locally, navigate to your project folder and run:

```sh
bundle exec middleman server
```

👉 See the generated website on `http://localhost:4567` in your browser. Any content changes you make to your website will be updated in real time.

To shut down the Middleman instance running on your machine, use `ctrl+C`

If you make changes to the `config/tech-docs.yml` configuration file, you need to restart Middleman to see the changes.

## Configure your website

The `middleman init` command creates a minimal website with basic configuration.

You can change your website's configuration by editing the `config/tech-docs.yml` file.

👉 See what [configuration options][config] are available.

You can set page-specific options by editing the page's frontmatter.

👉 See how [frontmatter configuration options][frontmatter] are available.

## Adding content

You can add content by editing the `index.html.md.erb` file. These files support content in:

- Markdown
- HTML
- Ruby

👉 For example, you can use Markdown and HTML to [generate different content types][example-content] and [Ruby partials to manage content][partials].

Any file in the `source` folder ending in `.html.md.erb` produces a separate page for your website.

👉 Learn more about [producing more complex page structures][multipage] for your website.

## Contribute

👉 See the [CONTRIBUTE.md file in the tech-docs-gem repository][contribute].

## Licence

Unless stated otherwise, the codebase is released under [the MIT License][mit].
This covers both the codebase and any sample code in the documentation.

The documentation is [© Crown copyright][copyright] and available under the terms of the [Open Government 3.0][ogl] licence.

[mit]: LICENCE
[copyright]: http://www.nationalarchives.gov.uk/information-management/re-using-public-sector-information/uk-government-licensing-framework/crown-copyright/
[ogl]: http://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/
[mmt]: https://middlemanapp.com/advanced/project_templates/
[tdt-docs]: https://tdt-documentation.london.cloudapps.digital
