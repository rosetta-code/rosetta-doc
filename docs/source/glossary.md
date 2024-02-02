# Glossary

<!-- for formatting instructions, see https://pandoc.org/MANUAL.html#definition-lists -->

This page defines words that are specific to the Rosetta package, as well as certain other technical terms for acoustics and open-source software libraries that may be helpful for the user to review.

## Rosetta-specific terminology

The following section defines key terms that are specific to Rosetta.

{.glossary}
Adapter
: A library of scripts and functions that can be called by a {term}`Rosetta Experiment<Experiment>`'s `convert` {term}`method<Method>` to implement itself in a third-party platform.
 
    More information can be found in the [Adapters](project:./adapters/index.md) section of this document.

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

Acoustics engineers, including those working in medical ultrasound, may have limited, specific experience with programming and computer science concepts (if any at all). To ensure that *everyone* can use Rosetta from an equal starting point, key terms are defined below.

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
: **Verb:** To subordinate a parent class and inherit {term}`properties<Property>` and {term}`methods<Method>`. Subclasses can also {term}`overload<Polymorphism>` or override methods that are defined by its parent superclass.

Superclass
: **Noun:** A {term}`class<Class>` that defines basic attributes, methods etc. that is elaborated upon by subordinate {term}`subclasses<Subclass>`.

Type
: **Noun:** A category of data; also called a datatype. All {term}`objects<Object>` are data of the type of their {term}`classes<Class>`.

Variable
: **Noun:** An {term}`abstraction<Abstract>` that {term}`encapsulates<Encapsulate>` some **value** (data or {term}`object<Object>`), the **{term}`type<Type>`** of that value, and where the value lives in the computer's memory.

Version control
: **Verb:** To maintain and organize multiple versions and configurations of files (usually software code) in a {term}`repository<Repository>`. This action usually comes up in the context of {term}`Git` where changes to files need to be recorded such that users have the option to switch to other configurations (branches).

## Git terminology

Software and documentation changes for Rosetta are maintained using the Git {term}`version control system<Version control>`. Since it could help to have a working understanding of Git, we've included the meaning and relationships of key terms in this section.

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
: **Verb:** To download commits and other updates from a remote {term}`repository<Repository>`. Fetching is a more conservative alternative {term}`pulling<Pull>` since fetching does not impact the current {term}`workspace<Workspace>`. Fetching is also the inverse to {term}`pushing<Push>`.

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

## Acoustics and ultrasound concepts

Rosetta is a software package for acoustics-related applications. This means that you may need to have a working understanding of important concepts in acoustics and ultrasound.

{.glossary}
Acoustic
: **Adjective:** Relating to the production, control, changes, recognition, and manipulation of sound. The scientific study of this field is **acoustics**. Subfields of acoustics include various academic fields such as:

    - Geology (e.g. seismology, meteorology, and oceanography)
    - Applied physical sciences (e.g. electroacoustics, material science, noise/shock/vibration studies)
    - Life sciences (e.g. medical ultrasound, bioacoustics, psychoacoustics)
    - History and the arts (e.g. speech, archaeoacoustics, architectural acoustics, musical acoustics)

Baffle
: **Noun:** A rigid object that gets in the way of sound propagation. Baffles in ultrasound extend out of a {term}`transducer<Transducer>` parallel to its active surface to manipulate how sound is emitted. Meanwhile, baffles in room acoustics are often suspended from ceilings to reduce {term}`reverb<Reverberate>`.

Clutter
: **Noun:** Signal that is physically real but unwanted in a particular application. This often includes {term}`reverberation<Reverberate>`, motion artifacts, and unwanted reflectors.

Critical distance
: **Noun:** The distance from a sound source where the magnitude of acoustic signal received directly from the source is equal to the magnitude of sound that is received from {term}`reverberation<Reverberate>`.

Echo
: **Noun:** {term}`Reflected<Reflect>` sound that can be detected at the source of the original signal. See the entry on {term}`echogenicity<Echogenic>` for how echoes can be described.

Echogenic
: **Adjective:** The quality of some object or space that returns an {term}`echo<Echo>` response when sound is transmitted. An object or space is **hyperechoic** if it gives off an echo that is relatively large in amplitude, whereas it is **hypoechoic** if the echoes are smaller in amplitude. Objects or spaces that do not return any echoes are **anechoic**.

