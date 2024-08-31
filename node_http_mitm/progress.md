# Node HTTP MITM Server Semi-Rewrite

- [x] Stripped out typescript and confirmed it's still working.
- [x] Analyzed code base and reformatted code to make it look to our standard.
- [ ] Moved code to their own respective classes.
    - [ ] HTTPMITMProxyFinalRequesFilter.class.js
    - [ ] HTTPMITMProxyFinalResponseFilter.class.js
    - [ ] HTTPMITMCertificateAuthority
    - [ ] HTTPMITMProxy
- [ ] Renamed classes to be more distinct and relative to the HTTP MITM project to prevent potential confusion with other classes in the class library.
- [ ] removed instances of "self" and replaced them with classname_ref.
