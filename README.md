# Code Runner

[![Marketplace Version](http://vsmarketplacebadge.apphb.com/version/formulahendry.code-runner.svg)](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner) [![Installs](http://vsmarketplacebadge.apphb.com/installs/formulahendry.code-runner.svg)](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner) [![Rating](http://vsmarketplacebadge.apphb.com/rating/formulahendry.code-runner.svg)](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner) [![Build Status](https://travis-ci.org/formulahendry/vscode-code-runner.svg?branch=master)](https://travis-ci.org/formulahendry/vscode-code-runner)

Run code snippet or code file for multiple languages: **javascript, php, python, perl, ruby, go, lua, groovy, powershell, bat/cmd, bash/sh, F# script, C# script**

## Features

* Run code file of current active Text Editor
* Run selected code snippet in Text Editor
* Stop code running
* View output in Output Window

## Usages

* Open code file or select code snippet in Text Editor, then use shortcut `Ctrl+Alt+N`, or press `F1` and then select/type `Run Code`, the code will run and the output will be shown in the Output Window.
* To stop the running code, use shortcut `Ctrl+Alt+M`, or press `F1` and then select/type `Stop Code Run`

![Usage](images/usage.gif)

## Configuration

Make sure the interpreter PATH of each language is set in the environment variable.
You could also add entry into `code-runner.executorMap` to set the interpreter PATH.
e.g. To set the interpreter PATH for ruby and php:
```json
{
    "code-runner.executorMap": {
        "javascript": "node",
        "php": "C:\\php\\php.exe",
        "python": "python",
        "perl": "perl",
        "ruby": "C:\\Ruby23-x64\\bin\\ruby.exe",
        "go": "go run"
    }
}
```

## Note
To run C# script, you need to install [scriptcs](http://scriptcs.net/)

## Change Log
### 0.0.5
* Add support for C# script

### 0.0.4
* Add support for F# script

### 0.0.3
* Add support for powershell, bat/cmd and bash/sh

### 0.0.2
* Add support for lua and groovy

### 0.0.1
* Initial Release

## Issues
Submit the [issues](https://github.com/formulahendry/vscode-code-runner/issues) if you find any bug or have any suggestion.

## Contribution
Fork the [repo](https://github.com/formulahendry/vscode-code-runner) and submit pull requests.