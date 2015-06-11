# How to submit

1. Fork haourt
2. Build a PKGBUILD. Contact me if you need help.
You WILL NEED an install file (in the format `<pkgname>.install`) that has a `post_install()` with at least these two lines in the body:
`sudo chown -R $(whoami) $HOME/<directory-installed-to>` and
`sudo chgrp -R $(whoami) $HOME/<directory-installed-to>`.
3. Build your project to make sure it works (`makepkg -sci`).
Make sure that your package has its check sums (`makepkg -g >> PKGBUILD` to generate).
4. Add your package to `mirrorlist` in the convention used and put the tarball (that `makepkg -S` generates) into the packages folder.
5. Submit a pull request in the fashion: `New Package: <package name>`
