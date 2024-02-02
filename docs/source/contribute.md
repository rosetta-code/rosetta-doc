# Contribute to Rosetta

We aim to make Rosetta's libraries and documentation as useful and understandable as possible. If you find any places where we could improve, we'd love to consider your suggestions! To do so - or implement changes yourself - we invite you to do that through our {term}`Git repositories<Repository>`.

## Suggest a feature

???

## Report a bug

???

## Implement a feature

Are you tired of waiting for someone else to fix a bug or add a feature? You can directly contribute to Rosetta by following these three simple steps:

1. **Set up your environment.** If you haven't done so already, {term}`fork<Fork>` off the Rosetta repo of your choice and create your development environment. The section describing how to install Rosetta contains [a walkthrough on how to do this](project:/start/install.md#get-rosetta-for-development).

2. **Make your contribution.** Make the changes you see fit. You can record changes you make in Git by periodically making {term}`commits<Commit>`.

3. **Submit your work.** {term}`Push` your changes to your own {term}`fork<Fork>` of Rosetta on GitHub, then submit a {term}`pull request<Pull request>` for your work.

There are some additional steps to keep in mind if your contribution involves creating a new {term}`Adapter` or our documentation. Please take a look at the additional guidance below:

### Create a new Adapter

???

### Enhance our documentation

The documentation for Rosetta (i.e. the source code for this website) consists of Markdown files, HTML templates, and auto-generated compilations of in-code comments brought together using Sphinx.

This means Rosetta treats documentation like code; we see this document as written files that can be tracked and improved upon. Therefore, you can follow [the same steps as code contributions](#implement-a-feature) using [the repo for this document](https://github.com/rosetta-code/rosetta-doc) to contribute to the Rosetta documentation.

Once you set up your local repo for this document's source files, you can elect to manually build a local copy of this Sphinx document by running:

:::{code-block} none
sphinx-build -M html docs/source/ docs/build/
:::

Alternatively, you can automatically rebuild your local copy with every change you make using `sphinx-autobuild`:

:::{code-block} none
sphinx-autobuild docs/source docs/\_build/html
:::

## License


## Roadmap for Rosetta's future
???