Haas effect
: **Noun:** A psychoacoustic effect where two sounds heard shortly after each other are perceived as a single sound beyond a certain minimum time delay. This phenomenon is also called the **precedence effect**.

Impact noise
: **Noun:** Unwanted sounds that arise from vibrations in structures that make up a medium. For example, the sound of knocks on a door or footsteps on a floor are two examples of impact noises.

Kerf
: **Noun:** The space that is cut into an array, or the size of such a space. This may refer to the kerf between elements in a transducer array as well as the kerf between acoustical panels. 

Leak
: **Verb:** To transmit sound from one environment such that it can be detected by another, undesired observer.

Love wave
: **Noun:** A type of acoustic {term}`surface wave<Surface wave>` where oscillations occur linearly parallel to the surface but perpendicular to the direction of the wave's propagation.

Pitch
: **Noun:** The distance between two identical, adjacent parts of an array.

Rayleigh-Lamb wave
: **Noun:** A type of acoustic {term}`surface wave<Surface wave>` where oscillations occur in an ellipse-like shape perpendicular to the surface. This type of wave is also called a **Rayleigh wave** when it occurs on the surface of a thick medium, and a **Lamb wave** when it occurs in a layer thinner than several wavelengths.

Reverberate
: **Verb:** To {term}`reflect<Reflect>` sound such that numerous reflections of the same signal are detected.

Sound intensity
: **Noun:** Power carried by sound waves for a given unit of area. This area is measured perpendicular to the direction that the sound is spreading.

Sound power
: **Noun:** Sound energy per unit of time.

Sound pressure
: **Noun:** Force applied by particles being affected by a sound wave in a given unit of area. This area is measured perpendicular to the direction that the sound is spreading.

Standing wave
: **Noun:** A wave that results from two waves that constructively {term}`interfere<Interfere>`.

## General physics and math concepts

Rosetta is a software package for acoustics-related applications. This means that you may need to have a baseline understanding of important words and ideas in physics.

{.glossary}
Absorb
: **Verb:** To convert acoustic energy into another form of energy such as heat or motion. This is the opposite of {term}`reflection<Reflect>`.

Ambient
: **Adjective:** Relating to a particular, universal feature of an environment when it is undisturbed.

Attenuate
: **Verb:** To reduce the magnitude of a signal. The process of something being attenuated is **attenuation**.

Body wave
: **Noun:** Waves that travel through media that is more than several {term}`wavelengths<Wavelength>` in size across all spatial dimensions. Body waves are sometimes also called **bulk waves**. {term}`Longitudinal` and {term}`transverse<Transverse>` waves exist, both of which are distinct from {term}`surface<Surface wave>` waves in three-dimensional space.

Convect
: **Verb:** To move atoms or molecules due to differences in pressure, temperature etc. **Convection** is the act of undergoing this process.

Couple
: **Verb:** To match the {term}`impedance<Impedance>` of two different media.

Damp
: **Verb:** To lose energy in a vibrating system. The act of **damping** is performed by a **damper**.

Diffract
: **Verb:** To bend a wave around an obstacle. The impacts of **diffraction** are especially important when a wave interacts with objects or gaps that are smaller than one {term}`wavelength<Wavelength>`.

Diffuse
: **Verb:** To randomly move around from an area of higher quantity to an area of lower quantity. **Diffusion** is usually discussed for the concentration of atoms or molecules, as well as for changes in temperature over time. However, {term}`numerical artifacts<Numerical artifact>` called **numerical diffusion** can also take place.
: **Adjective:** The quality of one or more objects or events where their presence is sparsely distributed over space. This can refer to objects that may have undergone diffusion, as well as **diffuse reflection** where a wave {term}`deflects over many angles<Scatter>` instead of {term}`reflecting at a single angle<Specular>`.

Disperse
: **Verb:** To modify the wavelength of a wave based on its frequency. **Dispersion** can occur due to the material properties of a wave's medium, geometric effects, or as a {term}`numerical artifact<Numerical artifact>` called **numerical dispersion**.

Dissipate
: **Verb:** To lose energy in a system to {term}`entropy<Entropy>`. {term}`Diffusion<Diffuse>` and {term}`damping<Damp>` are two examples of dissipation taking place.

Doppler effect
: **Noun:** A shift in {term}`frequency<Frequency>` when the source of a wave is moving in the perspective of the observer.

