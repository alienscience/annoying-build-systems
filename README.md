# Annoying Build Systems

Many people complain about many build (and packaging) systems.
This repo tries to collect the annoyances
in a similar fashion to
[awesome lists](https://github.com/sindresorhus/awesome).

To contribute, send pull requests.
The Licence for this repo is [CC0](https://creativecommons.org/publicdomain/zero/1.0/).

## Builds Systems and their Annoyances

### Ant

* Looks like Make with XML syntax

### Bazel

### Buck

### Cabal

### CMake

* Custom language

### Gradle

### Grunt

### Jam

### Make

* [Recursive Make Considered Harmful](http://www.lateralt.net/files/auug97.pdf)
* Changes to the Makefile to do not implicitly trigger rebuilds
* Dependencies on directories is not really possible
* Lots of output by default
* Rules with multiple output files are not really possible

### Maven

* Restricting [build lifecycle concept](https://maven.apache.org/guides/introduction/introduction-to-the-lifecycle.html)
* Throws Null Pointer Exceptions and gives a stack trace for simple errors such as missing parameters
* Verbose logs
* Uses XML (possibly annoying), does not support XML attributes (annoying)

### Meson

### MS Build

### Ninja

* Very low-level

### NPM

* `npm install` [can be dangerous](https://github.com/joaojeronimo/rimrafall)
* [Replicates transitive dependencies](https://lexi-lambda.github.io/blog/2016/08/24/understanding-the-npm-dependency-model/)

### Python Pip

* The `requirements.txt` can either contain
  the (small) set of direct dependencies
  or the set of all (transitive) requirements for better repeatability.

### Rake

### SBT

* Very slow
* Builds a directory tree on startup. If SBT is started in the `/` directory it [runs out of memory](https://github.com/sbt/sbt/issues/1458)
* Uses a hard to understand [multilayered mutable execution model](http://www.lihaoyi.com/post/SowhatswrongwithSBT.html)

### Scons

### Shell Scripts

* Hard to port
* Hard to parallelize (thus slow)
