# Development Axioms For All Projects

**These axioms are only for JavaScript projects that I myself build and maintain.  These rules work for me, personally.  They may not work for you.**

1. Code, static resources, and build utilities should all remain separate.
2. All projects should aim to limit dependencies.
3. Library Projects should contain utility classes.
4. Runnable Projects should be a runnable implementation of outside library classes.  Care should be taken to ensure that runnable projects hold only project specific implementations of existing classes.
5. Static File Projects contain static files which may be incorporated by various projects.
6. Package Builder Projects build packages of other project types.
7. Deployment Projects are created specifically for the purposes of deploying packages to various environments.
8. Deployment Projects should be entirely separate from Package Builder Projects (and vice versa).
9.  A runnable is a piece of software which can be invoked as a process.
10. A library is a buildable code base containing exported classes.
11. A deployment is the distribution, configuration, and orchestration of a project.
12. A package is the combination of any built code and static resources.
13. All packages should be buildable with a single command.
14. All deployments should be deployable with a single command.
15. Maximize readability, then simplicity, then brevity.
16. Where reasonable, administration tools should be developed to work only out of band.

