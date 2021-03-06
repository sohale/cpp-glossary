Meta:
# Scaffolding the principles

Meta: Scaffolding the principles:

Motivation:
Let's create a scaffold on these concerete learnings.
These are not design patterns. More than that: more clear cut, minimal, abstract, deep and simple, almost mathematical.
This is to be able to talk about these (communicate, interview, show competence).
* Abstractions to organise LTM learnings, Implicit knowledge (rather than a "flat set" linke linux).
   * To: consolidate them, make them explicit, make them tangible (almost like concrete).
* Start with C++ principles. But they are almost univdersal
   * At least universal across C++ and Java, until next paradigm disruption.  (Some not? In that case, find their roots in GIL.)
   * There are not OOP principles.
   * We have two levels of OOP: 1. OOP principles, 2. OOP as unfolded historically in its implementation: C++, Java, and probably Simula. Smalltalk is more essntial (further from these). Technical.
   * Three levels: 1. OOP in principle 2. OOP as Simula 3. OOP in essense (GIL)
   * Other levels: GIL in general: Any code/info system (which obvious will need a detials implementation as mechanism , defined in aan explicit communicaatable (with oither intelligent-design-ers) language, will need this).

Here I write things that I want to remember but could not very well. (I can use it to revise before ...). Bad memory => robustness (see below).
More importantly, these exist in my mind (LTM) "before" I put them here.
Or they preexist (before writing here) in a distributed close-style decentralised collective memory. (And this one will become part of the decentralised. But not only decentralised, but also "hard" and "stiff". ( #GIL).

* (Also [see](./cpp-glossary.md##phrases))


## C++ concrete acronyms
(initialism)
### SFINAE
* Substitution failure is not an error (SFINAE)
### RAII
* RAII (resource acquisition is initialization)
[pronunciation](https://stackoverflow.com/questions/99979/how-do-you-pronounce-raii)

Also known as Constructor Acquires, Destructor Releases (CADRe) [see](https://en.wikipedia.org/wiki/Resource_acquisition_is_initialization)

A sub-type of RAII is SBRM (Scope-based Resource Management). [link](https://en.wikipedia.org/wiki/Resource_acquisition_is_initialization)

### CADRe
Constructor Acquires, Destructor Releases. Another name for RAII. See [RAII]


### Other C++ concepts
Dangling concepts not in above list.
CADRe, SBRM

### Other things to separate out
So that they don't distract the above.
These are not technical.
(code smells, deisgn problems, etc)

* Don’t Repeat Yourself
* Tell Don’t Ask [see](https://deviq.com/encapsulation/)
* Flags Over Objects [see](https://deviq.com/encapsulation/)

### Candidates for GIL-level
( #GIL )
* DRY
* A written principle much be used by more than one person. Hence, if you search FOO, if the website is down, you will findd the meaning (like robustness by "clone"s).
* Mutiple eyeballs (Multiple IDs) => Code, not connectionist. Also it means (need for) explainability.
Aalso teachability. you must be able to teach everything: you must be able to write about it clearly in stackoverflow, talk about it in aislees of Acadedmy in Athens. A good professor teaches also.
* Bad memory => more robustness. (also Netflix's stress test: deflectiopn test, perturbation (perturbation test), knock-it-off, ebrace-change in Agile, etc.
