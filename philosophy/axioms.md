# Development Axioms For All Projects

**These axioms are only for specific projects that I myself build and maintain.  These rules work for me, personally.  These are not standard definitions, these are context dependent within my own working environment.**

1. A project is a contained folder that is organized to reflect a distinct development purpose.
2. A runnable is a piece of software which can be invoked as a process.
3. A library is a buildable code base containing exported classes.
4. A deployment is the distribution, configuration, and orchestration of a project to an environment.
5. A package is the combination of any built code and static resources.
6. All projects should aim to limit external dependencies.
7. All projects should remain separate except in linkage and packaging.
8. Utility Projects should contain functions which can be shared between libraries.
9. Library Projects should contain classes and should never operate as a runnable.
10. Runnable Projects should be an implementation of outside library classes.  Care should be taken to ensure that runnable projects hold only project specific implementations of existing classes.
11. Static File Projects contain static files which may be incorporated by various projects.
12. Package Builder Projects build packages from other project types.
13. Deployment Projects deploy packages to environments.
14. Deployment Projects should be entirely separate from Package Builder Projects (and vice versa).
15. All packages should be buildable with a single command.
16. All deployments should be deployable with a single command.
17. Maximize for readability, then simplicity, then brevity.
18. Comments give pause for a written second thought.  That is their primary purpose, not documentation.  An out of date comment is worth its cost, paid in prior contemplation.
19. Where reasonable, administration and moderation tools should be developed to work only out of band to minimize attack surface.
20. Unit tests ought to be used only where important and meaningful.
21. All web projects should incorporate the strictest CSP policy as a baseline.

