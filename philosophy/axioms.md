# Development Axioms For All Projects

**These axioms are only for specific projects that I myself build and maintain.  These rules work for me, personally.  These are not standard definitions, these are context dependent within my own working environment.**


1. Maximize for ease of readability, then simplicity, then brevity.
2.  Comments give pause for a written second thought.  That is their primary purpose, not documentation.  An out of date comment is worth its cost, paid in forced contemplation.
3.  A project is a contained folder that is organized to reflect a distinct development purpose.
4.  A runnable is a piece of software which can be invoked as a process.
5.  A plugin is a piece of software which can be loaded by a runnable.
6.  A library is a buildable code base containing exported classes.
7.  A deployment is the distribution, configuration, and orchestration of a project to/in an environment.
8.  A package is the combination of any built code and static resources.
9.  All projects should aim to limit external dependencies.
10. All projects should remain separate except in linkage and packaging.
11. Utility Projects should contain functions which can be shared between libraries.
12. Library Projects should contain classes and should never operate as a runnable.
13. Runnable Projects should be an implementation of outside library classes.  Care should be taken to ensure that runnable projects hold only project specific implementations of existing classes.
14. Plugin Projects should all use the same loader classes for all runnable projects.
15. Static File Projects contain static files which may be incorporated by various projects.
16. Package Builder Projects build packages from other project types.
17. Deployment Projects only deploy packages to environments; any other function is out of their scope.
18. Deployment Projects should be entirely separate from Package Builder Projects (and vice versa).
19. All packages should be buildable with a single command.
20. All deployments should be deployable with a single command.
21. Where reasonable, administration and moderation tools should be developed to work only out of band to minimize attack surface.
22. Unit tests ought to be used only where important and meaningful.
23. All web projects should incorporate the strictest CSP policy as a baseline.

