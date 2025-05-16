# ESTILO JETBRAINS

[← Regresar a notas](../../README.md) <br>

---
[1. Instalar plugins](#1-instalar-plugins) <br>
[2. Settings.json](#2-settingsjson) <br>

---

## 1. Instalar plugins

> > ### ⚙️ JetBrains IDE Keymap
> 
> - Identifier: `isudox.vscode-jetbrains-keybindings` <br>
> - Plugin para shortcuts
>
> ![img.png](resources/jetbrains-ide-keymap.png)

> > ### ⚙️ Material Icon Theme
> - Identifier: `pkief.material-icon-theme` <br>
> - Plugin para íconos
> 
> ![img.png](resources/jetbrains-icon-theme.png)
> 
> 📌 **Nota**: En caso no se haya establecido por defecto, entonces abra la paleta de comandos `ctrl+shift+p`, selecciona `Preferences: File Icon Theme` y a continuación `JetBrains Icon Theme v1 Dark`.
> 
> ![img.png](img.png)

> > ### ⚙️ JetBrains Darcula Theme
> - Identifier: `anan.jetbrains-darcula-theme`
> - Plugin para tema oscuro
> 
> ![img.png](resources/jetbrains-darcula-theme.png)
> 📌 **Nota**: En caso no se haya establecido por defecto, entonces abra la paleta de comandos `ctrl+shift+p`, selecciona `Color Theme` y a continuación, `JetBrains Darcula Theme`.

> > ### ⚙️ JetBrains Mono
> - Identifier: `narasimapandiyan.jetbrainsmono`
> - Plugin para fuente de texto
> 
> ![img.png](resources/jetbrains-mono.png)
> 
> 📌 **Nota**: El plugin descargará las fuentes en `C:\Users\<user>\.vscode\extensions\narasimapandiyan.jetbrainsmono-1.0.2\JetBrainsMono`. A continuación, instalarlas en `Windows/Fonts`.

> > ### ⚙️ Error Lens
> - Identifier: `usernamehw.errorlens`
> - Plugin para resaltar la línea que contiene errores y especificar su motivo.
>
> ![img.png](resources/error-lens.png)

## 2. Settings.json
```json
{
  "keyboard.dispatch": "keyCode", //shortcuts
  "workbench.colorTheme": "One Dark Pro",
  "files.autoSave": "onFocusChange", // autosave
  "editor.fontFamily": "JetBrains Mono, Fira Code, Consolas, 'Courier New', monospace",
  "editor.fontLigatures": true // change this kind of symbols "->" 
}
```