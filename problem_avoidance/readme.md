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
