# TypeScript

TypeScript is a programming language developed and maintained by Microsoft. It is a strict syntactical superset of JavaScript and adds optional static typing to the language. It is designed for the development of large applications and transpiles to JavaScript.

## How to Install the Compiler on local System
```
npm install typescript --save-dev or npm i -g typescript
```
The compiler is installed in the node_modules directory and can be run with:  ```npx tsc```

## Configuring the compiler
By default the TypeScript compiler will print a help message when run in an empty project.

The compiler can be configured using a ```tsconfig.json``` file.

You can have TypeScript create ```tsconfig.json``` with the recommended settings with:

```
npx tsc --init
```

<hr>

```
{
  "include": ["src"],
  "compilerOptions": {
    "outDir": "./build"
  }
}
```
You can open the file in an editor to add those options. This will configure the TypeScript compiler to transpile TypeScript files located in the src/ directory of your project, into JavaScript files in the build/ directory.


## How to Transpile
```
tsc -w
```