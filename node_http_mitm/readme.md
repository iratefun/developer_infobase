# Node HTTP MITM Server Semi-Rewrite

- [x] Stripped out typescript and confirmed it's still working.
- [x] Analyzed code base and reformatted code to make it look to our standard.
- [ ] Moved code to their own respective classes.
    - [x] HTTPMITMProxyFinalRequesFilter.class.js
    - [x] HTTPMITMProxyFinalResponseFilter.class.js
    - [x] HTTPMITMCertificateAuthority.class.js
    - [x] HTTPMITMProxy.class.js
- [x] Renamed classes to be more distinct and relative to the HTTP MITM project to prevent potential confusion with other classes in the class library.
- [x] removed instances of "self" and replaced them with classname_ref.
- [x] make copy of HTTPMITMProxy.class.js  (saved as HTTPMITMProxy.class.js.workingbackup)
- [ ] Make callbacks work linearly using async/await instead of async.forEach.  We want to do this to guarantee the order in which callbacks are executed.  We never want a situation where they are not executed in the order they are run.
    - [x] _onHttpServerConnect
    - [ ] _onHttpServerConnectData
    - [ ] _onError
    - [ ] _onWebSocketServerConnect
    - [ ] _onHttpServerRequest
    - [ ] _onRequestHeaders
    - [ ] _onRequest
    - [ ] _onWebSocketConnection
    - [ ] _onWebSocketFrame
    - [ ] _onWebSocketClose
    - [ ] _onWebSocketError
    - [ ] _onRequestData
    - [ ] _onRequestEnd
    - [ ] _onResponse
    - [ ] _onResponseHeaders
    - [ ] _onResponseData
    - [ ] _onResponseEnd

## _onHttpServerConnect: Async/Awaitification
- [x] Changed to async function
- [x] Moved from async.forEach to linear loop.
- [x] Tested and confirmed working.
- [ ] Added a test event listener.

## _onHttpServerConnectData: Async/Awaitification
- [x] Changed to async function
- [ ] Moved makeConnection() from a local function to a class method.
- [ ] Moved getHttpsServer() from a local function to a class method.
- [ ] changed makeConnection() to be an async function.
- [ ] changed getHttpsServer() to be an async function.
- [ ] removed _onSocketError() callback.
- [ ] modified return syntax to not use makeConnection as a return, as it implies a value is being returned, when in reality makeConnection returns nothing.
- [ ] modified each makeConnection call to await.
- [ ] Moved from async.forEach to linear loop.
- [ ] Tested and confirmed working.

