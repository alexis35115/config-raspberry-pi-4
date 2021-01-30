# Configuration de son Raspberry Pi

Voici la configuration nécessaire pour son Raspberry Pi dans le cadre du cours 420-253-MT Objets connectés

-- > parler des configurations pour le raspberry pi de base?


## Logiciels

mentionner le 32 versus le 64?

### Git

Installation :

```sh
sudo apt update
sudo apt install git
```

Valider l'installation :

```sh
git --version
```

Configuration initiale :

```sh
# Mettre vos informations
git config --global user.name "john doe"
git config --global user.email "johndoe@mail.com
```

Valider la configuration initiale :

```sh
git config --list
```

### Visual Studio Code

https://code.visualstudio.com/download

```sh
curl -L https://raw.githubusercontent.com/headmelted/codebuilds/master/docs/installers/apt.sh | sudo bash
```

gist des settings? + elle pour le formattage?

#### Extensions

```sh
code --install-extension bmewburn.vscode-intelephense-client
code --install-extension DavidAnson.vscode-markdownlint
code --install-extension donjayamanne.githistory
code --install-extension eamodio.gitlens
code --install-extension EditorConfig.EditorConfig
code --install-extension ms-python.python
code --install-extension ms-toolsai.jupyter
code --install-extension ms-vscode.vs-keybindings
code --install-extension vscode-icons-team.vscode-icons
code --install-extension yzane.markdown-pdf
code --install-extension PhonicCanine.micro-bit
```

valider l'autoformatting

linting https://code.visualstudio.com/docs/python/linting#_enable-linters

```json
{
    "editor.tabCompletion": "on",
    "editor.suggestSelection": "first",
    "editor.rulers": [80,120],
    "editor.fontSize": 18,
    "editor.quickSuggestions": {
        "other": true,
        "comments": false,
        "strings": false
    },
    "editor.fontLigatures": true,
    "editor.fontFamily": "'Cascadia Code PL'",
    "emmet.showAbbreviationSuggestions": true,
    "editor.renderIndentGuides": false,
    "[markdown]": {

        "editor.wordWrap": "on",
        "editor.quickSuggestions": false
    },
    "terminal.integrated.fontFamily": "'Cascadia Code PL'",
    "workbench.iconTheme": "vscode-icons",
    "editor.wordWrap": "on"
}
```

### Python

Python devrait être installé par défaut, il est possible de vérifier s'il est présent en utilisant la commande :

Installation :

```sh
sudo apt update
sudo apt install python3 python3-pip idle3
```

Vérifier l'installation :

```sh
python3 --version
```

### autres?


Installation de Python - déjà là?


_Dans le cadre du cours 420-253-MT Objets connectés_

Tous droits réservés 2021 © Alexis Garon-Michaud
