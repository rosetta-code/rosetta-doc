# Rosetta Documentation

![Rosetta logo](./docs/source/_static/brand/rosetta-logo-dark.png)
[![Codacy code quality assurance grade](https://app.codacy.com/project/badge/Grade/bd9c47a3f878470dab5c8450d8beb74a)](https://app.codacy.com/gh/rosetta-code/rosetta-doc/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
[![FOSSA license compliance status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Frosetta-code%2Frosetta-doc.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Frosetta-code%2Frosetta-doc?ref=badge_shield)
[![ReadTheDocs documentation build status](https://readthedocs.org/projects/rosetta-doc/badge/?version=latest)](https://rosetta-doc.readthedocs.io/en/latest/?badge=latest)
[![All Contributors](https://img.shields.io/github/all-contributors/rosetta-code/rosetta-doc?color=ee8449)](#contributors)

This repository contains source files used to auto-generate documentation for Rosetta using Sphinx.

## Contents of this repository

- `.vscode/` = Visual Studio Code configurations.
- `docs/` = Root that houses the Sphinx source code.
  - `source/` = Source files that gets reinterpreted by Sphinx into web-friendly files.
  - `make.bat` and `Makefile` = Configuration files to build this documentation.
- `pyproject.toml`, `.gitignore`, `.prettierignore`, `.all-contributorsrc`, and `.readthedocs.yaml` = Additional configurations for Git, Prettier (code auto-reformatting), all-contributors (attribution of contributors), and ReadTheDocs (web provider for the live version of this documentation).
- `requirements.txt` and `environment.yml` = Packages to recreate the development environment for this documentation using Pip and Conda respectively.

## Locally building the document

To render the Sphinx document as HTML files, run the command below.

`sphinx-build -M html docs/source/ docs/build/`

## License

See the attached license file for more information. License term compliance is inspected using FOSSA:

[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Frosetta-code%2Frosetta-doc.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Frosetta-code%2Frosetta-doc?ref=badge_large)

## Contributors

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tbody>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://keitaay.com/"><img src="https://avatars.githubusercontent.com/u/35097043?v=4?s=100" width="100px;" alt="Keita Yokoyama"/><br /><sub><b>Keita Yokoyama</b></sub></a><br /><a href="https://github.com/rosetta-code/rosetta-doc/commits?author=keitaay" title="Code">💻</a> <a href="https://github.com/rosetta-code/rosetta-doc/commits?author=keitaay" title="Documentation">📖</a> <a href="#a11y-keitaay" title="Accessibility">️️️️♿️</a> <a href="#business-keitaay" title="Business development">💼</a> <a href="#content-keitaay" title="Content">🖋</a> <a href="#design-keitaay" title="Design">🎨</a> <a href="#ideas-keitaay" title="Ideas, Planning, & Feedback">🤔</a> <a href="#infra-keitaay" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#projectManagement-keitaay" title="Project Management">📆</a> <a href="#tool-keitaay" title="Tools">🔧</a></td>
    </tr>
  </tbody>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->
