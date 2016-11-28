# SCs Language Support README

To use clone/copy this repo to the "Users/<USER>/.vscode/extensions/" folder.

For more pretty code look try using one of the ligatured fonts (e.g. Fira Code, Hasklig, etc.) - you can enable ligatures in VSCode settings - or/and [Prettify Symbols Mode extension][1].

## Features

SCs language support.

* Syntax coloring.
* Code snippets.

![syntax coloring example](http://i.imgur.com/3Xwlwm6.png)

## Requirements

None for now.

## Extension Settings

None for now.

## Known Issues

If using ligatured font (Fira Code, Hasklig, etc.) you'll have ⇐ symbol treated as ⩽. To avoid this either disable ligatures in VS Code settings, or use [Prettify Symbols Mode extension][1] with following settings for substitutions:

```json
"prettifySymbolsMode.substitutions": [
    "language": "scs",
    "substitutions": [
        {
            "ugly": "<=",
            "pretty": "⇐"
        },
        {
            "ugly": "=>",
            "pretty": "⇒"
        }
    ]
]
```

P.S.: There could be also some troubles with ⇒ symbol (no ligature for it) so there is a substitution for it too.

## Release Notes

### 0.0.1

Initial release: just SCs syntax coloring and some braces configuration.

### 0.0.2

Some snippets added.

-----------------------------------------------------------------------------------------------------------

## Contributors

* [Peter Gorban](https://github.com/msifd)
* [Artemy Bordushko](https://github.com/ArtemyB)

**Enjoy!**

[1]: https://github.com/siegebell/vsc-prettify-symbols-mode