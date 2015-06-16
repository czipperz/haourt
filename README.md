# HAOURT

The goal of this project is to easily distribute PKGBUILDs for Arch Linux that install into $HOME.

**Usage**

**haourt** is a package that allows for wrapping of *PKGBUILDs* into `pacman` for `$HOME` installs

**Sync options:**

<pre><ul>
<li> `-S`   => Install one or more package(s) </li>
<li> `-Ss`  => Search with fgrep </li>
<li> `-Ssr` => Search with egrep </li>
<li> `-Sy`  => Update the mirrorlist </li>
<li> `-Su`  => Update the packages (based on the local mirrorlist) </li>
<li> `-Syu` => Update the mirrorlist and packages </li>
<li> `-Sw`  => Downloads, extracts and modifys the package so that you can just `makepkg -sci` it/them </li>
<li> `-Sww` => Downloads the package(s) </li>
</ul></pre>

**Query options**

<pre><ul>
<li> `-Q`   => Print the package and its version as it is locally (or a list of all installed packages and their versions if no args given) </li>
<li> `-Qs`  => Search installed packages with fgrep </li>
<li> `-Qsr` => Search installed packages with egrep </li>
</ul></pre>

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
