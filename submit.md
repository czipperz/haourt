# How to submit

1. Fork haourt

2. Write a PKGBUILD. Contact me if you need help.

3. You **WILL NEED an install file** (in the format `<pkgname>.install`)
that has a (function) `post_install()` with at least these two lines in the body (drop the `-R` for files):

    sudo chown -R $_whoami $_HOME/<directory-installed-to>
    sudo chgrp -R $_whoami $_HOME/<directory-installed-to>

3. Build your project to make sure it works (`makepkg -sci`).
Make sure that your package has its check sums (`makepkg -g >> PKGBUILD` to generate).

4. Run `makepkg -S` and add the name of the file generated to the `mirrorlist`.
Put the resulting package in the packages folder.

5. Submit a pull request in the fashion: `New Package: <package name>`
