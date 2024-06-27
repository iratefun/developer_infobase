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

PentestUSA projects are fairly large, and contain very useful code, but due to the organization being defunct/disolved we'll be migrating those projects after iratefun projects.  Of special note, we have the auditcluster websocket api server, which allows for simultaneous event driven controls to utilize a single connection using a system of trancievers. We want to separate that functionality into it's own standalone project, which is easily integratable into the SpokeWebServer.

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
|project uuid|6709b687-974d-4473-967d-f8956942cb95|



### letsencryptserver

|----------------|-----------|
|migration state | unstarted |
|project uuid|0ab471e3-4edc-4d39-819c-4eeb5585f3ec|

### ptusa_audit_cluster_v2

|----------------|-----------|
|migration state | unstarted |
|project uuid|592012ed-f1a1-4216-b762-3f5f02c3b4e4|

### ptusa_deployment_tool

|----------------|-----------|
|migration state | unstarted |
|project uuid|00cc1871-8f51-46e0-80cf-e816561185c3|

### ptusa_scriptrunner

|----------------|-----------|
|migration state | unstarted |
|project uuid|681f6548-f203-4d11-93b2-202e5738f38c|


### WebAnythingStudio

|----------------|-----------|
|migration state | unstarted |
|project uuid|f0065b30-0ee3-4639-a0b5-70b0157ee049|

### iratefun_tooling

|----------------|-----------|
|migration state | unstarted |
|project uuid|53c4b27a-50ab-43af-a2c3-5fb8bf259a24|

### ptusa_alexander

|----------------|-----------|
|migration state | unstarted |
|project uuid|26e3fc91-27cb-49c0-8a59-0263d8d2a7e6|

### ptusa_audit_cluster_v2__worker_thread_apis

|----------------|-----------|
|migration state | unstarted |
|project uuid|90e060b3-c07e-4f1c-935f-54139dddea12|

### ptusa_microservices

|----------------|-----------|
|migration state | unstarted |
|project uuid|3f5233b8-6447-4acd-bcd5-a67d658e6b84|

### ptusa_shared_library_v2

|----------------|-----------|
|migration state | unstarted |
|project uuid|106b7bf1-0c31-49a5-8c6d-5d5ff8bfbdb6|

### WebAnythingStudioExampleModules

|----------------|-----------|
|migration state | unstarted |
|project uuid|ec60f443-2c91-45e8-a863-1e40de179f76|

### iratefun_utility_classes

|----------------|-----------|
|migration state | migrated but untested |
|project uuid|69b2fc0d-9d64-485c-8f91-de5d9350395a|

2024-06-26: 
Migrated the class loader to the new system of integration, but have not yet tested if everything is working as expected.  Running the library loader loads all expected classes, but those classes have not been tested.

### ptusa_app_server

|----------------|-----------|
|migration state | unstarted |
|project uuid|896c348f-0e13-459a-b327-13469f7ff05c|

### ptusa_cdp_client

|----------------|-----------|
|migration state | unstarted |
|project uuid|db3d716e-a218-4aab-abdf-cc8694a8b3e6|

### ptusa_microservice__skeleton_project

|----------------|-----------|
|migration state | unstarted |
|project uuid|f65a55b8-fdab-4adc-9410-f86d4e21eab1|

### ptusa_utility_classes

|----------------|-----------|
|migration state | unstarted |
|project uuid|5d483f5e-cc3c-4a43-afc3-042652437089|

### iratefun_website

|----------------|-----------|
|migration state | unstarted |
|project uuid|08e6091a-ecd4-4821-ae6f-ef35c3c5fac6|

### ptusa_audit_cluster_client_v2_unit_tests

|----------------|-----------|
|migration state | unstarted |
|project uuid|86b98ecd-b999-4901-a38b-4b3a79750110|

### ptusa_cdp_client_modified_during_pentest

|----------------|-----------|
|migration state | unstarted |
|project uuid|0e8e20ae-df8f-47b3-b77c-ceb6eae8b340|

### ptusa_pentest_client_v2

|----------------|-----------|
|migration state | unstarted |
|project uuid|33c94c9a-388f-4ea6-bd7d-8fc584e103e9|

### SpokeWebServer

|----------------|-----------|
|migration state | unstarted |
|project uuid|8635be15-184e-477c-b640-fd4689140247|
