# HAOURT

The goal of this project is to easily distribute PKGBUILDs for Arch Linux that install into $HOME.

##Usage

**haourt** is a package that allows for wrapping of *PKGBUILDs* into `pacman` for `$HOME` installs

###Sync options:

*  -S   => Install one or more package(s)\n
*  -Ss  => Search with fgrep\n
*  -Sy  => Update the mirrorlist\n
*  -Su  => Update the packages (based on the local mirrorlist)\n
*  -Syu => Update the mirrorlist and packages\n
*  -Sw  => Downloads, extracts and modifys the package so that you can just \`makepkg -sci\` it/them\
*  -Sww => Downloads the package(s)\n

###Query options

*  -Q   => Will print the package and its version as it is locally
*  -Qs  => Will print the package and its version that matches a search query

###Remove packages using -R

###To submit a package, see *<https://github.com/czipperz/haourt/blob/master/submit.md>*

## Installation

**NOTE THAT IT IS NOT FULLY WRITTEN YET**

Arch Linux:

	curl -L https://raw.githubusercontent.com/czipperz/haourt/master/install | bash

Not for use on non arch systems.

**BUILDING OF PACKAGES MUST BE AS DONE AS THE USER YOU WANT TO INSTALL AS**

## Contributing

See `submit.md`
