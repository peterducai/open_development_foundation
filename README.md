# open_development_foundation


## Rules

The Unix philosophy is documented by Doug McIlroy[1] in the Bell System Technical Journal from 1978:[2]

Make each program do one thing well. To do a new job, build afresh rather than complicate old programs by adding new "features".
Expect the output of every program to become the input to another, as yet unknown, program. Don't clutter output with extraneous information. Avoid stringently columnar or binary input formats. Don't insist on interactive input.
Design and build software, even operating systems, to be tried early, ideally within weeks. Don't hesitate to throw away the clumsy parts and rebuild them.
Use tools in preference to unskilled help to lighten a programming task, even if you have to detour to build the tools and expect to throw some of them out after you've finished using them.
It was later summarized by Peter H. Salus in A Quarter-Century of Unix (1994):[1]

Write programs that do one thing and do it well.
Write programs to work together.
Write programs to handle text streams, because that is a universal interface.
In their award-winning Unix paper of 1974, Ritchie and Thompson quote the following design considerations:[3]

Make it easy to write, test, and run programs.
Interactive use instead of batch processing.
Economy and elegance of design due to size constraints ("salvation through suffering").
Self-supporting system: all Unix software is maintained under Unix.




"You aren't gonna need it"[1][2] (YAGNI)[3] is a principle of extreme programming (XP) that states a programmer should not add functionality until deemed necessary.[4] XP co-founder Ron Jeffries has written: "Always implement things when you actually need them, never when you just foresee that you need them."[5] Other forms of the phrase include "You aren't going to need it"[6][7] and "You ain't gonna need it".[8]





Don't repeat yourself (DRY, or sometimes do not repeat yourself) is a principle of software development aimed at reducing repetition of software patterns,[1] replacing it with abstractions or using data normalization to avoid redundancy.

The DRY principle is stated as "Every piece of knowledge must have a single, unambiguous, authoritative representation within a system". The principle has been formulated by Andy Hunt and Dave Thomas in their book The Pragmatic Programmer.[2] They apply it quite broadly to include "database schemas, test plans, the build system, even documentation".[3] When the DRY principle is applied successfully, a modification of any single element of a system does not require a change in other logically unrelated elements. Additionally, elements that are logically related all change predictably and uniformly, and are thus kept in sync. Besides using methods and subroutines in their code, Thomas and Hunt rely on code generators, automatic build systems, and scripting languages to observe the DRY principle across layers.






SOLID

Concepts
Single responsibility principle[6]
A class should only have a single responsibility, that is, only changes to one part of the software's specification should be able to affect the specification of the class.
Open–closed principle[7]
"Software entities ... should be open for extension, but closed for modification."
Liskov substitution principle[8]
"Objects in a program should be replaceable with instances of their subtypes without altering the correctness of that program." See also design by contract.
Interface segregation principle[9]
"Many client-specific interfaces are better than one general-purpose interface."[4]
Dependency inversion principle[10]
One should "depend upon abstractions, [not] concretions."[4]






The first five principles are principles of class design. They are:
SRP	The Single Responsibility Principle	A class should have one, and only one, reason to change.
OCP	The Open Closed Principle	You should be able to extend a classes behavior, without modifying it.
LSP	The Liskov Substitution Principle	Derived classes must be substitutable for their base classes.
ISP	The Interface Segregation Principle	Make fine grained interfaces that are client specific.
DIP	The Dependency Inversion Principle	Depend on abstractions, not on concretions.

The next six principles are about packages. In this context a package is a binary deliverable like a .jar file, or a dll as opposed to a namespace like a java package or a C++ namespace.

The first three package principles are about package cohesion, they tell us what to put inside packages:

REP	The Release Reuse Equivalency Principle	The granule of reuse is the granule of release.
CCP	The Common Closure Principle	Classes that change together are packaged together.
CRP	The Common Reuse Principle	Classes that are used together are packaged together.

The last three principles are about the couplings between packages, and talk about metrics that evaluate the package structure of a system.