Entropy
: **Noun:** The amount of thermal energy that cannot be converted into usable work (i.e. predictable physical phenomena). This idea is often abbreviated as the amount of "randomness" or "disorder" in a closed system.

    A system is **isentropic** if the amount of entropy does not change after it performs some work. The second law of thermodynamics implies that the work performed by an isentropic system can be reversed. However, if entropy is increased by that system, then the work that it performs is **irreversible**.

Evanescent waves
: **Noun:** Waves that exist within a short distance from an interface between two media where there is a difference in {term}`impedance<Impedance>` and {term}`total internal reflection<Total internal reflection>` takes place.

    Unlike "typical" transmitted waves, evanescent waves do not radiate energy over distances. These waves decay exponentially as a function of distance from the interface, and the amount of energy that evanescent waves carry is confined to a small region of space.
    
    Still, evanescent waves are valid solutions of {term}`wave equations<Wave equation>`, and how they behave depends on properties of the {term}`incident<Incident>` wave and the media that it hits. Thus, these waves still contain useful information as long as they can be measured.

Far field
: **Noun:** This concept is the opposite of the {term}`near field<Near field>` of the source of a wave.

Frequency
: **Noun:** The number of times that the shape of a wave repeats given a set amount of time or distance.

    Given a certain speed and {term}`period (wavelength)<Wavelength>` of the wave, the frequency equals the wave speed divided by the wavelength. Frequency is usually in units of inverse time (i.e. Hertz, abbreviated as Hz), but **spatial frequency** is also discussed (expressed in inverse distance, such as inverse-meters) in some contexts.

Impedance
: **Noun:** The amount to which the propagation of energy is opposed. This concept comes from electrical impedance, a generalization of electrical resistance (opposition of a steady flow of electrons) for alternating currents that uses complex values. Close analogies to electrical impedance are used to discuss similar ideas like **acoustic impedance** and **optical impedance**.

    Impedance in optics is also called the **refractive index** because of the importance of the {term}`refraction<Refract>` of light.

Impulse
: **Noun:** A mathematical object where all values are zero except at zero, where the value equals infinity. This object, thus, has an integral (area under the curve) of one.

    While impulses are not true functions in the mathematical sense, they're still useful for a variety of signal processing tasks and are often called "functions" anyways. In particular, you can use impulses to sample other functions at specific points. This operation is a key part of the **impulse response** of a system.
    
    Impulse functions are also called the **Dirac delta function** or the **delta function**. The analogue to this function in a discrete domain is the **Kronecker delta**.

Incident
: **Adjective:** The property of a wave where it is approaching some feature of interest. For example, you may be interested in talking about an incident wave to distinguish it from a wave that is {term}`reflected<Reflect>`, {term}`refracted<Refract>`, or {term}`diffracted<Diffract>`.

Intensity
: **Noun:** The amount of {term}`power<Power>` transmitted by some radiating energy source over an area. This can also be called the **flux** of the radiation.

Interfere
: **Verb:** To add the {term}`intensities<Intensity>` or particle displacements of two waves. Interfering waves can be **coherent** by having matching {term}`frequencies<Frequency>`, be **incoherent** by having entirely different frequency ranges, or somewhere in between. The resulting interference can be **constructive** such that the two waves are summed into a wave with a larger amplitude, or the interference may be **destructive** such that the two waves cancel each other out.

Isotropy
: **Noun:** The concept of a material whose qualities are consistent across directions. This is in contrast to an **anisotropic** material where properties change depending on the direction.

Longitudinal
: **Adjective:** The quality of something that is parallel to a reference axis.

    In the context of wave physics, **longitudinal waves** are waves that travel in a direction parallel to how particles (e.g. compressional sound waves) oscillate.

Near field
: **Noun:** This concept is the opposite of the {term}`far field<Far field>` of the source of a wave.

Noise
: **Noun:** Signals that are not desired for a particular application. This may include electronic noise, thermal noise, statistical uncertainties in signals, or known signal processing artifacts such as aliasing and {term}`clutter<Clutter>`.

Numerical artifact
: **Noun:** {term}`Noise` that arises due to how computers discretize certain mathematical operations. Unless numerical artifacts are suppressed or avoided through careful design, numerical artifacts can lead to some signals or solutions that may be undesirable or unexpected.

