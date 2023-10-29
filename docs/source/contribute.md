# Contribute to Rosetta
We aim to make Rosetta's libraries and documentation as useful and understandable as possible. If you find any places where we could improve, we'd love to consider your suggestions! To do so - or implement changes yourself - we invite you to do that through our {term}`Git repositories<Repository>`.

## Suggest a feature
???

## Implement a feature
Are you tired of waiting for someone else to fix a bug or add a feature? You can directly contribute to Rosetta by follow these three simple steps:

1. **Set up your environment.** If you haven't done so already, fork off the Rosetta repo of your choice and create your development environment. Details on how you could do this are [described here](project:/start/install.md#get-rosetta-for-development).

2. **Make your contribution.** Make the changes you see fit. You can record changes you make in Git by periodically making **commits**.

3. **Submit your work.** Push your changes to your own branch of Rosetta on GitHub, then submit a **pull request** for your work. By submitting a pull request, you are asking the Rosetta project to *pull* from your work into the project's development branch.

### Enhance our documentation
The documentation for Rosetta (i.e. the source code for this website) consists of Markdown files, HTML templates, and auto-generated compilations of in-code comments brought together using Sphinx.

This means Rosetta treats documentation like code; we see this document as written files that can be tracked and improved upon. Therefore, you can follow [the same steps as code contributions](#implement-a-feature) using [the repo for this document](https://github.com/rosetta-code/rosetta-doc) to contribute to the Rosetta documentation.

Once you set up your local repo for this document's source files, you can elect to manually build a local copy of this Sphinx document by running:

:::{code-block} none
sphinx-build -M html docs/source/ docs/build/
:::

Alternatively, you can automatically rebuild your local copy with every change you make using `sphinx-autobuild`:

:::{code-block} none
sphinx-autobuild docs/source docs/_build/html
:::

## License
Rosetta defines its relationships with its users under the ____ license.

### What you get from Rosetta
???

### What you grant to Rosetta as a contributor
Meanwhile, if you become a contributor to the Rosetta project by submitting a pull request, certain rights and responsibilities will be granted to you, and you will grant the Rosetta project certain permissions in return. Contributors are generally bound by [GitHub's Terms of Service](https://help.github.com/en/github/site-policy/github-terms-of-service#6-contributions-under-repository-license). This policy explicitly grants the Rosetta project an "input=output" policy so that, when you contribute to Rosetta, you agree that:

1. You license your contribution under the same terms as the rest of the Rosetta project, and;

2. You have the right to license your contributions (for example, by being its author).

This practice is the same one as what is used by the Linux Foundation's [Developer Certificates of Origin (DCOs)](https://developercertificate.org/) and [some Contributor License Agreements (CLAs)](https://www.mondaq.com/unitedstates/intellectual-property/807444/what-you-should-know-about-contributor-license-agreements-in-open-source-projects). However, [trade-offs exist for both approaches](https://katedowninglaw.com/2019/02/15/should-i-use-a-developers-certificate-of-origin-or-a-contributor-agreement/), and we believe that neither solution allows for the experience that we prefer for Rosetta.

While DCOs are short and sweet in theory, it requires contributors to [sign off on every Git commit](https://git-scm.com/book/en/v2/Git-Tools-Signing-Your-Work). This can be a quick task in and of itself, but it can also be disproportionately burdensome to new contributors who are unfamiliar with the process. 

On the other hand, we value how a good CLA can explicitly delineate intellectual property (IP) ownership as well as who is responsible if a part of Rosetta turns out to infringe on someone else's IP rights. However, we believe that Rosetta's approach enables those features without the use of [potentially-developer-hostile](https://ben.balter.com/2018/01/02/why-you-probably-shouldnt-add-a-cla-to-your-open-source-project/) contracts.

## Roadmap for Rosetta's future
???