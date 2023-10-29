The documentation for Rosetta consists of Markdown files, HTML templates, and auto-generated compilations of in-code comments brought together using Sphinx.

## Build the document
You can recreate the environment used to generate this document by using our Pip requirements file or Conda environment file. Then, you can elect to manually build a local copy of this Sphinx document by running:

`sphinx-build -M html docs/source/ docs/build/`

Alternatively, you can automatically rebuild your local copy with every change you make using `sphinx-autobuild`:

`sphinx-autobuild docs/source docs/_build/html`

**For more information including how you can suggest edits, please take a look at the live documentation.**