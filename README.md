
# atom-standard-formatter

Atom package to format your Javascript using [Standard Style](https://github.com/feross/standard), [Semi-Standard Style](https://github.com/Flet/semistandard)

![](https://cloud.githubusercontent.com/assets/5852428/8020717/adbf10c0-0c51-11e5-8537-2714c9f698e5.gif)

### Usage

#### Keybindings

Use `Ctrl-Alt-F` to format the current Javascript file. If a text selection is made, only the selected text will be formatted.

#### Format On Save

Automatically format your Javascript file on save by enabling the _Format On Save_ package setting.  This is off by default.

#### Menu

_Packages &gt; Standard Formatter &gt; Format_

### Settings

#### formatOnSave \(default: false\)

Format Javascript files when saving.

#### checkStyleDevDependencies \(default: false\)

Check code style in package.json `devDependencies`. If a valid style is not found it won't format.

\| Note: This will use the nearest package.json

#### style \(default: standard\)

Choose the style formatter module you want to use. If `checkStyleDevDependencies` is `true` this setting will be ignored.

* [standard](https://github.com/feross/standard) - equivalent to running `standard --fix`

* [semi-standard](https://github.com/Flet/semistandard) - equivalent to running `semistandard --fix`

#### honorPackageConfig \(default: true\)

Don't auto-format files included in the package.json's `"ignore"` configuration for the detected style.

\| Note: This will use the nearest package.json

### A note on formatting

This package relies on the excellent work from the following modules to perform formatting:

* [standard](https://github.com/feross/standard)

* [semi-standard](https://github.com/Flet/semistandard)

Code based on the https://github.com/standard/atom-standard-formatter package. Changes made:
 - Package updated to the newest software versions - original package wasn't updated since 2017
 - Removed Happiness, Standard-format, Semistandard-format
 - Added Prettier option