Power
: **Noun:** The amount of energy transmitted by some radiating energy source over time.

Reflect
: **Verb:** To redirect a wave at an interface between two media so that the {term}`incident<Incident>` wave returns into the medium from where it came.

    Reflections can be {term}`diffuse<Diffuse>` or {term}`specular<Specular>`, and all reflections can happen alongside {term}`refraction<Refract>`.

Refract
: **Verb:** To redirect a wave at an interface between two media so that the {term}`incident<Incident>` wave continues to travel through a second medium.

    How reflection takes place depends on the difference of {term}`impedance<Impedance>` between the two media. All refraction happen alongside some degree of {term}`reflection<Reflect>`.

Resonate
: **Verb:** To undergo **resonance**, the phenomenon where something undergoes a forced vibration and responds with a continuous oscillation at a constant amplitude and {term}`frequency<Frequency>` even if additional external forces are not applied. This repetitive motion occurs at the **resonant frequency** of that object or medium.

Signal-to-noise ratio
: **Noun:** The ratio between the magnitude of a desired signal and underlying {term}`noise<Noise>`. In many contexts, this is abbreviated as **SNR** and is expressed in decibels.

Specular
: **Adjective:** The quality of a reflection that is directionally specific. This is usually discussed in the context of a **{term}`specular reflection<Reflect>`** to contrast with {term}`diffuse reflections<Diffuse>` that take place due to {term}`scattering<Scatter>`.

Scatter
: **Verb:** To deflect an {term}`incident<Incident>` wave across multiple directions. This stands in contrast to {term}`the act of reflection<Reflect>` where the direction of wave deflection is more specific.

Surface wave
: **Noun:** Waves that travel in media that is less than several {term}`wavelengths<Wavelength>` in size in one or more spatial dimensions. In three-dimensional space, surface waves are distinct from {term}`bulk<Body wave>` waves in that they travel *along the surface* of a medium.

    In {term}`acoustics<Acoustic>`, surface waves are classified based on the direction that particles in a medium are displaced. Matter oscillates in an ellipsoid trajectory perpendicular to the surface in {term}`Rayleigh and Lamb waves<Rayleigh-Lamb wave>`, while particles that displace perpendicularly to the direction of wave propagation but parallel to the surface are said to be part of a {term}`Love wave`.

Total internal reflection
: **Noun:** The phenomenon where a wave traveling through one medium arrives at a change in {term}`impedance<Impedance>`, but the wave fully {term}`reflects<Reflect>` without any {term}`refraction<Refract>` taking place.

    Note that {term}`evanescent waves<Evanescent waves>` can be present when total internal reflection takes place.

Transducer
: **Noun:** An object that converts one form of energy into another. For example, an acoustic transducer converts sound into electrical currents and vice versa.

Transverse
: **Adjective:** The quality of something that is perpendicular to a reference axis.

    In the context of wave physics, **transverse waves** are waves that travel in a direction perpendicular to how particles (e.g. elastic shear waves) or force fields (e.g. light) oscillate.

    In the context of material properties or anatomy, something that is transverse is perpendicular to an arbitrary axis that is defined as the dominant axis. For example, the transverse Young's modulus of a {term}`transversely isotropic<Isotropy>` material is the stiffness of the material perpendicular to a predefined axis. Likewise, the transverse plane (also called the horizontal or axial plane) in a human body describes a cross-section perpendicular to the body's longitudinal axis (roughly the direction of the person's spine).

Wave
: **Noun:** A disturbance in one or more physical properties that spreads over time and space. {term}`Body<Body wave>`, {term}`surface<Surface wave>`, and {term}`evanescent<Evanescent waves>` waves exist. All three wave types of waves can be described succinctly as solutions of a well-defined {term}`wave equation<Wave equation>`.

Wave equation
: **Noun:** A mathematical expression for how waves travel and behave over space and time. Different wave equations exist for different types of waves (e.g. sound, light, seismic waves), as well as for different assumptions about physical behaviors that take place.

Wavelength
: **Noun:** The distance at which the shape of a wave repeats.

    Given a certain speed and {term}`frequency<Frequency>` of the wave, the wavelength equals the wave speed multiplied by the frequency. Wavelengths are usually expressed in units of distance. If the wavelength is being discussed in units of time, it is often called the **period**.
