This package is intended to patch certain files on the local debian installation
and keep them patched throughout the constant system updates. It is fed with a
bunch of diff files (separate diff for every patch we maintain) and automatically
creates the proper dpkg triggers. Every time the system installs a new version on top
of the patched file, the corresponding trigger is fired calling the maintainer's
script, which applies the patch again.
