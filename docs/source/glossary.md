# Glossary

<!-- for formatting instructions, see https://pandoc.org/MANUAL.html#definition-lists -->

This page defines words that are specific to the Rosetta package, as well as certain other technical terms for acoustics and open-source software libraries that may be helpful for the user to review.

## Rosetta-specific terminology

The following section defines key terms that are specific to Rosetta.

{.glossary}
Adapter
: A library of scripts and functions that can be called by a {term}`Rosetta Experiment<Experiment>`'s `convert` {term}`method<Method>` to implement itself in a third-party platform.
 
    More information can be found in the [Adapters](project:./adapters/index.md) section of this document.

Component
: A {term}`class<Class>` (or an {term}`instance<Instance>` of an {term}`object<Object>` thereof) that defines a particular aspect of an ultrasound/acoustic experiment or environment.

    More information can be found in the [Components](project:./components/index.md) section of this document.

Experiment
: A {term}`class<Class>` (or an {term}`instance<Instance>` of an {term}`object<Object>` thereof) that contains references to other Rosetta objects and defines relationships between them.

    More information can be found in the [Experiments](project:./experiments/index.md) section of this document.

Medium
: A {term}`class<Class>` (or an {term}`instance<Instance>` of an {term}`object<Object>` thereof) that defines one or more material properties where sound (or another form of energy or matter) will propagate through.

    More information can be found in the [Media](project:./media/index.md) section of this document.

Rosetta
: The Reusable Organizer for Simulating, Experimenting, Teaching, and Testing in Acoustics.

## Programming concepts

Acoustics engineers, including those working in medical ultrasound, may have limited, specific experience with programming and computer science concepts (if any at all). To ensure that _everyone_ can use Rosetta from an equal starting point, we've included the definition of key terms below.

{.glossary }
Abstract
: **Verb:** To hide the implementation of data manipulation outside of the {term}`scope<Scope>` of that operation. By abstracting a class or a function through {term}`encapsulation<Encapsulate>`, you can simplify an interface so that the user only has to worry about whether they are using the correct input and output.
: **Adjective:** Existing as an incomplete entity (usually a class) that cannot be {term}`instantiated<Instantiate>`. For example, an **abstract class** is not meant to be used on its own to create {term}`objects<Object>`, but it can be {term}`subclassed<Subclass>` by other {term}`classes<Class>`.

Anonymous function
: **Noun:** An unnamed {term}`function<Function>` that cannot be directly accessed but _can_ be used similarly to a {term}`variable<Variable>`. This is sometimes also called a **lambda function**.

Assign
: **Verb:** To (re)set a value that is stored using a {term}`variable<Variable>`.

Attribute
: **Noun:** A particular aspect of information that is associated with an {term}`objects<Object>` of some {term}`class<Class>`. This is sometimes also called the **state** of an object. Also see {term}`properties<Property>`.

Class
: **Noun:** A blueprint that defines a particular category of {term}`objects<Object>`. Classes are possess various {term}`attributes<Attribute>`, and they can be analyze or manipulated using {term}`methods<Method>` that are designed for that particular class.

Constructor
: **Noun:** A special {term}`method<Method>` that {term}`instantiates<Instantiate>` an {term}`object<Object>` of a given {term}`class<Class>`. Constructors can take (or even require) certain input arguments to define an {term}`instance<Instance>`.

Control Flow
: **Noun:** The order in which specific instructions (e.g. {term}`function<Function>` calls) are executed.

Destroy
: **Verb:** To perform specific tasks, then release an {term}`object<Object>` from memory.

Destructor
: **Noun:** A special {term}`method<Method>` that {term}`destroys<Destroy>` an {term}`object<Object>` of a given {term}`class<Class>`. This is the opposite of a {term}`constructor<Constructor>`, and marks the end of an object's {term}`life cycle<Lifetime>`.

Encapsulate
: **Verb:** To restrict direct access to some {term}`attributes<Attribute>` or {term}`methods<Method>` of an {term}`object<Object>`. This can be helpful to make certain features of a class read- or write-only, as well as for data security. This is the opposite of {term}`exposure<Expose>`.

Enumeration
: **Noun:** A {term}`data type<Type>` that consists of specific values. For example, in a rating system where diners can indicate that they (dis)like a restaurant, a rating could be encoded as either `good`, `bad`, or `neutral`.

