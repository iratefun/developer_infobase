# Development Axioms For All Projects

**These axioms are only for specific projects that I myself build and maintain.  These axioms work for me, personally.  These are not standard definitions, these are context dependent within my own working environment and lived experience.**


1. Maximize for ease of readability, then simplicity, then brevity.
2.  Comments give pause for a written second thought.  That is their primary purpose, not documentation.  An out of date comment is worth its cost, paid in forced contemplation.
3.  A project is a contained folder that is organized to reflect a distinct development purpose.
4.  A runnable is a buildable project which can be invoked as a process.
5.  A plugin is a buildable project which can be loaded by a runnable.
6.  A library is a buildable project containing exported classes.
7.  A package is the combination of any built code and static resources.
8.  A deployment is the distribution, configuration, and integration of a project to/in an environment.
9.  An orchestration is multiple deployments.
10. An orchestra manages orchestrations.
11. All projects should aim to limit external dependencies.
12. All projects should remain separate except in linkage and packaging.
13. Utility Projects should contain functions which can be shared between libraries.
14. Library Projects should contain classes and should never operate as a runnable.
15. Runnable Projects should be an implementation of outside library classes.  Care should be taken to ensure that runnable projects hold only project specific implementations of existing classes.
16. Plugin Projects should all use the same loader classes for all runnable projects.
17. Static File Projects contain static files which may be incorporated by various projects.
18. Package Builder Projects build packages from other project types.
19. Deployment Projects only deploy packages to environments; any other function is out of their scope.
20. Deployment Projects should be entirely separate from Package Builder Projects (and vice versa).
21. All packages should be buildable with a single command.
22. All deployments should be deployable with a single command.
23. Administration and moderation tools should be developed to work only out of band to minimize attack surface.
24. Unit tests ought to be used only where important and meaningful.
25. All web projects should incorporate the strictest CSP policy as a baseline.
26. Always be suspicious of code, and the people that write it.
27. A hash is often, but not always, the best index.
28. Enigmatic ideas, labels, and conventions are useless outside of marketing.
29. Avoid SQL, it is useful, and performant.
