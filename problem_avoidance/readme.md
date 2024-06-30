# Problem Avoidance

This is just to hold information about problems that we fix, but often forget why, and how they influence axioms.

## Bundle Builders and require/import

esbuild and webpack are fairly stupid in that they do not handle dynamic requires/imports well.  For this reason the code features "ugly" syntax like as follows:

```
// add base dependencies
addDeps
({
    path  : require("path"),
    events: require("events"),
    async : require("async"),
    util  : require("util")
});
```

Requires or imports must be called with literal strings, not variables, or esbuild can crap out.  This means a lot of things are hard coded when building bundles.

# NodeSEA Building Duplicate Fuse Sentinel Errors

When you encounter the following error when building a nodesea bundle:
```
Multiple occurences of sentinel "NODE_SEA_FUSE_fce680ab2cc467b6e072b8b5df1
```

It's because nodejs is stupid in how it looks for the sentinel.  It doesn't parse the binary, or do anything fancy, it simply looks for the string.  In our case, prcr__abraxas__runnable, is used to build nodesea binaries, therefore it contains the string "NODE_SEA_FUSE_fce680ab2cc467b6e072b8b5df1" in it's bundle.  This causes the error to occur. 
To avoid the error, you have to split the string into two pieces so that node checks the bundle and doesn't find a single string matching NODE_SEA_FUSE_fce680ab2cc467b6e072b8b5df1.

Example:
```
var node_sentinel_trailing = `6e072b8b5df1996b2`;
var node_sentinel_string = `NODE_SEA_FUSE_fce680ab2cc467b${node_sentinel_trailing}`;
```
 
