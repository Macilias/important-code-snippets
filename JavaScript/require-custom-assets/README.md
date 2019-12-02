This was a real real pain in the a**

How ever to be able to get it up and running one must know the following
1. The custom package need to be referenced from the app/package.json and
2. even more importantly, from package-lock.json with `"version": "file:custom-assets"` annotation!
3. The package.json must contain a "main" entry which references one of the files inside and its path must start with `./`!!!


you can test it with: `$ node index.js` 
and verify with:
``` 
$ node 
> module.paths
[
  '.../important-code-snippets/JavaScript/require-custom-assets/repl/node_modules',
  '.../important-code-snippets/JavaScript/require-custom-assets/node_modules',

```



