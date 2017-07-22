# scss-lint README

This is a small scss-lint extension for vscode.

![Alt text](images/demo.gif?raw=true "Demo Gif")

## Features

This extention runs scss-lint in bash and displays the errors found by highlighting the errors in your scss files upon saving of that file.

## Requirements

This extention is dependant on the ruby gem scss-lint. It has only been tested with version .0.49.0 of scss_lint so we therefore suggest you run the following in your terminal:
`gem install scss_lint -v 0.49.0`

## Extension Settings

This extension runs scss-lint which uses your .scss-lint.yml file. Simply install the extension, and it works.
scssLint.showHighlights sets whether or not to show highlights in addition to underlines.
scssLint.errorBackgroundColor sets the error background color and defaults to "rgba(200, 0, 0, .8)".
scssLint.warningBackgroundColor sets the warning background color and defaults to "rgba(200, 120, 0, .8)".
scssLint.languages sets the languages this extension works with. It defaults to ["scss"]. To add css make it ["scss", "css"].
scssLint.statusBarText sets what the status bar text should read.

Default settings

```settings.json
{
    "scssLint.showHighlights": false,
    "scssLint.errorBackgroundColor": "rgba(200, 0, 0, .8)",
    "scssLint.warningBackgroundColor": "rgba(200, 120, 0, .8)",
    "scssLint.languages": [
        "scss"
    ],
    "scssLint.statusBarText": "`$(telescope) scss-lint  ${errors.length} $(x)  ${warnings.length} $(alert)`",
    "scssLint.configDir": ""
}
```

To add css support change to this:

```settings.json
{
    "scssLint.showHighlights": false,
    "scssLint.errorBackgroundColor": "rgba(200, 0, 0, .8)",
    "scssLint.warningBackgroundColor": "rgba(200, 120, 0, .8)",
    "scssLint.languages": [
        "css",
        "scss"
    ],
    "scssLint.statusBarText": "`$(telescope) scss-lint  ${errors.length} $(x)  ${warnings.length} $(alert)`",
    "scssLint.configDir": ""
}
```

## Known Issues

Known issues are tracked on github. Feel free to post them there or resolve some of the issues you see.

## Release Notes

### See the [CHANGELOG](CHANGELOG.md) for notes on each release.

-----------------------------------------------------------------------------------------------------------

## Thanks

We must thank [sass](http://sass-lang.com), [scss-lint](https://github.com/brigade/scss-lint), and [vscode-wordcount](https://github.com/Microsoft/vscode-wordcount) for the help they provided in making this extension.

Also, thank you to [@youdame](https://github.com/yoodame) for his PR making this extension work even when the .scss-lint.yml isn't in the root directory of the project and to [@donni106](https://github.com/donni106) for his help identifying and finding solutions to issues with the extension.

**Enjoy!**
