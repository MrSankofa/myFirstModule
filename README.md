tsc build based on your tsconfig file.

if you do not have a tsconfig file or there is some 
typo in your code it will look in the current dir
for ts file and transpile them to js es5 by default.

You generally need this to create a basic module
```
{
  "compilerOptions": {
    "outDir": "./dist/",
    "module": "commonjs",
    "target": "es5"
  },
  "include": ["./"]
}
```
