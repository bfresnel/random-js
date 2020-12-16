# INIT-TS-PROJECT

Project showing how to create a TS project from scratch

# Initialize the project

Simply execute this command (Ensure you are in ``init-ts-project/`` folder)

    $ npm install

# How i made this project #

Initialize your JS project with NPM

    $ npm init

This will create a ``package.json`` file.

Now we have to add typescript to our project :

    $ npm install typescript --save-dev

Now we have to create a ``tsconfig.json`` file : 

    $ npx tsc --init

We can set some properties for our project. For this one, we will uncomment the "OutDir" property and set a specific value :

```JSON
"outDir": "./dist"
```

This will create a ``dist`` folder where all compiled js will be placed

Create an ``index.js`` file in a ``src/`` folder and write some code in it. After that, select the folder where the ``tsconfig.json`` file is. Use the next command :

    $ npx tsc

<em>**NOTE: the npx command is specific in this case because we don't install typescript globally. It allows to use tsc (TypeScriptCompiler) without setting typescript globally**</em>

Now the ``dist`` folder is created with all sources written in JS. You can execute the ``index.js`` file with the next command :

    $ cd dist/
    $ node index.js