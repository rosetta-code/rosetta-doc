# About Rosetta
```{toctree}
:hidden:
install
contact
```

Welcome to the documentation for {term}`Rosetta`, the Reusable Organizer for Simulating, Experimenting, Teaching, and Testing in Acoustics. It's an open-source, cross-platform tool to describe, manipulate, and implement ultrasound transmissions in simulations *and* physical hardware using a single codebase.

Rosetta aims to create a community of engineers from various backgrounds can share and implement new techniques in a standardized, transparent, and democratic way. While it was conceived and designed as a way to accelerate medical ultrasound beamforming techniques, it can also be used to simplify and standardize descriptions of acoustic experiments in other fields, as well.

This document describes key concepts and procedures used in Rosetta, as well as guidance documentations for Rosetta's APIs.

## Getting started
To get started, you can:

* Learn more about Rosetta and how it could help your engineering needs in [our homepage](project:/index.md)

* [Get Rosetta for an environment of your choice](project:./install.md)

* [Contribute to Rosetta](project:../contribute.md) by reporting issues or submitting changes

* Get to know the Rosetta project's [core principles](project:../principles.md)

* Read Rosetta's [licensing terms](project:../contribute.md#license) and [our expectations](project:../cite.md) when you build off of our work

## Anatomy of Rosetta
The Rosetta API is organized in identical ways regardless of what programming language you use to interface with it. Rosetta consists of three main parts:

### Components
{term}`Components<Component>` describe different hardware, software, and processes that involve ultrasound. Components are the fundamental building blocks for Rosetta; just like how every computer has a list of parts (a bill of materials) and standardized ways for parts to be assembled (standard operating procedures), every ultrasound-based operation in Rosetta relies upon some action or object that is described using a Component.

More information can be found in the [Components](project:../components/index.md) section of this document.

Note that various types of Components are defined in Rosetta. This includes various subcategories that are listed under the Components section of this document, as well as definitions of material properties ({term}`Medium` objects). However, the Medium class is detailed [in its own section](project:../media/index.md) due to its diversity in how it can be defined.

### Experiments
{term}`Experiments<Experiment>` combines particular sets of Components and defines how they relate to each other. Experiments outline what signals are transmitted, when and where they are transmitted from, what it travels through etc. Thus, Experiments give context to how Components come together.

More information can be found in the [Experiments](project:../experiments/index.md) section of this document.

### Adapters
Although Rosetta Components and Experiments are platform-independent on their own, it can be helpful to implement them in specific environments. For example, you may want to implement an Experiment in a particular hardware system. This translation operation can be done by calling an {term}`Adapters<Adapter>`.

More information can be found in the [Adapters](project:../adapters/index.md) section of this document.
