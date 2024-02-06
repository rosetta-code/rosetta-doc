# Style guide

Coding, comments, and documentation for Rosetta can quickly become overwhelming or inconsistent. These rules and guidelines aim to create standard expectations that fit [our community's principles](project:./principles.md).

## General ideas

- **Be conversational, friendly, and clear.**

  - **Focus on the reader.** Address the reader as "you" and focus your writing on them. To avoid talking down on users, only use "we" to talk about the Rosetta project and its moderators.

  - **Use active voice.** Be clear about who's performing an action.

  - **Explain your thoughts.** Instructions should explain _what_ you do, as well as _why_ it's important or why it's done in a certain way.

  - **Be explicit about your actions.** Tell your readers when to do specific tasks, such as creating files or running scripts.

  - **Put conditions before actions.** For example, "to delete the text, click here" rather than "click here to delete the text".

  - **Use American English.** Variables should be named and spelled in American English according to the latest edition of [Webster's Dictionary](https://www.merriam-webster.com/).

  - **Use serial commas,** also called Oxford commas.

  - **Format text using the appropriate features.** Use numbered lists for procedures, bullet lists for other lists, date formatting that is not culturally ambiguous, and code in code font.

  - **Make your content accessible.** Add alternative text, high-resolution images, and vector graphics where they're appropriate.

- **Refer to Google's Developer Documentation Style Guide.** If this document doesn't answer a question you have, look at [Google](https://developers.google.com/style) and [Digital Ocean](https://www.digitalocean.com/community/tutorials/digitalocean-s-technical-writing-guidelines)'s writing guidelines, as well as the third-party references that they recommend.

- **Break the rules when it's necessary.** In certain cases, your content may be easier to use or understand if you _don't_ follow the guidelines in this document. You should depart from them in those specific instances. However, you should also be prepared if anyone asks why you made that decision.

## Coding style

### General practices

- **Prioritize clarity, _then_ brevity.** Rosetta is, first and foremost, a tool for communication and collaboration.

- **Minimize coupling.** Code that is contained in one file or module should work independently from outside code. This helps to simplify relationships between different files and modules, making it easier to write and test code. To do this:

  - **Use subfunctions and modules.** If a function is only used by one other function, consider defining them in the same file so that code files are easier to understand and maintain. If the same task is used in multiple places, isolate repeated code into a single place.

  - **Write out and minimize dependencies.** For example, if two objects need to be related, only one object needs to store a reference to the other object. For example, to relate an ultrasound transducer to a scanner system that will control it, the scanner could have an "attach" method that connects the transducer to the scanner. The transducer does not need to store any information about the scanner.

- **Maximize cohesion.** Each file or module of code should only perform one task, and their contents should be related. This helps to ensure that a certain type of action is the specific responsibility of a specific piece of code, making it easier to edit and test. To do this:

  - **Dedicate one function to one task.** If you find it easiest to describe a task through multiple concerete steps, each step should be its own function. Each function should abstract out other sub-steps.

  - **Make interactions specific and clear.** Use explicit inputs and outputs to functions, and avoid global variables.

- **Be careful of using floating points as binary operators.** Floating point errors can cause unexpected results when floating point numbers are used as binary values.

- **Only make assumptions explicitly.** If a part of code uses hardcoded numbers or arguments, the reasons for those values or the sources of those values could become unclear. To avoid this, you should explicitly set those values as variables (or even as optional function inputs or object properties).

### Naming conventions

Please follow the rules and patterns below to make sure Rosetta's codebase can be written consistently:

- **Use ASCII characters for variable names.**

- **Variable names should be singular nouns.** Even for an array of multiple objects, variable names should be based on singular words. For example, you should call an array of strings that define the names of different shapes `shape` rather than `shapes`.

- **Function and method names should start with verbs.** Functions and methods perform some operation on data. To reinforce this, these operations should be named for what they do. However, there is an exception:

  - **Functions with single outputs should be named for their outputs.** For example, a function that gives the sum of two numbers performs one task and returns one output. Thus, you should name this function `sum` rather than, for instance, `doSum`.

- **Reserve certain verbs for certain operations.** By having rule-based or symmetric names, you can help make your code simpler to understand and easier to maintain. For example:

  - **Is** for boolean operations
  - **Add** and **remove** to append or omit data
  - **Create** and **destroy** to manipulate {term}`objects<Object>`
  - **Read** and **write** or **open** and **close** for file operations

- **Prefix related variable names with common categories.** For example, you could clarify that two strings define the name of colors and belong together. To do so, they could be named `colorRed` and `colorGreen`.

- **Functions, methods, and variables should have specific, intuitive, and meaningful names** that can be easily categorized and require minimal explanation. For example, a good name for a function that calculates the area of a triangle `computeAreaTriangle`. This would be better than `compTriA` since the meanings of the abbreviations are vague out of context. Similarly:

  - **Avoid negative boolean variable names.** For example, the meaning of a line of code that reads `not(isNotFound)` may not be immediately clear to other readers.

  - **Treat acronyms as one word in capitalization rules.** For example, a variable name that mentions the acronym "USA" (the United States of America) should be called `isResidentUsa` instead of `isResidentUSA`.

- **Beware of namespace shadowing.** Beware of function and class names that overlap with other built-in or imported operations. If you call the "wrong" function, unexpected behaviors may arise.

- **Keep names consistent across languages.** Word choices for names of public variables and functions should be consistent across programming languages. For example, a {term}`Medium` object of the "scatterer" class may be called `medium_scatterer` in Python and `mediumScatterer` in Matlab, but both names derive from the same ordering of the same words.

- **Follow the standards and styles adopted by Rosetta.** Rosetta abides by code formatting as enforced by [Prettier](https://prettier.io/) where possible. Otherwise, the exact standards that Rosetta uses depend on the language:

  - **Matlab:** Camel case (e.g. `nameOfVariable`). Matlab does not have an official style guide, but independently-written ones like those from [Richard Johnson](https://www.ee.columbia.edu/~marios/matlab/MatlabStyle1p5.pdf), [Nico Schlömer](https://github.com/nschloe/matlab-guidelines), or [Yuval Harpaz](https://github.com/yuval-harpaz/mep8) are helpful points of reference.

  - **Python:** Python styling defers to the latest version of the [PEP8 standard](https://peps.python.org/pep-0008) as enforced by [Black](https://black.readthedocs.io/en/stable/). The [Google Style Guide for Python](https://google.github.io/styleguide/pyguide.html) can also be referenced for best practices on specific situations such as how to write exceptions or how to name function inputs.

  - **Web (HTML/CSS):** Learn more about best practices on semantic tagging through [Google's explanation in their developers document](https://developers.google.com/style/semantic-tagging) as well as [the Mozilla Foundation's guide on coding semantics](https://developer.mozilla.org/en-US/docs/Glossary/Semantics).

- **Spell out words.** Generally, you should not abbreviate words so that the meaning of variables, functions etc. are easy to pronounce and understand. However, there are **some exceptions** where abbreviations can make text _easier_ to read:

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
