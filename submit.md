# How to submit

1. Fork haourt

2. Write a PKGBUILD. Contact me if you need help.
You WILL NEED an install file (in the format `<pkgname>.install`)
that has a `post_install()` with at least these two lines in the body:
`sudo chown -R $(whoami) $_HOME/<directory-installed-to>` and
`sudo chgrp -R $(whoami) $_HOME/<directory-installed-to>`.
Note that you use `$_HOME` because the install file is ran as root
(therefore `$HOME` in the install file is `/root` while `$HOME` in the PKGBUILD is `/home/<username>`.

3. Build your project to make sure it works (`makepkg -sci`).
Make sure that your package has its check sums (`makepkg -g >> PKGBUILD` to generate).

4. Run `makepkg -S` and add the name of the file generated to the `mirrorlist`

5. Submit a pull request in the fashion: `New Package: <package name>`
