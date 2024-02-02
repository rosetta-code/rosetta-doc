# Components

{term}`Components<Component>` are the basic building blocks of Rosetta. Components define hardware, parameters, and processes that form conceptually distinct parts of an {term}`Experiment` where ultrasound signals are emitted and detected.

Rosetta defines the following Components:

{term}`Components<Component>` are the basic building blocks of Rosetta. Components describe different hardware, software, and processes that involve ultrasound. Components are the fundamental building blocks for Rosetta; just like how every computer has a list of parts (a bill of materials) and standardized ways for parts to be assembled (standard operating procedures), every ultrasound-based operation in Rosetta relies upon some action or object that is described using a Component.

Rosetta defines the following Components:

```{toctree}
base.md
transducer.md
transception.md
waveform.md
controller.md
ensemble.md
timeline.md
```

```{note}
Material properties are also defined using Components - specifically, using {term}`Medium` objects. However, we will discuss the Medium class [in its own section](project:../media/index.md) since the ways that it can be defined is so diverse that it needs its own part in this document.
```
