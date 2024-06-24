# Development Axioms For All Projects

1. Code, static resources, and build utilities should all remain separate.
2. All projects should aim to limit dependencies.
3. Library Projects should contain utility classes.
4. Runnable Projects should be a runnable implementation of outside library classes.  Care should be taken to ensure that runnable projects hold only project specific implementations of existing classes.
5. Static File Projects contain static files which may be incorporated by various projects.
6. Package Builder Projects build packages of other project types.
7. Deployment Projects are created specifically for the purposes of deploying packages to various environments.
8. Deployment should be separate from building, and should be dynamic.
9. A package is the combination of any built code and static resources.
10. All packages should be buildable with a single command.
11. Maximize readability, then simplicity, then brevity.
12. Where reasonable, administration tools should be developed to work only out of band.

