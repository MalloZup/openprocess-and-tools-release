# openprocess-and-tools-release

# Community:

https://gitter.im/MalloZup-openprocess-and-tools-release/community


# Goals:

- [ ] Document how opensource Distro and Companies do Software release engineering.
- [ ] Create a community of people who are interested and active work on some subjects or help other maintainers/communities.

Rationale:

The aim of openprocess-and-tools-release is to share knowledge about **Releasing Software**.
It is a curated documentation about release process, tools, workflows, best practices used for Releasing sofware in the opensource world.



# Release engineering:

* [Freebsd Release engineering](doc/freebsd.md)

* [Archlinux Release engineering](doc/archlinux.md) Status: WIP

* [Reproducible builds](https://reproducible-builds.org) 
  Reproducible builds are a set of software development practices that create an independently-verifiable path from source to binary code
 
  

# How to research/standards:

Note: this question could change when the projects becomes more mature.
Take this question as guideline when you want to investigate/research on Release engineering practices for X project.


- What are the process for a release from the smallest one, (package building) to the higher level one (distrubution, Projects like kernels etc?)
- What is the build-system/or how is software built and integrated with source code?
- Where it the code hosted? Same build-system platform or other?
- How bugs are handled? Bugzilla or any other integration/automation workflow?
- What are the best-practices/releases workflow? 
- What is the testing system/CI if there is only 1, or how the project handles CI from the minimal to largest part? Example: in a distro, CI for X package differs to the "global" CI of the distro.
- How is the integration of all of this tools, are existing any tools documentation/automation?
- How the project handle semver or is using other or additional practices for breaking changes and updates?

# Contributing:

I have opened a few issues for contributors.

In the normal case, if you have any idea/proposal, feel free to open an issue **before sending PRs** to discuss the rationale.


### Note

Software should be driven by rationale and scope.

So this repo is not just a bare list of X tools for release. 

Instead we should focus more on problems/scope and documentation.
