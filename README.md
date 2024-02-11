# Rosetta Documentation

<div style="text-align:center;"><img style="width:100%; max-width:200px" src="./docs/source/_static/brand/rosetta-logo-dark.svg"></div>

[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Frosetta-code%2Frosetta-doc.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Frosetta-code%2Frosetta-doc?ref=badge_shield)
[![Documentation Status](https://readthedocs.org/projects/rosetta-doc/badge/?version=latest)](https://rosetta-doc.readthedocs.io/en/latest/?badge=latest)
[![All Contributors](https://img.shields.io/github/all-contributors/rosetta-code/rosetta-doc?color=ee8449)](#contributors)

This repository contains the source files used to auto-generate documentation for Rosetta using Sphinx.

## Contents of this Repository

- `.vscode/` = Visual Studio Code configurations.
- `docs/` = Root that houses the Sphinx source code.
  - `source/` = Source files that gets reinterpreted by Sphinx into web-friendly files.
  - `make.bat` and `Makefile` = Configuration files to build this documentation.
- `pyproject.toml`, `.gitignore`, `.prettierignore`, and `.readthedocs.yaml` = Additional configurations for Git, Prettier (code auto-reformatting), and ReadTheDocs (web provider for the live version of this documentation).
- `requirements.txt` and `environment.yml` = Packages to recreate the development environment for this documentation using Pip and Conda respectively.

## Building the document

To render the Sphinx document as HTML files, run the command below.

`sphinx-build -M html docs/source/ docs/build/`

## License

See the attached license file for more information.

[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Frosetta-code%2Frosetta-doc.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Frosetta-code%2Frosetta-doc?ref=badge_large)

## Contributors

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tbody>
    <tr>
      <td align="center" valign="top" width="14.28%"><img src="https://avatars.githubusercontent.com/u/35097043?v=4?s=100" width="100px;" alt="Kéita A. Yokoyama"/><br /><sub><b>Kéita A. Yokoyama</b></sub></a><br /><a href="https://github.com/all-contributors/all-contributors/commits?author=keitaay" title="Documentation">📖</a></td>
    </tr>
  </tbody>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

Rosetta follows the [all-contributors](https://allcontributors.org) specification to provide credit in its repository. [Many types of contributions](https://allcontributors.org/docs/en/emoji-key) are welcomed - even if they don't involve any sort of scientific developments or coding!
