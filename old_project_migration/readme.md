# Old Project Migrations

While I'm considering these projects "old," most of them are still modern.  The term "old" in this context, means projects which are disjointed to our current list of axioms.  Projects which were designed, implemented, and work, but do not follow rhyme or reason with regards to each other.  The migration goal, is to consolidate all code into a usable set of libraries and runnables which can much easier be pulled from for the sake of invention and development.

Old projects should be migrated before any new development takes place.

## Project Directories

Core projects should be migrated first.

* SpokeWebServer

Since the iratefun website project is the most modern, and pressing project, we will migrate those projects next.

* iratefun_utility_classes
* iratefun_tooling
* iratefun_website
* iratefun_mitmproxy_plugins  

PentestUSA projects are fairly large, and contain very useful code, but due to the organization being defunction/disolved we'll be migrating those projects after iratefun projects.  Of special note, we have the auditcluster websocket api server, which allows for simultaneous event driven controls to utilize a single connection using a system of trancievers. We want to separate that functionality into it's own standalone project, similar to the SpokeWebServer.

* ptusa_utility_classes
* ptusa_audit_cluster_v2
* ptusa_deployment_tool
* ptusa_scriptrunner
* ptusa_alexander
* ptusa_audit_cluster_v2__worker_thread_apis
* ptusa_microservices
* ptusa_shared_library_v2
* ptusa_app_server
* ptusa_cdp_client
* ptusa_microservice__skeleton_project
* ptusa_audit_cluster_client_v2_unit_tests
* ptusa_cdp_client_modified_during_pentest
* ptusa_pentest_client_v2

WebAnythingStudio is an older module-driven electron application designed for performing web automation tasks using puppeteer.  It's an interesting project, which should be ported and absorbed into our class libraries.

* WebAnythingStudio
* WebAnythingStudioExampleModules

The remaining projects are miscelaneous projects.

* letsencryptserver

### iratefun_mitmproxy_plugins

|----------------|-----------|
|migration state | unstarted |


### letsencryptserver

|----------------|-----------|
|migration state | unstarted |

### ptusa_audit_cluster_v2

|----------------|-----------|
|migration state | unstarted |

### ptusa_deployment_tool

|----------------|-----------|
|migration state | unstarted |

### ptusa_scriptrunner

|----------------|-----------|
|migration state | unstarted |


### WebAnythingStudio

|----------------|-----------|
|migration state | unstarted |

### iratefun_tooling

|----------------|-----------|
|migration state | unstarted |

### ptusa_alexander

|----------------|-----------|
|migration state | unstarted |

### ptusa_audit_cluster_v2__worker_thread_apis

|----------------|-----------|
|migration state | unstarted |

### ptusa_microservices

|----------------|-----------|
|migration state | unstarted |

### ptusa_shared_library_v2

|----------------|-----------|
|migration state | unstarted |

### WebAnythingStudioExampleModules

|----------------|-----------|
|migration state | unstarted |

### iratefun_utility_classes

|----------------|-----------|
|migration state | migrated but untested |

2024-06-26: 
Migrated the class loader to the new system of integration, but have not yet tested if everything is working as expected.  Running the library loader loads all expected classes, but those classes have not been tested.

### ptusa_app_server

|----------------|-----------|
|migration state | unstarted |

### ptusa_cdp_client

|----------------|-----------|
|migration state | unstarted |

### ptusa_microservice__skeleton_project

|----------------|-----------|
|migration state | unstarted |

### ptusa_utility_classes

|----------------|-----------|
|migration state | unstarted |

### iratefun_website

|----------------|-----------|
|migration state | unstarted |

### ptusa_audit_cluster_client_v2_unit_tests

|----------------|-----------|
|migration state | unstarted |

### ptusa_cdp_client_modified_during_pentest

|----------------|-----------|
|migration state | unstarted |

### ptusa_pentest_client_v2

|----------------|-----------|
|migration state | unstarted |

### SpokeWebServer

|----------------|-----------|
|migration state | unstarted |
