# INIT-TS-PROJECT

Project showing how to create a TS project from scratch

# How-To #

Initialize your JS project with NPM

    $ npm init

This will create a ``package.json`` file.

Now we have to add typescript to our project :

    $ npm install -g typescript

Now we have to create a ``tsconfig.json`` file : 

    $ npx tsc --init

We can set some properties for our project. For this one, we will uncomment the "OutDir" property and set a specific value :

```JSON
"outDir": "./dist"
```

This will create a ``dist`` folder where all compiled js will be placed

Create an ``index.js`` file in a ``src/`` folder and write some code in it. After that, select the folder where the ``tsconfig.json`` file is. Use the next command :

    $ npx tsc

Now the dist folder is create with all sources written in JS. You can execute the index.js with the next command :

    $ cd dist/
    $ node index.js