# Development Axioms For All Projects

**These axioms are only for specific projects that I myself build and maintain.  These axioms work for me, personally.  These are not standard definitions, these are context dependent within my own working environment and lived experience.**


1. Maximize for ease of readability, then simplicity, then brevity.
2. Code duplication is a grevious sin.
3. Comments give pause for a written second thought.  That is their primary purpose.
4. A project is a contained folder that is organized to reflect a distinct development purpose.
5. A runnable is a buildable project which can be invoked as a process.
6. A plugin is a buildable project which can be loaded by a runnable.
7. A library is a buildable project containing exported/importable/linkable classes or code.
8. A package is the combination of any built code and/or static resources.
9. A builder is a project designed to be used by a manufacturer to create packages.
10. A manufacturer operates one or more builders to build packages.
11. A deployment is the distribution, configuration, and integration of a project to/in an environment.
12. An orchestration is multiple deployments.
13. An orchestra manages orchestrations.
14. Projects should aim to limit external dependencies.
15. Projects should remain separate except in linkage and packaging.
16. Utility Library Projects should contain functions which can be shared between libraries.
17. Class Library Projects should contain classes and should never operate as a runnable.
18. Runnable Projects should be an implementation of outside library classes.  Care should be taken to ensure that runnable projects hold only project specific implementations of existing classes.
19. Plugin Projects should all use the same loader classes for all runnable projects.
20. Static File Projects contain static files which may be incorporated by various projects.
21. Package Builder Projects build packages from other project types.
22. Deployment Projects only deploy packages to environments; any other function is out of their scope.
23. Orchestra Projects only orchestrate over their defined dominion.
24. Conductor Projects only conduct orchestrations in their defined dominion.
25. Deployment Projects should be entirely separate from Package Builder Projects (and vice versa).
26. All packages should be buildable with a single command.
27. All deployments should be deployable with a single command.
28. Administration and moderation tools should be developed to work only out of band to minimize attack surface.
29. Unit tests ought to be used only where important and meaningful.
30. All web projects should incorporate the strictest CSP policy as a baseline.
31. Always be suspicious of code, and the people that write it.
32. A hash is often, but not always, the best index.
33. Enigmatic ideas, labels, and conventions are useless outside of marketing.
34. Avoid SQL, it is useful, and performant, but its cost in maintainence and data transformation is painful.
35. A runnable must either be packagable as an electron app, or a node single-executable-application.
36. All projects should try to share a parent node_modules directory for development. (workspace/software/git_controlled/node_modules/)
37. Runnable entrypoints should be async functions: (async function(){...})()
38. Libraries should be loaded by importing an async function symbol named load().
39. Avoid opaque definitions.  Define in rigid, quasi mathematical terms.
40. Definitions should seek to be natural.
41. process.irf_core contains shared process resources.  The name was chosen arbitrarily to be distinct.
42. process.irf_core.deps contains loaded dependencies (such as those loaded via require/import).
43. Dependencies should propagate through library loads.
44. Seek to make the developers life more streamlined; their role is sarcosanct to any success.
