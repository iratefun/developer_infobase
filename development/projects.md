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



## Project Names

A project name should be a lowercase, underscore separated, name.

## Project Type Suffixes

A project type suffix should always be a project type classification.  The list below shows the current project types represented.

* __static
* __util
* __lib
* __runnable
* __plugin
* __builder
* __manufacturer
* __deployer
* __orchestrator
* __conductor


## Project Optional Tailings

Project optional tailings should be avoided where possible, but sometimes, they become necessary to distinguish between packages.  They are project dependent, and are not deterministically parsable by default.
