# Freebsd Release engineering

https://www.freebsd.org/releng/

Freebsd Release Engineering: https://www.freebsd.org/doc/en_US.ISO8859-1/articles/freebsd-releng/index.html


# Open questions/research needed:

- [ ] CI systems. Is the CI system phabricator or other tools are in place (jenkins etc)
- [ ] is there any comprensive list of tools which migh help on releasing/automated the process?

# Code Source/hosting:

Freebsd uses https://reviews.freebsd.org/ for reviwing modification of pkgs and code.

The platform is [phabricator](https://www.phacility.com/phabricator/)


# Build System:

Freebsd used a build system which is integrated to the source code web interface 

[phabricator](https://www.phacility.com/phabricator/). For more information check https://secure.phabricator.com/book/phabricator/article/harbormaster/.

# Bug tracker:

- bugzilla: https://bugs.freebsd.org/bugzilla/

 TO research: is there any automation between bugzilla and phabricator? Like one reference bug report and once it is merged on phabricators bug is closed or something similar.

# Processes:

As many others distrubutions UNIX/LINUX and software projects, freebsd uses `Milestones` https://www.freebsd.org/doc/en_US.ISO8859-1/articles/freebsd-releng/releng-prep.html.


## Branching terminology:

- `head`:  reflects the top of the source tree.
- `stable`: this is after testing head ( The default minimum timeframe before merging to stable/ branches is three (3) days)
->`official`: After several months, and the number of changes in the stable/ branch have grown significantly, release the next version of FreeBSD. These releases have been historically referred to as “point” releases.


## Notable Practices/Workflow:

- `Code Slush`:

Freebsd uses the term the Code Slush, when the release date is approaching, for just bugfixing instead of introducing new features.

From their doc:
"Although the code slush is not a hard freeze on the tree, the FreeBSD Release Engineering Team requests that bugs in the existing code base take priority over new features"
The code slush does not enforce commit approvals to the branch.

After the "Code Slush", comes the Code Freeze, this  marks the point in time where all changes, require explicit approval from the FreeBSD Release Engineering Team.

