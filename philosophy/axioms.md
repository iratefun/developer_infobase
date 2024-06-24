# Development Axioms For All Projects

**These axioms are only for JavaScript projects that I myself build and maintain.  These rules work for me, personally.  They may not work for you.**

1. Code, static resources, and build utilities should all remain separate.
2. A project is a contained folder that is organized to reflect a distinct purpose.
3. A runnable is a piece of software which can be invoked as a process.
4. A library is a buildable code base containing exported classes.
5. A deployment is the distribution, configuration, and orchestration of a project to an environment.
6. A package is the combination of any built code and static resources.
7. All projects should aim to limit external dependencies.
8. Library Projects should contain classes and should never function as a runnable.
9.  Runnable Projects should be a runnable implementation of outside library classes.  Care should be taken to ensure that runnable projects hold only project specific implementations of existing classes.
10. Static File Projects contain static files which may be incorporated by various projects.
11. Package Builder Projects build packages from other project types.
12. Deployment Projects are deploy packages to environments.
13. Deployment Projects should be entirely separate from Package Builder Projects (and vice versa).
14. All Package Builder Projects should be buildable with a single command that executes all of them sequentially.
15. All deployments should be deployable with a single command.
16. Maximize readability, then simplicity, then brevity.
17. Where reasonable, administration tools should be developed to work only out of band.
18. Unit tests are not a way of life, they ought to be used only where important and meaningful.

