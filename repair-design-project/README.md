#repair-design-project
Start of project:
1. Create index.html and style.scss
2. install Live Sass Compiler in VSC
3. Create a .vscode folder in the root of project.
4. Inside of .vscode folder create a json file named settings.json
5. Inside of settings.json write a code:
  ```
   {
     "liveSassCompile.settings.formats":[
        {
            "format": "expanded",
            "extensionName": ".css",
            "savePath": "/css"
        },
        {
            "extensionName": ".min.css",
            "format": "compressed",
            "savePath": "/dist/css"
        }
    ],
    "liveSassCompile.settings.excludeList": [
       "**/node_modules/**",
       ".vscode/**"
    ],
    "liveSassCompile.settings.generateMap": true,
    "liveSassCompile.settings.autoprefix": [
        "> 1%",
        "last 2 versions"
    ]
}
```