# Contribute to Rosetta

We aim to make Rosetta's libraries and documentation as useful and understandable as possible. If you find any places where we could improve, we'd love to consider your suggestions! To do so - or implement changes yourself - we invite you to do that through our {term}`Git repositories<Repository>`.

## Report a problem

You might be frustrated with something "going wrong" with Rosetta, and you may want to ask for help. You can ask for support in two different ways depending on the kind of help you want.

**If you need help with using Rosetta correctly**, you can ask other users for advice in [Rosetta's discussion area](https://github.com/orgs/rosetta-code/discussions/new?category=q-a). The form will ask you several questions that could help other users understand your work, and reproduce or solve it as needed.

**If you think there is a problem with Rosetta**, each Rosetta repo has its own Bug Report form. The forms will ask you several questions that will help others reproduce your problem and potentially find solutions.

## Suggest a feature

If you have ideas for new features that you'd like to see in Rosetta, tell the world about it in [the project discussion area](https://github.com/orgs/rosetta-code/discussions/new?category=ideas) on Rosetta's GitHub page.

## Implement a feature

Are you tired of waiting for someone else to fix a bug or add a feature? You can directly contribute to Rosetta by following these three simple steps:

1. **Set up your environment.** If you haven't done so already, {term}`fork<Fork>` off the Rosetta repo of your choice and create your development environment. The section describing how to install Rosetta contains [a walkthrough on how to do this](project:/develop.md).

2. **Make your contribution.** Make the changes you see fit. You can record changes you make in Git by periodically making {term}`commits<Commit>` to your local repo.

3. **Submit your work.** {term}`Push` your changes to your own {term}`fork<Fork>` of Rosetta on GitHub, then submit a {term}`pull request<Pull request>` for your work. To have your pull request accepted, you will need to:

    1. Make a valid push to a `dev` or feature branch

    2. Describe the change that you proposed and why it's helpful

    3. Pass a license compliance test automatically performed by FOSSA

    4. *Unless you're changing documentation:* Pass tests to make sure that your code doesn't break things

    5. *Main branch releases only:* pass a security test automatically performed by Snyk

    6. Receive approval of your push from a Rosetta moderator

% There are some additional steps to keep in mind if your contribution involves creating a new {term}`Adapter` or our documentation. Please take a look at the additional guidance below:
%
% ### Create a new Adapter
%
% ???

### Enhance our documentation

The documentation for Rosetta (i.e. the source code for this website) consists of Markdown files, HTML templates, and auto-generated compilations of in-code comments brought together using Sphinx.

This means Rosetta treats documentation like code; we see this document as written files that can be tracked and improved upon. Therefore, you can contribute to [the repo for this document](https://github.com/rosetta-code/rosetta-doc) by following [the same steps as code contributions](#implement-a-feature).

Once you set up your local repo for this document's source files, you can manually build a copy of this Sphinx document by running:

:::{code-block} none
sphinx-build -M html docs/source/ docs/build/
:::

Alternatively, you can automatically rebuild your local copy with every change you make using `sphinx-autobuild`:

:::{code-block} none
sphinx-autobuild docs/source docs/_build/html
:::

If you decide to suggest changes to the Rosetta documentation, please remember to follow [our project's principles](project:./principles.md) and [our style guide](project:./style.md).

## License

Rosetta defines its relationships with its users through license files in each repository. We describe our licenses and how they relate to the Rosetta project's belief in [the page on our core principles](project:./principles.md).