Exception
: **Noun:** A condition that arises while a program is running and requires special handling. This occurs most commonly in abnormal, unpredictable, and erroneous situations, but it can also be used in the context of regular programming (e.g. Python uses exceptions to signal when iterations in a loop are complete).

Expose
: **Verb:** To allow direct access to some {term}`attributes<Attribute>` or {term}`methods<Method>` of an {term}`object<Object>`. This is the opposite of {term}`encapsulation<Encapsulate>`.

Function
: **Noun:** A self-contained, reusable unit of code that takes an input, accomplishes a specific task, and returns an output. Functions are typically named and stored in a static way (i.e. a file that doesn't change when a program is run), but {term}`they could be anounymous<Anonymous function>` as well.

Git
: **Noun:** A lightweight software system that enables {term}`version control<Version control>`. Learn more at [Git's website](https://git-scm.com/) or refer to the [Git terminology](project:#git-terminology) section of this glossary.

IDE
: **Noun:** Short for an integrated developer environment; an app that helps software engineers write, test, and run code. Some languages like Matlab come with its own, proprietary IDE while other languages like Python are not tied to any particular IDE. In the latter case, many programmers use free, general-purpose IDEs like [Visual Studio Code](https://code.visualstudio.com/).

Inherit
: **Verb:** To derive characteristics from one {term}`class<Class>` to define another. The result of this is a new class that is a {term}`subclass<Subclass>` of the original {term}`superlass<Superclass>`.

Instance
: **Noun:** A single, unique entity of data that is a member of a particular {term}`class<Class>`. Some places also call this a single {term}`object<Object>`, but the act of creating one is still called {term}`instantiation<Instantiate>`.

Instantiate
: **Verb:** To generate an {term}`instance<Instance>` of a certain {term}`class<Class>`.

Lifetime
: **Noun:** The series of events that occur between the {term}`instantiation<Instantiate>` and {term}`destruction<Destroy>` of an {term}`object<Object>`.

Method
: **Noun:** A function that acts upon {term}`objects<Object>` of a particular {term}`class<Class>`. Methods are defined in the context of the class where it belongs, so it's defined within that class.

Namespace
: **Noun:** Declared imaginary domains that defines a {term}`scope<Scope>`. Namespaces are often controlled using specific directory structures, packages etc. so that certain functions and variables can be used in a given context without conflicts with other, identically-named resources that exist elsewhere.

Object
: **Noun:** Specific units of data that is specifically defined by some {term}`class<Class>`. Every object is unique versus every other object based on its **identity**, possess one or more **states**, and undergo some predefined set of **behaviors**.

    Note that the word "object" universally refers to the idea of an arbitrary set of such an item (i.e. it's an indefinite noun) or it refers to multiple units of them (i.e. it's a definite plural noun). However, some authors may call an individual entity of class-defined data as "an object" while others refer to them as individual _{term}`instances<Instance>`_ of objects.

Object-oriented programming
: **Noun:** A type of programming where code performs tasks by manipulating data, defined as one or more {term}`objects<Object>`, in controlled ways. This is sometimes abbreviated as "**OOP**".

Polymorphism
: **Noun:** The ability for something to take on multiple forms. In {term}`OOP<Object-oriented programming>`, this can take on several forms:

    1.  **Ad-hoc polymorphism**: an interface (e.g. a {term}`function<Function>`) is ad-hoc polymorphic if a single interface can be used for multiple {term}`classes<Class>` and the interface is implemented separately for each class. This is also called **function overloading** or **method overloading** as you are _overloading_ a function or {term}`method<Method>` by creating distinct implementations for different classes.
    2.  **Parametric polymorphism**: an interface is parametrically polymorphic if it uses one implementation regardless of class. This sort of interface is also called a **generic function** as it's a single, _generic_ piece of code that behaves identically regardless of {term}`type<Type>`.
    3.  **Subtyping**: if an object is a {term}`subclass<Subclass>` of another class, then any feature or operation that can be done for the original {term}`superlass<Superclass>` also applies to the subclass. This idea has two close relatives: one for the _structure_ of objects exists as **row polymorphism**, and one for the ability to use operations regardless of the size and dimension of arrays called **rank polymorphism**. Row polymorphism is not as relevant for Rosetta, but rank polymorphism can be useful for performing certain mathematical operations quickly and more efficiently.

    How polymorphic relationships of code are understood by computers can be understood based on how they are dispatched. The relationships may be resolved once when code is compiled (static dispatching, which confers **static polymorphism**) or they may be constructed each time code is executed (dynamic dispatching, which leads to **dynamic polymorphism**).

Property
: **Noun:** The preferred terminology for {term}`attributes<Attribute>` in Matlab, the first programming language where {term}`Rosetta` was implemented.

Scope
: **Noun:** The conceptual space where certain {term}`variables<Variable>` or {term}`functions<Function>` can be accessed. There are several different scopes:

    1.  **Global scopes**: A variable or subfunction can be used in an entire program. This can be changed by accessing and manipulating the global {term}`namespace<Namespace>` that is made accessible to a program.
    2.  **File** or **module scopes**: A variable or subfunction can be used as long as a module is imported or the user is currently parsing the file. This is most often modified by specifying or manipulating the local namespace.
    3.  **Function scopes**: A variable or subfunction can be used inside of a function but not outside of it.
    4.  **Code block scopes**: A variable or subfunction can only be used within a specific block of code.

Subclass
: **Noun:** A {term}`class<Class>` that defines how it is implemented based on a superior parent class.
: **Verb:** To subordinate a parent class and inherit `properties<Property>` and `methods<Method>`. Subclasses can also {term}`overload<Polymorphism>` or override methods that are defined by its parent superclass.

Superclass
: **Noun:** A {term}`class<Class>` that defines basic attributes, methods etc. that is elaborated upon by subordinate {term}`subclasses<Subclass>`.

Type
: **Noun:** A category of data; also called a datatype. All {term}`objects<Object>` are data of the type of their {term}`classes<Class>`.

Variable
: **Noun:** An {term}`abstraction<Abstract>` that {term}`encapsulates<Encapsulate>` some **value** (data or {term}`object<Object>`), the **{term}`type<Type>`** of that value, and where the value lives in the computer's memory.

Version control
: **Verb:** To maintain and organize multiple versions and configurations of files (usually software code) in a {term}`repository<Repository>`. This action usually comes up in the context of {term}`Git` where changes to files need to be recorded such that users have the option to switch to other configurations (branches).

## Git terminology

Software and documentation changes for Rosetta are maintained using the Git {term}`version control system<Version control>`. While we presume that you have a working understanding of Git, we've included the meaning and relationships of key terms, below, for your convenience.

{.glossary}
Branch
: **Verb:** To create a new chronology of {term}`tracked<Track>` changes in a {term}`repository<Repository>`, similar to branches that splits out of a growing tree or a branch in a timeline of alternate histories. Unlike a {term}`fork<Fork>`, branching is an operation that takes place _within_ a repo.
: **Noun:** A reference to a particular line of development in a {term}`repository<Repository>`. Every repo has at least one branch (usually called `main` or `master`), but multiple branches can exist depending on [how a repo is maintained](https://www.atlassian.com/git/tutorials/comparing-workflows).

Checkout
: **Verb:** To change the contents of the {term}`working directory<Workspace>` to reflect a particular {term}`commit<COmmit>`. Commits can be checked out even if they belong in a different {term}`branch<Branch>` or a {term}`remote repo<Repository>`.

Clone
: **Verb:** To locate a {term}`repository<Repository>` and create a copy of it elsewhere.

Commit
: **Verb:** To record of changes in files that are {term}`staged<Stage>` in the {term}`index<Index>` of a {term}`repository<Repository>`. This essentially clears out the index and creates a permanent record of changes that were staged.
: **Noun:** A snapshot of a repo. When changes to files in a {term}`workspace<Workspace>` are recorded as commits, contents of the directory can be recreated by {term}`checking out<Checkout>` that commit.

Diff
: **Noun:** An operation where two different data sources in Git are compared. {term}`Tracked<Track>` files, {term}`commits<Commit>`, {term}`branches<Branch>` etc. can be compared using this function.

Downstream
: **Adjective:** A {term}`repository<Repository>` is derived from another repo. Since Git is a distributed system where there is no inherent heirarchy, it only makes sense to say that a local repo is downstream _to_ another repo. This is the opposite of a repo that is {term}`upstream<Upstream>`.

Fetch
: **Verb:** To download commits and other updates from a remote {term}`repository<Repository>`. Fetching is a more conservative alternative {term}`pulling<Pull>` since fetching does not impact the current <term>`workspace<Workspace>`. Fetching is also the inverse to {term}`pushing<Push>`.

Fork
: **Verb:** To create a new, independent copy of a {term}`repository<Repository>`. This is similar to {term}`branching<Branch>` but it creates an entirely separate repository.
: **Noun:** A repository that was created by forking another repo.

Index
: **Noun:** Temporary location where file changes can be recorded ({term}`staged<Stage>`) prior to a {term}`commit<Commit>`.

Ignore
: **Verb:** To exempt a file or folder from {term}`version control<Track>`. This can be done on a case-by-case basis or, more commonly, by listing files in a text file called `.gitignore`.

Merge
: **Verb:** To create a {term}`commit<Commit>` where changes in two different branches of a {term}`repository<Repository>` are combined.
: **Noun:** The commit that results from a merge operation.

Merge conflict
: **Noun:** A situation where changes to files are contradictory between two {term}`commits<Commit>`. This could be anticipated (and thus prevented) by performing a {term}`diff<Diff>`. More information about merge conflicts are given on [this webpage](https://www.atlassian.com/git/tutorials/using-branches/merge-conflicts).

Pull
: **Verb:** To download commits and other updates from a remote {term}`repository<Repository>` and {term}`merge<Merge>` them with the latest {term}`commits<Commit>`. This is essentially a more aggressive version of {term}`fetching<Fetch>`.

Pull request
: **Noun:** A message where someone who forked a {term}`repository<Repository>` asks the original repo's maintainers to incorporate specific {term}`commits<Commit>` that they wrote. If this _request_ is accepted, the original repo will _pull_ those changes.

Push
: **Verb:** To upload {term}`commits<Commit>` and other data from a local {term}`repository<Repository>` to a remote repo. This is essentially the inverse of {term}`fetching<Fetch>`.

Repository
: **Noun:** A collection of files whose changes are {term}`tracked<Track>` in a {term}`version control system<Version control>`; also called a **repo**. Multiple versions of files and folders can exist in the form of different **branches** of a repository. Copies of files can exist in the **local repo** where you are currently working, as well as on other machines (or even elsewhere on your own machine) as **remote repos**. From a technical perspective, no repo is more special or authoritative than any other repo.

Stage
: **Verb:** To make Git recognize changes in files by storing them in a temporary holding area (an {term}`index<Index>`) before {term}`committing<Commit>` them.

Submodule
: **Noun:** A record within one {term}`repository<Repository>` that points to a specific {term}`commit<Commit>` in another repo. [This webpage](https://www.aviator.co/blog/managing-repositories-with-git-submodules/) discusses the benefits, limitations, and best practices for using this approach. Subtrees can be seen as the more specific but harder-to-use alternative to {term}`subtrees<Subtree>`.

Subtree
: **Noun:** A {term}`repository<Repository>` that resides within another repo. [This webpage](https://www.atlassian.com/git/tutorials/git-subtree) discusses the benefits, limitations, and best practices for using this approach. Subtrees can be seen as the more specific but harder-to-use alternative to {term}`submodules<Submodule>`.

Tag
: **Noun:** A reference to a specific {term}`commit<Commit>`. This is often used to denote specific, versioned releases of the contents of a {term}`repository<Repository>`.

Track
: **Verb:** To recognize, monitor, and record changes to files in a {term}`repository<Repository>`. This is the key feature of a {term}`version control system<Version control>`.

Upstream
: **Adjective:** A {term}`repository<Repository>` that is the source of content for another, derivative repo. Since Git is a distributed system where there is no inherent heirarchy, it only makes sense to say that a local repo is upstream _of_ another repo; no repository is absolutely or supremely upstream. This is the opposite of a repo that is {term}`downstream<Downstream>`.

Workspace
: **Noun:** The actual path where files are located and potentially {term}`version-tracked<Track>`. This location is also called the **working directory** or **project folder**, and contains a hidden folder called `.git` where Git's actual version-controlling operations take place. However, untracked files can also exist in the workspace where they act like regular files that are unaffected by Git operations.

    Put another way: Git is used to change the existence and contents of files in a workspace based on a selected {term}`commit<Commit>` in a {term}`repo<Repository>`.

## Physics concepts

As a software package for acoustics-related applications, we must also ensure that we have a common baseline understanding of relevant terms in physics.

{.glossary}
Wave
: **Noun:** A disturbance in one or more physical properties that propagates (spreads over time and space).

Wave equation
: **Noun:** A mathematical expression for how waves travel and behave over space and time.
