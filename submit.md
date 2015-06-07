# How to submit

1. Fork haourt
2. BUILD YOUR PROJECT TO MAKE SURE IT WORKS (`makepkg -sci`).
Make sure that your package has its check sums (`makepkg -g >> PKGBUILD` to generate).
3. Add your package to `mirrorlist` in the convention used and put the tarball (that `makepkg -S` generates) into the packages folder.
4. Submit a pull request in the fashion: `New Package: <package name>`
