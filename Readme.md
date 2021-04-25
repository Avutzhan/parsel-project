### Errors list

* Packages uncompatibility 

when i installed latest parcel-bundler and run ``` npm start``` thrown error 

```angular2
> parsel-project@1.0.0 start /home/avutzhan/myprojects/parsel-project
> parcel index.html

Server running at http://localhost:1234 
🚨  /home/avutzhan/myprojects/parsel-project/index.js: function __clone() {
    var node2 = new Node();
    for (var key in this) {
      // Do not clone comments tha...<omitted>... } could not be cloned.
    var node2 = new Node();
    for (var key in this) {
      // Do not clone comments tha...<omitted>... } could not be cloned.
    at Object.serialize (v8.js:206:7)
    at _default (/home/avutzhan/myprojects/parsel-project/node_modules/@babel/core/lib/transformation/util/clone-deep.js:16:30)
    at normalizeFile (/home/avutzhan/myprojects/parsel-project/node_modules/@babel/core/lib/transformation/normalize-file.js:52:36)
    at normalizeFile.next (<anonymous>)
    at run (/home/avutzhan/myprojects/parsel-project/node_modules/@babel/core/lib/transformation/index.js:31:50)
    at run.next (<anonymous>)
    at Function.<anonymous> (/home/avutzhan/myprojects/parsel-project/node_modules/@babel/core/lib/transform-ast.js:20:41)
    at Generator.next (<anonymous>)
    at evaluateSync (/home/avutzhan/myprojects/parsel-project/node_modules/gensync/index.js:251:28)
    at Function.sync (/home/avutzhan/myprojects/parsel-project/node_modules/gensync/index.js:89:14)

```

after reinstalling parcel-bundler@1.7.1 error solved and build run normally