# Development Axioms For All Projects

**These axioms are only for specific projects that I myself build and maintain.  These axioms work for me, personally.  These are not standard definitions, these are context dependent within my own working environment and lived experience.**


1. Maximize for ease of readability, then simplicity, then brevity.
2. Code duplication is a grevious sin.
3.  Comments give pause for a written second thought.  That is their primary purpose, not documentation.  An out of date comment is worth its cost, paid in forced contemplation.
4.  A project is a contained folder that is organized to reflect a distinct development purpose.
5.  A runnable is a buildable project which can be invoked as a process.
6.  A plugin is a buildable project which can be loaded by a runnable.
7.  A library is a buildable project containing exported/importable/linkable classes or code.
8.  A package is the combination of any built code and static resources.
9.  A deployment is the distribution, configuration, and integration of a project to/in an environment.
10. An orchestration is multiple deployments.
11. An orchestra manages orchestrations.
12. All projects should aim to limit external dependencies.
13. All projects should remain separate except in linkage and packaging.
14. Utility Library Projects should contain functions which can be shared between libraries.
15. Class Library Projects should contain classes and should never operate as a runnable.
16. Runnable Projects should be an implementation of outside library classes.  Care should be taken to ensure that runnable projects hold only project specific implementations of existing classes.
17. Plugin Projects should all use the same loader classes for all runnable projects.
18. Static File Projects contain static files which may be incorporated by various projects.
19. Package Builder Projects build packages from other project types.
20. Deployment Projects only deploy packages to environments; any other function is out of their scope.
21. Orchestra Projects only orchestrate over their defined dominion.
22. Conductor Projects only conduct orchestrations in their defined dominion.
23. Deployment Projects should be entirely separate from Package Builder Projects (and vice versa).
24. All packages should be buildable with a single command.
25. All deployments should be deployable with a single command.
26. Administration and moderation tools should be developed to work only out of band to minimize attack surface.
27. Unit tests ought to be used only where important and meaningful.
28. All web projects should incorporate the strictest CSP policy as a baseline.
29. Always be suspicious of code, and the people that write it.
30. A hash is often, but not always, the best index.
31. Enigmatic ideas, labels, and conventions are useless outside of marketing.
32. Avoid SQL, it is useful, and performant, but its cost in maintainence and data transformation is painful.
33. A runnable must either be packagable as an electron app, or a node single-executable-application.
