# HAOURT

The goal of this project is to easily distribute PKGBUILDs for Arch Linux that install into $HOME.

##Usage

**Sync options:**

* `-S`   => Install one or more package(s)
* `-Ss`  => Search with fgrep
* `-Ssr` => Search with egrep
* `-Sy`  => Update the mirrorlist
* `-Su`  => Update the packages (based on the local mirrorlist)
* `-Syu` => Update the mirrorlist and packages
* `-Sw`  => Downloads, extracts and modifys the package so that you can just `makepkg -sci` it/them
* `-Sww` => Downloads the package(s)

**Query options**

* `-Q`   => Print the package and its version as it is locally (or a list of all installed packages and their versions if no args given)
* `-Qs`  => Search installed packages with fgrep
* `-Qsr` => Search installed packages with egrep

**Remove packages using -R**

To submit a package, see *<https://github.com/czipperz/haourt/blob/master/submit.md>*

## Installation

**NOTE THAT IT IS NOT FULLY WRITTEN YET**

Arch Linux:

	curl -L https://raw.githubusercontent.com/czipperz/haourt/master/install | bash

Not for use on non arch systems.

**BUILDING OF PACKAGES MUST BE AS DONE AS THE USER YOU WANT TO INSTALL AS**

## Contributing

See `submit.md`
