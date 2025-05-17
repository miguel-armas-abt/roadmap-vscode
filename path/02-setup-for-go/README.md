# CONFIGURACIÓN PARA GO

[← Regresar a notas](../../README.md) <br>

---

> ### ⚙️ Extensión para Go
> Identifier: `golang.go`
> 
> ![img.png](resources/golang.go.png)

> ### ⚙️ Settings.json
> ```json
> {
>   "terminal.integrated.defaultProfile.windows": "Git Bash",
>   
>   //style
>   "workbench.colorTheme": "JetBrains Darcula Theme",
>   "editor.fontFamily": "JetBrains Mono, Fira Code, Consolas, 'Courier New', monospace",
>   "editor.fontLigatures": true, // change this kind of symbols "->"
> 
>   "go.formatTool": "gofumpt", //goimports, gofumpt
>   "[go]": {
>     "editor.codeActionsOnSave": {
>       "source.organizeImports": "explicit", //always, explicit
>     },
>     "editor.codeLens": true
>   },
> 
>   "go.enableCodeLens": {
>     "runtest":    true
>   },
> 
>   "gopls": {
>     "ui.semanticTokens": true,
>     "completeUnimported": true,
>     "ui.completion.usePlaceholders": true,
>     "staticcheck": false,
>     "analyses": {
>       "unusedparams": true,
>       "shadow": true
>     },
>     "completionBudget": "50ms",
>     "diagnosticsDelay": "250ms"
>   }
> }
> ```

> ### ⚙️ tasks.json
> ```json
> {
> 	"version": "2.0.0",
> 	"tasks": [
> 		//ctrl + f9
> 		{
> 			"label": "Go: Build Project",
> 			"type": "shell",
> 			"command": "go build ./...",
> 			"group": {
> 				"kind": "build",
> 				"isDefault": true
> 			},
> 			"problemMatcher": [
> 				"$go"
> 			],
> 			"presentation": {
> 				"reveal": "always",
> 				"panel": "shared"
> 			}
> 		}
> 	]
> }
> ```