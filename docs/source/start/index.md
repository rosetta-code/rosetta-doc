# About Rosetta

```{toctree}
:hidden:
install
verify
contact
```

Welcome to the documentation for {term}`Rosetta`, the Reusable Organizer for Simulating, Experimenting, Teaching, and Testing in Acoustics. It's an open-source, cross-platform tool to describe, manipulate, and implement ultrasound transmissions in simulations _and_ physical hardware using a single codebase.

This document describes key concepts and procedures used in Rosetta, as well as guidance documentations for Rosetta's APIs.

## Getting started

To get started, you can:

::::{grid} 1 2 2 3
:gutter: 3 3 4 5

:::{grid-item-card} Discover Rosetta
:link: ../index.html
Learn more about Rosetta and how it could help your engineering needs.
:::
:::{grid-item-card} Get started
:link: ./install.html
Get Rosetta by trying out Rosetta for an environment of your choice.
:::
:::{grid-item-card} Read our User Guide
:link: ../components/index.html
Learn about in-depth ideas and key concepts behind the technology that makes Rosetta work.
:::
:::{grid-item-card} Learn our principles
:link: ../principles.html
Get to know the core beliefs, values, and objectives held by the community members and moderators of Rosetta.
:::
:::{grid-item-card} Contribute to Rosetta
:link: ../contribute.html
Want to add to this text or enhance our code? Learn about the process of reporting issues and submitting changes to Rosetta.
:::
:::{grid-item-card} Describe our API
:link: /index.html
Read detailed descriptions about what code exists in Rosetta and which concepts will be used.
:::
::::

## Anatomy of Rosetta

The Rosetta API is organized in identical ways regardless of what programming language you use to interface with it. Rosetta consists of three main parts:

- **{term}`Components<Component>`:** hardware, software, and processes that involve ultrasound; Components are the fundamental building blocks for Rosetta.

- **{term}`Experiments<Experiment>`:** a combination of Components related to a single set of acoustic signal emission and acquisition.

- **{term}`Adapters<Adapter>`:** a software module that implements an Experiment described using Rosetta into another platform.
