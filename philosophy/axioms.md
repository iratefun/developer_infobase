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
9. A builder is a project designed to be used by a manufacturer to build packages.
10. A manufacturer operates one or more builders to build packages.
11. A deployment is the distribution, configuration, and integration of a project to/in an environment.
12. An orchestration is multiple deployments.
13. An orchestra manages orchestrations.
14. A conductor manages orchestras.
15. Projects should aim to limit external dependencies.
16. Projects should remain separate except in linkage and packaging.
17. Utility Library Projects should contain functions which can be shared between libraries.
18. Class Library Projects should contain classes and should never operate as a runnable.
19. Runnable Projects should be an implementation of outside library classes.  
20. Runnable projects only hold (read: not link, but actually contain the files for) project specific implementations of their classes.
21. All projects should use the same loader classes for all things: eg. libraries, plugins, and dependencies.
22. All projects should use the same API conventions (for both websocket and POST APIs).  We use WebServerRoute.respondError and respondJSON which notates data to our standard.
23. All POST APIs should share the same data validation mechanisms (DataValidators.class.js)
24. Static file projects contain static files which may be incorporated by various projects.
25. Builder projects build packages from other project types.
26. Deployment projects only deploy packages to environments; any other function is out of their scope.
27. Orchestra projects only orchestrate over their defined dominion.
28. Conductor projects only conduct orchestrations in their defined dominion.
29. Deployment projects should be entirely separate from Package Builder Projects (and vice versa).
30. All packages should be buildable with a single command.
31. All deployments should be deployable with a single command.
32. Administration and moderation tools should be developed to work ***only*** out of band to minimize attack surface.
33. Unit tests ought to be used only where important and meaningful.
34. All web projects should incorporate the strictest CSP policy as a starting baseline.
35. Always be suspicious of code, and the people that write it.
36. A hash is the index for unique data.
37. A UUID is the index for unordered data.
38. An integer is the index for asc/desc-ending data.
39. All database records must be cross referencable with the project uuid that inserted it.
40. Enigmatic ideas, labels, and conventions are useless outside of marketing.
41. Avoid SQL, it is useful, and performant, but its cost in maintainence and data transformation is painful.
42. A runnable must either be packagable as an electron app, or a node single-executable-application.
43. All projects should share a parent node_modules directory for development. (workspace/software/git_controlled/node_modules/)
44. A node_modules can be added to a project, but care must be taken to ensure this is ***absolutely*** required.
45. Runnable entrypoints are async functions: (async function(){...})()
46. Libraries are loaded by importing an async function named load().
47. Avoid opaque definitions.  Define in rigid semantics.
48. Definitions should seek to be natural.
49. process.project_core contains shared process resources.  
50. All processes, workers, and threads have their own process.project_core.
51. process.project_core.deps contains loaded dependencies (such as those loaded via require/import).
52. The developers role is sarcosanct to any success.
53. All runnable projects import the prcr__custom_utilities__util library as a first library. 
54. All projects must have a unique UUID value that never changes.
55. All projects and databases must have a documentation page, no exceptions.
56. Stress and work are not the same thing.  Beware of any who would add stress to work, as it is allegorical to poisoning.
57. I would rather one large library than many smaller ones.
58. All classes that are not explictly and wholely proprietary to a project, should ONLY live in the prcr__class__lib project.
59. Be patient with the vestigial.  It takes time to disappear, but it should be sought to disappear.
60. All class names in a project should be distinct and not repeating.
61. Organization can be studied, and study makes knowledge tennable.
62. Projects that require a configuration file, should be capable of also generating configuration file templates for users to expand on.
63. Objects should use always named self-references instead of "this."
64. All runnables share a standard entry point (prcr__runnable_entry_point__util)
65. Configuration parsers should be within prcr__class__lib.  Projects ought not hold their own config parsers.  This is so other projects can import configurations without having to look into a runnable source.
66. If the project is a runnable, it should have only one ProjectCoreRunnable instance, and it should be available in process.project_core.runnable.
67. Always consider the dimensionality of what "better" means.
68. Work in immediacy, only with what you have.
69. Work for the sake of accomplishment, even if none celebrate those wins.
70. Innate failings and shortcomings are not an excuse to drown.
71. Configuration files are nearly always better as configuration scripts.
72. Configuration scripts are almost always dangerous.
73. It is not a sin to give code execution to those who ought be able to execute code.
74. It is always a sin to give code execution to those which should not have it.
75. All non-sensitive development environment variables go in "/etc/bash.bashrc".
76. A workstation has a workspace.  That workspace is a folder.  That folder is defined in "/etc/bash.bashrc".  Most workspace tools reference $WORKSPACE_DIR in one way or another, so this variable must be set.  The preferred spot for this folder is "~/workspace/".
77. Obtuse configuration files are anathema to a new user.  Always make tools run immediately unless pre-configurations are absolutely required (eg database/other credentials).
