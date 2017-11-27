# inspired-by-promyze
Setup Code Quality

## Use of unified code style config
Here is an intelliJ code style config for : java, js, ts, html, css, scss files :
 > codestyle/intelliJ/neo9-codestyle.xml
 
 Another for vscode is comming :
 > // TODO 
 
## Linter on your project(s)
Linters are programs that analyze statically the source code of a project and verify if coding standards are respected 
 #### Javascript Linter
 My Choice for ECMAscript/Javascript code is ESLINT
 ```json
 {
 	"env": {
 		"amd": true,    // for require() keyword
 		"node": true,   // nodeJS global varibales
 		"browser": true // browsers global variables
 	},
 	"plugins": [
 		"angular" // here you can add plugin for built-in rules
 	],
 	"rules": {
 		"eqeqeq": ["errors","always"],
 		"quotes": ["warn", "single"],
 		"strict": "off",
 		"eol-last": "off",
 		"no-use-before-define": 0,
 		"angular/ng_on_watch": 0 // from angular plugin
 	},
 	"globals": { // global varibales to avoid undef error
 		"angular": true,
 		"_": true,
 		"moment":true
 	}
 }
 ```
 
 
# Automate them all