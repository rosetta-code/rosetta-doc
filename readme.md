# Rosetta Documentation

![Rosetta logo](./docs/_build/_static/brand/rosetta-logo-dark.svg)

[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Frosetta-code%2Frosetta-doc.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Frosetta-code%2Frosetta-doc?ref=badge_shield)
[![Documentation Status](https://readthedocs.org/projects/rosetta-doc/badge/?version=latest)](https://rosetta-doc.readthedocs.io/en/latest/?badge=latest)

This repository contains the source files used to auto-generate documentation for Rosetta using Sphinx.

`.vscode/` = Visual Studio Code configurations.

`docs/` = Root that houses the Sphinx source code.

    `source/` = Source files that gets reinterpreted by Sphinx into web-friendly files.

    `make.bat` and `Makefile` = Configuration files to build this documentation.

## Building the document

To render the Sphinx document as HTML files, run the command below.

`sphinx-build -M html docs/source/ docs/build/`

## License

![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Frosetta-code%2Frosetta-doc.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Frosetta-code%2Frosetta-doc?ref=badge_large)
