Npm Link Demo
=============

We don't need to publish to npmjs when developing npm projects.

Register current project to local:

```
npm link
```

Use it in another project:

```
cd testing-project
npm link my-npm-lib
```

and run:

```
node index.js
```

You will see the function `hello` from the root project is calling successfully.


If we modify code in `my-npm-lib`, we don't need to do anything to use the new code in `testing-project`.