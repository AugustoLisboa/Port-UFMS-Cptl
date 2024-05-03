# Extensão de sintaxe p/ VSCODE -> Portugol CPTL README
## Recomendado *APENAS* para uso em sala de Aula
Extensão desenvolvida para facilitar o uso da pseudo-linguagem "Portugol" em sala de aula. A extensão de arquivo ".ufms" passa a ser reconhecida pelo Visual Studio Code, colorindo palavras reservadas, operadores aritiméticos, etc.

## Features
- Sintaxe reconhecida pelo editor
- Snippets de estrutura
- Fechamento automático de operações

![Screen Recording 2024-05-03 at 20 21 14](https://github.com/AugustoLisboa/Port-UFMS-Cptl/assets/60906217/45e3b237-4847-4d43-a81a-ccdef95d0155)


## Requirements

- Visual Studio Code
- Fontes compatíveis com "FontLigatures" (Ex: JetBrainsMono)

## Manual de instalação:
* Faça download da pasta "portugol" e mova para sua pasta de extensões do VSCode
  - Windows %USERPROFILE%\.vscode\extensions.
  - macOS/Linux ~/.vscode/extensions.
* Adicione as configurações necessárias no "settings.json" do VSCode
```
    "editor.fontFamily": "JetBrains Mono",   //Define a fonte a ser utilizada
    "editor.fontLigatures": true,            //Habilita o FontLigatures
    "editor.tokenColorCustomizations": {     //Define as cores das palavras reservadas
        "textMateRules": [
            {
                "scope": "keyword.control.ufms",
                "settings": {
                    "fontStyle": "underline",
                    "foreground": "#ffb16d"
                }
                
            },
            {
                "scope": "keyword.ufms",
                "settings": {
                    "fontStyle": "underline",
                    "foreground": "#f455ff"
                },
                
            }
        ]
    }
  ```
Para alterar as cores utilizadas pelas extensão, basta alterar a variável "foreground:" no settings.json.
* Salve as alterações e reinicie o VSCode