ADP	The Acyclic Dependencies Principle	The dependency graph of packages must have no cycles.
SDP	The Stable Dependencies Principle	Depend in the direction of stability.
SAP	The Stable Abstractions Principle	Abstractness increases with stability.










In information systems design and theory, single source of truth (SSOT) is the practice of structuring information models and associated data schema such that every data element is mastered (or edited) in only one place. Any possible linkages to this data element (possibly in other areas of the relational schema or even in distant federated databases) are by reference only. Because all other locations of the data just refer back to the primary "source of truth" location, updates to the data element in the primary location propagate to the entire system without the possibility of a duplicate value somewhere being forgotten.











KISS, an acronym for "keep it simple, stupid" or "keep it stupid simple", is a design principle noted by the U.S. Navy in 1960.[1][2] The KISS principle states that most systems work best if they are kept simple rather than made complicated; therefore, simplicity should be a key goal in design, and unnecessary complexity should be avoided. The phrase has been associated with aircraft engineer Kelly Johnson.[3] The term "KISS principle" was in popular use by 1970.[4] Variations on the phrase include: "Keep it simple, silly", "keep it short and simple", "keep it simple and straightforward",[5] "keep it small and simple", or "keep it stupid simple".[6]




## OO principles


In object-oriented programming, the open/closed principle states "software entities (classes, modules, functions, etc.) should be open for extension, but closed for modification";[1] that is, such an entity can allow its behaviour to be extended without modifying its source code.

The name open/closed principle has been used in two ways. Both ways use generalizations (for instance, inheritance or delegate functions) to resolve the apparent dilemma, but the goals, techniques, and results are different.

Open-closed principle is one of the five SOLID principles of object-oriented design.




A module will be said to be open if it is still available for extension. For example, it should be possible to add fields to the data structures it contains, or new elements to the set of functions it performs.
A module will be said to be closed if [it] is available for use by other modules. This assumes that the module has been given a well-defined, stable description (the interface in the sense of information hiding).[3]
At the time Meyer was writing, adding fields or functions to a library inevitably required changes to any programs depending on that library. Meyer's proposed solution to this dilemma relied on the notion of object-oriented inheritance (specifically implementation inheritance):

A class is closed, since it may be compiled, stored in a library, baselined, and used by client classes. But it is also open, since any new class may use it as parent, adding new features. When a descendant class is defined, there is no need to change the original or to disturb its clients.[4]






## Other


Release early, release often (also: time-based releases, sometimes abbreviated RERO) is a software development philosophy that emphasizes the importance of early and frequent releases in creating a tight feedback loop between developers and testers or users, contrary to a feature-based release strategy. Advocates argue that this allows the software development to progress faster, enables the user to help define what the software will become, better conforms to the users' requirements for the software,[1] and ultimately results in higher quality software.[2] The development philosophy attempts to eliminate the risk of creating software that no one will use.[3]

This philosophy was popularized by Eric S. Raymond in his 1997 essay The Cathedral and the Bazaar, where Raymond stated "Release early. Release often. And listen to your customers".[4]

This philosophy was originally applied to the development of the Linux kernel and other open-source software, but has also been applied to closed source, commercial software development.

The alternative to the release early, release often philosophy is aiming to provide only polished, bug-free releases.[5] Advocates of RERO question that this would in fact result in higher-quality releases.[4]



## Design

Active-Admin-driven development (AADD)
Behavior-driven development (BDD)
Bug-driven development (BgDD)
Configuration-driven development (CDD)
Design-driven development (D3)
Domain-driven design (DDD)
Feature-driven development (FDD)
Test-driven development (TDD)
User-centered design (UCD)
Value-driven design (VDD)



https://en.wikipedia.org/wiki/Software_design_pattern


https://en.wikipedia.org/wiki/Software_development_process


https://en.wikipedia.org/wiki/Minimum_viable_product



https://en.wikipedia.org/wiki/Agile_software_development



https://en.wikipedia.org/wiki/Programming_paradigm

