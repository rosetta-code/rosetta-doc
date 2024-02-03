# Style guide

Coding, comments, and documentation for Rosetta can quickly become overwhelming or inconsistent. These rules and guidelines aim to create standard expectations that fit [our community's principles](project:./principles.md).

## General ideas

- **Use American English.** Variables should be named and spelled in American English according to the latest edition of [Webster's Dictionary](https://www.merriam-webster.com/).

- **Use serial commas,** also called Oxford commas.

- **Refer to Google's Developer Documentation Style Guide.** If this document doesn't answer a question you have, look at [Google's developer document style guide](https://developers.google.com/style).

- **Break the rules when it's necessary.** In certain cases, your content may be easier to use or understand if you _don't_ follow the guidelines in this document. You should depart from them in those specific instances. However, you should also be prepared if anyone asks why you made that decision.

## Coding style

### Datatypes

UTF-8 everywhere

### Naming conventions

Please follow the rules and patterns below to make sure Rosetta's codebase can be written consistently:

- **Keep names consistent across languages.** Word choices for names of public variables and functions should be consistent across programming languages. For example, a {term}`Medium` object of the "scatterer" class may be called `medium_scatterer` in Python and `mediumScatterer` in Matlab, but both names derive from the same ordering of the same words.

- **Follow the standards and styles adopted by Rosetta.** Rosetta abides by code formatting as enforced by [Prettier](https://prettier.io/) where possible. Otherwise, the exact standards that Rosetta uses depend on the language:

  - **Matlab:** Camel case (e.g. `nameOfVariable`). Matlab does not have an official style guide, but independently-written ones like those from [Richard Johnson](https://www.ee.columbia.edu/~marios/matlab/MatlabStyle1p5.pdf), [Nico Schlömer](https://github.com/nschloe/matlab-guidelines), or [Yuval Harpaz](https://github.com/yuval-harpaz/mep8) are helpful points of reference.

  - **Python:** Python styling defers to the latest version of the [PEP8 standard](https://peps.python.org/pep-0008) as enforced by [Black](https://black.readthedocs.io/en/stable/). The [Google Style Guide for Python](https://google.github.io/styleguide/pyguide.html) can also be referenced for best practices on specific situations such as how to write exceptions or how to name function inputs.

  - **Web (HTML/CSS):** Learn more about best practices on semantic tagging through [Google's explanation in their developers document](https://developers.google.com/style/semantic-tagging) as well as [the Mozilla Foundation's guide on coding semantics](https://developer.mozilla.org/en-US/docs/Glossary/Semantics).

- **Spell out words.** Generally, you should not abbreviate words so that the meaning of variables, functions etc. are easy to understand. However, there are **some exceptions** where abbreviations can make text _easier_ to read:

  - **Common symbols for physical constants.** These should be restricted to unambiguous, widely recognized terms, such as `c0` for the speed of sound under ambient conditions.

  - **Common acronyms.** Acronyms should be treated as one word.

  - `b` = Base

  - `ctrl` = Controller

  - `doc` = Document

  - `ens` = Ensemble

  - `exp` = Experiment

  - `idx` = Index (when indexing an array or iterating in a loop)

  - `io` = Input/output

  - `med` = Medium

  - `num` = Number

  - `r`, `x`, `y`, `z` = Unit vectors in a coordinate system. Note that Greek alphabets used for rotation angles (e.g. `theta`) should still be spelled out in Latin letters. Do not use `i`, `j`, and `k`.

  - `rx` = Reception

  - `t` = Time

  - `tx` = Transmission

  - `ui` = User interface

  - `xdc` = Transducer

  - `xpt` = {term}`Experiment object<Experiment>`
