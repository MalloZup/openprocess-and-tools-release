# Freebsd Release engineering

https://www.freebsd.org/releng/

Freebsd Release Engineering: https://www.freebsd.org/doc/en_US.ISO8859-1/articles/freebsd-releng/index.html

# Branching terminology:

- `head`:  reflects the top of the source tree.
- `stable`: this is after testing head ( The default minimum timeframe before merging to stable/ branches is three (3) days)
- `official`: After several months, and the number of changes in the stable/ branch have grown significantly, release the next version of FreeBSD. These releases have been historically referred to as “point” releases.


## Notable Practices/Workflow:

Freebsd uses the term "the Code Slush", when the release date is approaching, for just bugfixing instead of introducing new features.

From their doc:
"Although the code slush is not a hard freeze on the tree, the FreeBSD Release Engineering Team requests that bugs in the existing code base take priority over new features"
The code slush does not enforce commit approvals to the branch.

After the "Code Slush", comes the Code Freeze, this  marks the point in time where all changes, require explicit approval from the FreeBSD Release Engineering Team.


