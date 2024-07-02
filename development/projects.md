# Projects

## Project Folder Naming convention

Project folders should utilize the following convention: project_prefix__project_name__project_type_suffix__optional_tailings

Example: 
* prcr__custom__util
* ptusa__audit_cluster__run

## Project Prefixes

A project prefix should always be an organizational name.  It should strive to be a sortable, recognizable, organizational classification.

### PRCR

Projects prefixed with prcr/PRCR are core projects (project core).  These are used as a
baseline to build other projects.

### PTUSA

Projects prefixed with ptusa/PTUSA are projects developed for the previously valid, pentestusa entity.  That entity is currently disolved, making the ptusa prefix present, but invalid. 

### IRF/IRATEFUN

Projects prefixed with irf/IRF/iratefun/IRATEFUN are my current personal projects.

### MITMMOD

MITM Modular Proxy project prefix.


## Project Names

A project name should be a lowercase, underscore separated, name.

## Project Type Suffixes

A project type suffix should always be a project type classification.  The lists below shows the current generic and specific project types represented.  Specific project types are defined according to their own obviously-unique purpose.  A project type specification should be avoided if a generic type fits more accurately.

### Generic Project Types
* __static: static files
* __util: utility function library
* __lib: class library
* __runnable: runnable program project
* __plugin: plugin project (extends functionality to a runnable)
* __builder: builds a library or runnable.
* __manufacturer: runs multiple builders (manufacturers)
* __deployer: runs a deployment
* __orchestrator: orchestrates deployments.
* __conductor: conducts orchestrations.

### Application Specific Project Types
* __spokesite: A website build to be imported within the spoke webserver.


## Project Optional Tailings

Project optional tailings should be avoided where possible, but sometimes, they become necessary to distinguish between packages.  They are project dependent, and are not deterministically parsable by default.
