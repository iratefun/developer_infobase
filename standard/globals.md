# Standard Globals

To make development easier, we do use a few globals which are set within the nodejs process global.  Things like dependencies, and loaded libraries are shared between files via the process object.

# process.irf_core

An irf_core object should always be made present in any of the following: 

* process
* thread
* worker

```
process.irf_core = 
{
    deps: {},
    libraries: {}
};
```
